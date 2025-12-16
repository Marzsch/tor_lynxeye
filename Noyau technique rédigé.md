
## Préparation du terrain et données initiales

### Data providers pour la phase de pré-déploiement 

Les données utilisées pour construire la carte d'initialisation proviennent exclusivement de sources institutionnelles et d'expertise terrain : 

- **Topographie / Modèles Numériques de Terrain (MNT)** : agences nationales de cartographie (pente, orientation, altitude, rugosité).
- **Occupation des sols et végétation** : bases environnementales officielles (types de couvert, biomasse, continuité du combustible).
- **Météo et climatologie** : services météorologiques nationaux (régimes de vent dominants, sécheresse saisonnière, climatologie).
- **Données satellites** : programmes institutionnels (ex. Copernicus Sentinel) pour les indices de végétation, d’humidité et de température de surface.
- **Expertise terrain** : SDIS, ONF, gestionnaires du site, pour la validation qualitative des zones sensibles.
### Importance d’une connaissance **a priori** du territoire

Le moteur de risque LynxSense ne peut être calibré correctement qu’à partir d’une connaissance fine du territoire étudié.  

Le risque d’ignition et de propagation n’est pas uniforme :  
il dépend d’un ensemble de facteurs intrinsèques - végétation, topographie, microclimat - qui doivent être cartographiés avant toute modélisation.

Le territoire observé $\Omega \subset \mathbb{R}^{2}$ est vu comme un espace hétérogène où chaque point possède un ensemble de caractéristiques environnementales regroupées en un vecteur $z(\mathbf{x})$.

Plus formellement, pour chaque point $x \in \Omega$, on définit un vecteur de caractéristiques associées :
$$ \mathbf{z}(x) = ( z^{veg}(x), z^{topo}(x), z^{hydro}(x), z^{clim}(x), z^{anth}(x), z^{hist}(x))$$
Chaque bloc capture un aspect essentiel du risque, tel que : 

1) Variables de végétation et de biomasse ($z^{veg}(x)$) :

	La végétation est le principal combustible. 
	Ainsi le risque dépend donc de :
	
	-  Type de couverts : forêt dense, conifères, maquis, broussailles, prairies, sol nu; 
	- Densité de biomasse au sol et en hauteur;
	- Continuité du couvert végétal
	- Inflammabilité intrinsèque du combustible

$$z^{veg}(x) = (type^{veget}(x),density^{soil}(x), density^{canopy}(x), NDVI(x), NDWI(x))$$
où NDVI (Normalized Difference Vegetation Index) et NDWI (Normalized Difference Water Index) sont dérivés de données satellites.

![[Pasted image 20251212142500.png]]

![[Pasted image 20251212142401.png]] ![[Pasted image 20251212142428.png]]

La variable $z^{veg}(x)$ capte la charge combustible + humidité végétale, ce qui permet de produire une première idée du risque d'ignition.

2) Variables topographiques : $z^{topo}(x)$ 

La topographie influence l'extraction de l'humidité, la vitesse de propagation, l'exposition solaire.
$$z^{topo}(x) = (slope(x), orientation(x), altitude(x), rugosity(x))$$
Les variables essentielles, sont avant tout $slope$ et $orientation$, qui vont aider à structurer les pathways physiques pour la propagation inter-clusters. 

3) Variables hydriques et état du sol : $z^{hydro}(x)$ 

Elles déterminent la teneur hydrique du combustible, de façon plus affinée.

$$z^{hydro}(x) = (humidity^{soil}(x), stress^{hydric}(x), PET(x), rain^{cumulated}(x)) $$

où $PET$ est le Potential Evapotranspiration, la capacité d'un sol à faire s'évaporer l'eau en cas d'approvisionnement suffisant et $stress^{hydric}$, le déficit entre besoin en eau et eau disponible.

Ces variables permettent de donner une idée de la tension inflammable du sol et de la végétation.

4) Variables climatiques et météorologiques : 

Elles caractérisent les conditions structurelles locales : 

$$ z^{clim}(x) = (temp^{avg}(x), wind^{dominating}(x), humidity^{avg}(x), dryness^{seasonal}(x))$$
Cela décrit les **patterns persistants** du climat local, indépendants de la météo instantanée, orientant la sélection des DRCs vers des zones systémiquement sèches ou chaudes.

5) Variables anthropiques : 

Sachant que près de 9 feux sur 10 sont déclenchés par l'activité humaine, il est critique de modéliser ce facteur humain dans nos calculs : 

$$z^{anth}(x) = (distance^{roads}(x), distance^{trail}(x), visitors(x), proximity^{camping}(x), proximity^{houses}(x))$$

6) Variables historiques et mémoire du risque : 

$$z^{hist}(x) = (fire^{rate}(x), frequency^{fire}(x), average^{intensity}(x),last^{ignition}(x))$$
Ces variables permettent de pondérer la vulnérabilité structurelle en prenant en compte l'historique passé, on obtient un indicateur de risque excellent même si assez rare. 

Chaque sous-vecteur du vecteur $\mathbf{z}(x)$ joue un rôle différent dans la sélection des DRCs, le calcul de la vulnérabilité structurelle, la propagation inter-clusters, la propagation par similarité au voisinage et l'estimation initiale du risque. 

En définitive, le vecteur $\mathbf{z}(x)$ est l'information fondatrice au calcul du risque. 

Le but est désormais de créer une carte de vulnérabilité préalablement, à partir des données disponibles pour permettre de présélectionner les candidats potentiels à prendre le statut de DRC (Dynamic Risk Cluster) dans la suite méthodologique.
### Apports de l'expertise humaine locale

La première étape consiste à intégrer l'expertise humaine, notamment : 

- SDIS (pompiers) : zones historiquement critiques, couloirs de propagation rapide, secteurs difficiles d'accès. 
- ONF (écologues) : continuité du combustible, stress hydrique chronique, vulnérabilité écologique
- Gestionnaires du site : zones fréquentes ou sensibles, infrastructures, usages humains. 

Cette expertise nous octroie la possibilité de créer une carte qualitative initiale de vulnérabilité sur quatre niveaux, nécessaire avant d'implémenter nos systèmes de monitoring : 

$$S_{expert}(x) \in \{0,1,2,3\} $$
### Données géospatiales structurelles 

Les informations expertes sont ensuites complétées par des données objectives, disponibles et accessibles, produite par des organismes institutionnels (services météo, agences environnementales, institut de cartographie) et l'expertise terrain : 

- cartes de végétations, biomasse et combustible potentiel
- modèles topographiques numériques du terrain
- réseau anthropique (routes, sentiers)
- historique des feux

Ces données offrent la possibilité d'estimer un score structurel de vulnérabilité $S_{struc}$ pour chaque cellule du territoire $\Omega$, qui est discrétisé en petite unités spatiales cellulaire, d'indice $i \in \{1,2,3,...,N\}$, construisant le maillage de $\Omega$. 

Le repère $\Omega_i$ nous permet donc de nous situer dans la carte et donc d'avoir le plan de projection de nos vecteurs de caractéristiques : l'espace est donc divisé en $\Omega_{i} \subset \Omega$ cellules spatiales polygonales dans un système d'information géographique (SIG).

Pour chaque $\Omega_i$, on peut en tirer un vecteur local $z_{i,k}$ pour une caractéristique $k \in \{ 1,2,3,...\}$ où $1 \mapsto \mathcal{density^{soil}}$ , $2 \mapsto density^{canopy}$, ...
$$S_{struc}(\Omega_i) = \sum_{k}w_k \ z_{i,k}$$ avec $z_{i,k} = z_k(x_i)$ où $z_i := z(x_i)$ et $x_i \in \Omega_i$ avec $x_i$ un centroïde qui résume l'information de la cellule $\Omega_i$. 

Il existe une infinité de points de coordonnée $\mathbf{x} = (x,y)$  dans $\Omega_i$ et $x_i$ est un point représentatif de $\Omega_i$ approximant l'essentiel de l'information de la cellule, utile pour les calculs.

 On considère $z_{i,k}$ comme la $k$-ième caractéristique vectorisée dans la cellule spatiale $\Omega_i$ et les poids $w_k$ sont calibrés selon des critères dérivés d'expertise ou d'information statistiques. 

On obtient ainsi un *score structurel de vulnérabilité* $S_{struc}$ pour chaque cellule $\Omega_i$ : ce score classe les zones selon leur propension naturelle à l'ignition ou à la propagation.

### Données climatologiques et météorologiques 

Les conditions atmosphériques influencent en grande partie l'état du combustible, une faible humidité ou une exposition régulière aux vents forts transforme un espace de biomasse, en épicentre d'ignition particulièrement dangereux. On recherche à identifier les zones structurellement vulnérables sur les plans météorologiques et climatiques, celles qui, en moyenne et sur le long terme, sont les plus exposés.

Les variables météorologiques et climatologiques utilisées sont donc principalement structurelles, construites à partir de séries historiques (moyennes, extrêmes, fréquence d'épisodes) : 

- régimes de vent dominants (direction et intensité),
- fréquence d'épisodes chauds et secs, 
- saisonnalité des sécheresses, 
- déficits hydriques récurrents, 
- climatologie des températures et de l'humidité.

On crée un indice climatique de fond, représentatif de ces informations : 

$$ C(x) = (\bar{T}(x),\bar{H}(x),\bar{W}(x),\bar{D}(x))$$

Les données météo/climat de cette phase servent uniquement à identifier des secteurs chroniquement soumis à des régimes favorables à l'assèchement et à la propagation.

### Données satellites et environnementales de site 

Les données satellite apportent une observation synoptique du territoire, permettant de confirmer que certaines zones sont durablement "stressés" ou potentiellement plus inflammables que d'autres. Ces données serviront à identifier des patterns persistants : 

- densité et vigueur de la végétation (proxy biomasse/combustible),
- stress hydrique récurrent (tendance à la dessiccation),
- température de surface moyenne plus élevée localement (hotspots thermiques),
- variations saisonnières régulières associées à la vulnérabilité.

On regroupe ces champs dans un vecteur satellite structurel : 

$$X_sat(x) = (\bar{NDVI}(x), \bar{NDWI}(x), \bar{T^{surface}}(x),...)$$
### Carte d'initialisation : carte de vulnérabilité long-terme pour sélectionner les DRCs.

Avec toutes ces données et variables latentes en main principalement centrées sur la connaissance préalable du terrain sur les plans météorologiques et climatologiques, nous avons les outils pour confirmer statistiquement et objectiver les zones pressenties par l'expertise territoriale : manque de canopée, forte exposition solaire, sécheresse chronique, végétation inflammable, corridors de vents...

Il est désormais possible de générer un espace SIG, une carte d'initialisation $V(x)$ qui modélise l'espace d'étude en terme de vulnérabilité long-terme : on peut ainsi repérer plus aisément les zones les plus susceptibles d'être des points d'ignition probables et qui peuvent favoriser une propagation importante à priori.

On combine ainsi notre expertise terrain $S_{expert}(x)$, les caractéristiques structurelles du site $S_{struct}(x)$, la climatologie et les régimes de vents $C(x)$ et les observation satellite structurelle $X_{sat}(x)$.

$$V(x) = F(S_{expert}, S_{struct}(x), C(x), X_{sat}(x))$$
On obtient ainsi une variable $V(x)$ de vulnérabilité structurelle (hotspot potentiel) qui nous servira de brique élémentaire pour construire notre carte d'initialisation, et donc d'avoir un premier cadre pour identifier les hotspots candidats et sélectionner les DRCs.

**La sélection des hotspots candidats à être des DRCs**

On définit un ensemble de candidats sur la base d'un seuil ou d'un quantile élevé : 

$$\mathcal{I}_{cand} = \{\Omega_i | V(x_i) > q_{\alpha}(V)\}$$
Cela signifie que seulement les hotspots les plus chauds seront sélectionnées pour être DRCs, d'ailleurs l'avantage de cet outil est qu'en fonction des moyens et de l'efficacité du système (qui pourrait être prouvé dans des études à posteriori) : le système est évolutif et en desserrant la contrainte vers un quantile plus faible, nous permettre d'avoir une plus vaste sélection de hotspot candidats et donc de DRCs à monitorer, renforçant ainsi la puissance intrinsèque du framework LynxSense.

Les hotspots candidats seront ensuite étudiés et validés par un comité d'experts à travers une pipeline annexe de comparaison inter-hotspots, à partir de là seront sélectionnées les Dynamic Risk Clusters, qui seront nos unités instrumentées de monitoring. 

La puissance du framework se déploie, on change donc de régime en passant d'une logique d'analyse structurelle "à distance" vers une logique de monitoring avancée "sur le terrain", en instrumentant les DRCs afin de réduire l'incertidude et de combler l'écart d'information entre la réalité du terrain et le décideur. 

## Identification, délimitation et sélection des DRCs

## Installation des capteurs IoT 

## Ingestion et prétraitement du streaming de données 

## Moteur spatio-temporel du risque (Black-box) : génération de la fonction de risque et inférences sur un network de propagation de clusters et neighboring des clusters.

## Construction de la surface de risque

## Système de seuil d'alertes

## Output final



