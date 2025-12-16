
1) Question causale 
2) Traitement principal
3) Outcomes
4) Modèle d'inférence causale 
5) Gestion des hypothèses 
6) Robustesses de la méthode
7) Interprétations

LynxSense est conçu comme un outil d'aide à la décision publique, visant à améliorer la gestion du risque incendie en renforçant la qualité du contexte informationnel dans lequel les autorités opèrent. Le système ne cherche pas à agir directement sur l'environnement, mais à fournir une **Dynamic Risk Map** accompagnée de métadonnées opérationnelles décrivant la fréquence, la couverture et la latence de l'information produite.

Dans un contexte marqué par une forte incertitude environnementale et des contraintes budgétaires et opérationnelles, la performance de l'action publique dépend moins de la quantité de décisions prises que de leur adéquation au niveau de risque effectivement observé. Dès lors, l'enjeu central n'est pas d'évaluer l'impact de LynxSense sur l'occurence des feux - un objectif difficilement identifiable - mais de mesurer si l'information fournie est effectivement intégrée dans le processus décisionnel. 

L'analyse économétrique vise ainsi à déterminer si, à niveau de risque donné, l'amélioration du contexte informationnel apportée par LynxSense permet aux autorités publiques de prendre des décisions plus proportionnées, plus réactives et mieux ciblées. 
### Question causale 

*Dans quelle mesure l'utilisation de la **Dynamic Risk Map** produite par le framework LynxSense de LynxEye améliore-t-elle l'alignement des décisions publiques avec le niveau de risque observé, en optimisant le processus décisionnel des autorités sous contrainte d'incertitude et de ressources limitées ?* 

*Le choc informationnel produit par LynxSense, sur les plans de la fréquence, de la couverture et de la latence de l'information additionnelle perçue, permet-il pour un risque environnemental donné, d'augmenter la sensibilité des autorités décisionnels aux signaux de risque ?*

LynxSense est interprété comme un choc informationnel qui modifie la fonction de décision publique sans affecter directement l'environnement physique. L'effet recherché n'est donc pas une augmentation mécanique de l'intensité décisionnelle, mais une modification systématique de la relation entre risque observé et décision prise. 

D'un point de vue empirique, l'optimisation du processus décisionnel se traduit par : 

- Une réponse plus marquée lorsque le risque est élevé
- Une limitation des décisions coûteuses lorsque le risque est faible
- Une meilleure proportionnalité globale de l'action publique

L'évaluation consiste dès lors à tester si la pente de la relation décision-risque devient plus forte lorsque le contexte informationnel s'améliore, ce qui constitue la justification économétrique centrale de l'utilité de LynxSense.


### Données mobilisées 

L'analyse économétrique repose sur un jeu de données de panel structuré au niveau territoire $i$ $\times$ période $t$. 

Les données utilisées proviennent de deux sources distinctes : 

- Les données et métadonnées du système LynxSense,
- Les données publiques de décisions administratives.

#### Les données de LynxSense : Dynamic Risk Map

La Dynamic Risk Map associe à chaque cellule $\Omega_i$ $\in \Omega$, une valeur de risque d'ignition et de propagation : 

$$R(\Omega_i,t) \in [0,1]$$

Nous déterminons le champ d'action des décideurs, sur une échelle de territoires administratifs, notés $j$, qui regroupent plusieurs cellules $\Omega_i$. 

Pour chaque territoire $j$, on définit l'ensemble des cellules qu'il recouvre : 
$$\mathcal{I}(j) = \{ \ i \ | \ \Omega_i \subset j \ \}$$
Afin de relier le signal de risque au niveau de la décision publique, on définit un risque territorial agrégé : 
$$Risk_{jt} = \mathcal{A}(\{R(\Omega_i,t) : i \in \mathcal{I}(j) \})$$ où $\mathcal{A}(*)$ est un opérateur d'agrégation fixé en amont (comme le maximum ou le quantile élevé). 

La variable $Risk_{jt}$ constitue le signal de risque effectivement observé par le décideur, elle concentre l'interprétation du risque par ces derniers.

On obtient donc une valeur de risque agrégée pour un espace d'intervention $j$ donnée et sous la direction d'une autorité locale compétente. 






### Traitement principal 

LynxSense est modélisé comme une technologie d'amélioration du contexte informationnel, le traitement économétrique correspondra ainsi à une variation exogène de la qualité de l'information disponible pour les autorités publiques. 

Plus précisément, le traitement principal est définie comme **qualité informationnelle effective** fournie par LynxSense pour un territoire donné et une date donnée. Cette qualité est capturée par des métadonnées opérationnelles, fournis par nos systèmes et décrivant les conditions de production et de diffusion d'information de la Dynamic Risk Map.

Le traitement qui sera appliqué est un traitement continu et non binaire, nous le modélisons comme **l'indice synthétique de qualité informationnelle (IQSI, Information Quality Synthetic Index)** :


