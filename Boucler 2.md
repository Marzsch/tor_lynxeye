
# 0/ Executive Summary

# I/ Context and Strategic Background

Over the past decade, **wildfire risk has undergone a profound transformation across Europe**, driven by the combined effects of **climate change, prolonged droughts, recurring heatwaves, and increasing ecosystem stress**. These structural shifts have altered fire behavior in depth, resulting in **longer fire seasons**, **higher ignition probabilities**, and **faster, less predictable propagation dynamics**, particularly across the **Mediterranean basin**.

Southern Europe—and Southern France in particular—has become a region of **systemic exposure**, where wildfire risk can no longer be understood as a series of isolated seasonal events. The 2022 wildfire season in France, during which more than **60,000 hectares burned**, illustrated how rapidly extreme climatic conditions can overwhelm existing prevention and response mechanisms, even in territories historically considered moderately exposed. This episode marked a turning point, revealing that wildfire risk has evolved into a **structural constraint on territorial governance**.

This transformation is not solely climatic in nature. It is amplified by **land-use patterns**, **vegetation continuity**, and **growing human pressure** at the wildland–urban interface. As a result, wildfire risk increasingly emerges from the interaction between environmental stressors and human activity, producing **highly localized, heterogeneous, and rapidly evolving risk conditions** that challenge traditional monitoring paradigms.

In parallel, wildfire governance has benefited from significant institutional and technological advances. At both national and European levels, major frameworks have been deployed to strengthen monitoring, prevention, and civil protection capacities. In France, these include the **Plan National d’Adaptation au Changement Climatique (PNACC 2)** and the **National Strategy for Forest and Vegetation Fire Risk Management (2023–2030)**. At the European level, mechanisms such as the **EU Civil Protection Mechanism (UCPM)**, **RescEU**, the **European Forest Fire Information System (EFFIS)**, and the **Copernicus Emergency Management Service (EMS)** have substantially improved satellite observation, meteorological modelling, and cross-border coordination.

Despite this dense institutional architecture and the growing availability of macro-scale environmental data, public authorities continue to face **persistent blind spots** in their ability to anticipate and manage wildfire risk. Existing systems remain primarily oriented toward **periodic, large-scale observation**, offering limited capacity to capture **fine-scale environmental variations**, **intra-day risk dynamics**, and **localized ignition conditions** that are critical for early decision-making.

This gap is particularly problematic in territories characterized by strong spatial heterogeneity, where ignition probability and propagation potential can vary sharply over short distances and time intervals. Public authorities are therefore required to make decisions under conditions of **high uncertainty**, while relying on information systems that were not designed to support **continuous, localized, and decision-relevant risk assessment**.

The result is a growing mismatch between the **temporal and spatial dynamics of wildfire risk** and the **informational context in which public decisions are taken**. This mismatch constrains the ability of institutions to move beyond reactive response and toward **proactive, anticipatory wildfire governance**, even when political will, operational capacity, and institutional coordination are present.

It is within this context that the **LynxSense framework** has been conceived. Rather than replacing existing national and European infrastructures, LynxSense is designed as a **complementary, AI-enabled information system**, capable of delivering **continuous, multi-source, high-resolution environmental intelligence** at the local level. By strengthening the informational foundations of public action, the framework aims to support more timely, better targeted, and more proportionate wildfire risk management across high-exposure Mediterranean territories.


# II/ Problem Statement: Wildfire Risk Governance and Decision-Making Challenges

### 1) Wildfire Risk as a Decision Problem Under Uncertainty

Within the strategic context described above, wildfire risk governance emerges primarily as a **decision-making problem under uncertainty**. Public authorities are not only confronted with a higher frequency of extreme events, but with the need to make **time-sensitive decisions**—related to prevention, preparedness, and resource allocation—under rapidly changing and partially observed conditions.

At this stage, the challenge is no longer to recognize the existence of wildfire risk, but to determine **how public action should be adjusted in real time** as risk levels evolve. Decisions must be taken under binding operational and budgetary constraints, often before risk fully materializes, and with limited margins for correction once interventions are deployed. In this setting, the effectiveness of public action depends critically on its **timing, spatial targeting, and proportionality** relative to underlying risk dynamics.

Wildfire governance is therefore less a question of intervention capacity than of **decision quality conditioned by information availability**. When risk signals are delayed, aggregated, or weakly connected to operational choices, even well-coordinated institutions face systematic difficulties in aligning action with evolving risk conditions.

### 2) Decision Constraints and Information Asymmetries

In practice, public decision-making is shaped by a set of **structural constraints** that interact directly with the informational environment. Preventive and preparatory measures—such as patrol deployment, surveillance missions, or resource pre-positioning—must often be planned in advance, based on forecasts or indicators that may lose relevance within hours.

At the same time, wildfire risk evolves at a much higher temporal frequency. Short-term changes in weather conditions, vegetation stress, or human activity can generate abrupt shifts in ignition probability and propagation potential. This creates a persistent **asymmetry between the speed of risk dynamics and the pace at which decisions can be revised**, particularly when information updates are infrequent or spatially coarse.

These constraints are further amplified by the need to coordinate decisions across multiple administrative levels and operational actors. As a result, public authorities operate in a decision environment where **information is structurally incomplete at the moment when it is most needed**, limiting the capacity to adjust actions dynamically as conditions evolve.


### 3) Limits of Existing Decision-Support Systems

Although existing monitoring and prevention systems provide valuable situational awareness, they remain **weakly aligned with the needs of operational decision-making**. Most systems have been designed to support regional-scale monitoring, post-event assessment, or strategic planning, rather than continuous, fine-grained decision support.

Information is typically delivered through aggregated indicators, periodic updates, and separate data streams. Local environmental signals, short-term anomalies, and micro-scale risk variations are rarely integrated into a unified operational picture that can be directly mobilized for decision-making. As a consequence, available information often lacks **decision salience** at the spatial and temporal scales at which preventive action must be taken.

This structural limitation does not prevent action, but it **distorts it**: decisions are taken with partial visibility, forcing authorities to rely on precautionary heuristics or reactive adjustments rather than on continuous risk-informed guidance.

### 4) Implications for Wildfire Risk Governance

The interaction between rapid risk dynamics, constrained decision processes, and limited decision-relevant information produces a governance model that remains **predominantly reactive**, even in the presence of strong institutional frameworks and growing technical capacity.

Preventive actions may be initiated too late, insufficiently targeted, or weakly correlated with localized risk conditions. Conversely, resources may be over-mobilized to compensate for uncertainty, generating inefficiencies and opportunity costs elsewhere in the system. These outcomes reflect not a lack of commitment or coordination, but a **structural misalignment between how wildfire risk evolves and how decisions are informed**.

Improving wildfire risk governance therefore requires more than incremental improvements in monitoring or response capacity. It calls for an intervention that directly addresses the **informational foundations of public decision-making**, by reducing uncertainty at the moment decisions are taken and by improving the alignment between observed risk and public action.

It is this specific governance challenge—emerging from the context described in Section I—that motivates the intervention presented in the following section.


# III. Overview of the Proposed Solution: The LynxSense Framework

### 1. Project vision and value proposition  

The LynxSense framework is conceived as a **decision-support system** designed to address the governance challenges identified in the previous section. Its primary objective is not to intervene directly on wildfire events, but to **improve the informational environment** in which public authorities assess risk and make preventive and preparatory decisions.

LynxSense is built on the premise that wildfire risk governance can be significantly strengthened by providing **continuous, localized, and decision-relevant environmental intelligence**. By reducing informational uncertainty at the moment decisions are taken, the framework aims to improve the **timeliness, targeting, and proportionality** of public action under constrained operational and budgetary conditions.

The value proposition of LynxSense therefore lies in its capacity to transform heterogeneous environmental observations into **actionable risk signals**, enabling public authorities to move from predominantly reactive approaches toward more anticipatory and risk-informed governance practices.

### 2. System overview and functional architecture  

LynxSense is designed as an **integrated, modular system** combining data acquisition, analytical processing, and decision-support functionalities within a unified framework. The system operates continuously, ingesting information from multiple sources and updating risk assessments as new data become available.

At a high level, the framework is structured around three functional layers :

- a **data acquisition layer**, responsible for collecting heterogeneous environmental observations;  
- an **analytical and inference layer**, where data are processed, integrated, and translated into risk assessments;
- a **decision-support layer**, providing public authorities with dynamic risk representations and operational insights.

This layered architecture ensures scalability, adaptability, and interoperability with existing national and European monitoring and civil protection infrastructures, while maintaining a clear focus on decision relevance.

### 3. Multi-source data acquisition strategy  

The LynxSense framework relies on a **multi-source data acquisition strategy** to capture the complexity and heterogeneity of wildfire risk dynamics. Data inputs include ground-based environmental sensors, autonomous aerial platforms, satellite imagery, and meteorological forecasts.

Each data source contributes complementary information at different spatial and temporal resolutions. Ground sensors provide localized, high-frequency measurements of environmental conditions; aerial platforms enable targeted observation of high-risk zones; satellite imagery offers broad territorial coverage; and meteorological data support short-term risk anticipation.

By combining these heterogeneous sources, LynxSense aims to overcome the limitations of single-source monitoring systems and to ensure **robust coverage of localized and rapidly evolving risk conditions**.

### 4. Integrated intelligence layer and decision support  

At the core of the LynxSense framework lies an **integrated intelligence layer** responsible for transforming raw environmental data into decision-relevant risk information. This layer continuously fuses incoming observations, updates risk assessments, and generates dynamic representations of wildfire risk across the monitored territory.

The primary output of this process is a **Dynamic Risk Map**, which provides public authorities with a continuously updated view of ignition and propagation risk at a fine spatial scale. This representation is designed to support operational decision-making by highlighting priority areas, emerging risk patterns, and short-term risk escalation.

By delivering **timely, localized, and interpretable risk information**, the decision-support layer enables public authorities to better align preventive and preparatory actions with observed risk dynamics, addressing the governance challenges outlined in Section II.

# IV. Methodological Framework
*(Technical Core provided in Annex)*

The LynxSense Framework is built upon a **continuous, adaptive, and multi-layer analytical methodology** designed to monitor wildfire risk in real time.  
Rather than operating through periodic assessments or static danger maps, the system functions as a **living analytical ecosystem**, recalibrating its risk indicators each time new environmental data become available.

The methodological architecture relies on three core components:

-  **Dynamic Risk Clusters (DRCs)** — an adaptive, data-driven sampling strategy identifying the most ignition-prone and propagation-sensitive units within a territory.
-  **A real-time analytical pipeline** — responsible for ingesting, structuring, integrating, and enriching heterogeneous data streams from IoT sensors, drones, satellite imagery, and meteorological services.
- **Propagation and spatial inference models** — providing advanced fire-spread simulations, inter-cluster risk diffusion, and probabilistic inference to anticipate fire behavior under changing environmental conditions.

Together, these components allow LynxSense to produce **high-resolution, continuously updated wildfire intelligence**, linking micro-scale environmental observations to broader regional and climatic dynamics.  
The following subsections detail each component of this methodological framework.


#### Dynamic Risk Clusters (DRCs)

At the core of the LynxSense methodology is the concept of **Dynamic Risk Clusters (DRCs)** — localized environmental units designed to reflect wildfire ignition potential, vegetation stress, and propagation sensitivity.  
They form the backbone of the system’s sampling strategy, enabling LynxSense to focus monitoring efforts where they yield the highest predictive value.

##### **1) Identification and Characterization of High-Risk Zones**

Instead of attempting to monitor vast territories exhaustively, LynxSense identifies **high-impact clusters** through a multi-criteria assessment combining:

- vegetation and biomass density,
- topography, slope orientation, and terrain complexity,
- historical fire occurrence,
- human activity patterns (tourism, agriculture, transport),
- and meteorological and climatic variables (humidity, temperature, wind exposure).

This process isolates zones that are **intrinsically more susceptible to ignition** and where environmental stress evolves most rapidly.

##### **2) DRCs as Adaptive Environmental Units**

Each DRC acts as a **living data unit** whose internal parameters—dryness indices, microclimatic variables, vegetation stress markers—are **continuously updated** as new data are ingested.

A DRC also functions as a **representative sampling node**, capturing fine-scale environmental dynamics that can be extrapolated to surrounding areas through spatial inference.

##### **3) DRC Deployment Process**

A reconnaissance process, assisted by local specialists and historical environmental datasets, determines the initial DRC configuration.  
Selected clusters receive the monitoring infrastructure:

- IoT environmental sensors,
- autonomous drone stations with solar-powered charging,
- localized micro-weather probes.

##### **4) Advantages of the DRC Methodology**

This adaptive sampling strategy yields:

- **Higher precision** → risk indicators updated continuously.
- **Lower latency** → rapid detection of changing conditions.
- **Better scalability** → reduced need for exhaustive instrumentation.

In essence, DRCs provide a **high-density, high-relevance environmental signal**, enabling early detection of ignition conditions and fine-scale understanding of fire dynamics.

#### Analytical Pipeline

The analytical pipeline is the **central processing engine** of the LynxSense Framework.  
It transforms raw, heterogeneous environmental observations into structured, actionable intelligence through a continuous sequence of operations.

##### 1) Multi-Source Data Ingestion

The pipeline ingests four primary classes of data:

- **IoT sensors** (humidity, soil temperature, microclimate indicators)
- **Satellite imagery** (Copernicus Sentinel, MODIS, EFFIS vegetation indices)
- **Meteorological feeds** (Météo-France, ECMWF, atmospheric models)
- **Autonomous drones** (RGB imagery, thermal data, canopy stress indicators) (optional)

These sources vary widely in **scale**, **frequency**, and **data formats**, requiring a robust ingestion architecture.

##### 2) Preprocessing and Data Structuring

To ensure coherence across sources, the system applies:

- **spatio-temporal alignment**,
- **data normalization**,
- **feature extraction** for vegetation and dryness indices,
- **noise reduction**.

These steps transform raw data into harmonized, analysis-ready environmental variables.

##### 3) Real-Time Data Fusion

LynxSense uses advanced fusion techniques to integrate heterogeneous inputs, including:

- **Kalman filters** for continuous state estimation despite missing or noisy data,
- **kriging and geostatistical interpolation** to fill spatial gaps,
- **anomaly detection algorithms** to identify sensor drift or faulty readings,
- a **hybrid edge–cloud architecture** ensuring resilience even under limited connectivity.

This real-time fusion allows the system to recompute risk metrics and environmental indicators at each update cycle.

##### 4) Continuous Risk Recalibration

As new data arrive, the LynxSense engine automatically recalibrates :

- DRC dryness indices,
- fuel stress variables,
- microclimate conditions,
- inferred risk scores,
- and inter-cluster relationships.

This mechanism—supported by **incremental learning algorithms**—ensures that risk assessment remains synchronized with evolving environmental conditions.


#### Propagation and Spatial Inference Models

Wildfire behavior is inherently **spatial and interconnected**. A change occurring in one cluster can influence adjacent zones within minutes.  
To capture this complexity, LynxSense models the monitored area as a **graph network**, where:

- each **node** represents a DRC, and
- each **edge** represents a **weighted propagation pathway**.

##### 1) Propagation Pathway Modeling

Propagation weights are computed based on:

- wind alignment and speed,
- topographic gradients and slope-driven acceleration,
- vegetation and fuel continuity,
- dryness differentials.

These factors determine how risk can diffuse from one cluster to another.

##### 2) Fire Behavior Simulation and Inference

The system uses a combination of:

- **graph-based diffusion models** to simulate short-term fire spread,
- **Markov Random Fields** to infer unobserved risk states in poorly instrumented regions,
- **Graph Neural Networks (GNNs)** to learn complex spatial interactions between environmental variables,
- hybrid approaches combining physics-inspired models (cellular automata) with data-driven methods.

##### 3) Regional Risk Extrapolation

Using these models, LynxSense extrapolates the likely evolution of risk beyond the directly observed clusters, creating a **coherent, landscape-scale risk picture**.

This enables authorities to anticipate:

- where fire could spread next,
- how fast it could propagate,
- which clusters act as “risk bridges”,
- and where to prioritize surveillance or resource deployment.

#### Feasibility assessment 

##### Technological feasibility

The technologies mobilized by the LynxSense Framework—IoT environmental sensors, autonomous drones, satellite imagery, and real-time data processing—are **mature, commercially available, and field-tested** in various environmental monitoring contexts.  
The system relies on **proven hardware**, **standard communication protocols**, and a **scalable cloud-edge architecture**, ensuring robust deployment even in remote or connectivity-limited areas.

**Conclusion:** All technological components required for LynxSense exist, are interoperable, and can be deployed at scale.

##### Operational feasibility 

LynxSense builds on existing operational infrastructures (SDIS, ONF, regional crisis cells) and integrates seamlessly with national and European procedures.  
Deployment relies on:

- pre-identified DRCs,
- lightweight sensor installation,
- autonomous drone stations,
- and standardized operational workflows.

Local teams require **minimal additional workload**, as the system functions autonomously once installed, with periodic maintenance.

**Conclusion:** Operational integration is straightforward, and field deployment is compatible with existing institutional capacities.

##### Data feasibility

All required data streams—IoT measurements, drone imagery, Copernicus products, EFFIS feeds, meteorological forecasts—are **accessible, standardized, and legally usable** within the framework of environmental monitoring.  
The LynxSense pipeline is designed to ingest heterogeneous data formats and comply with **INSPIRE** and **ISO 19115** standards for geospatial information.

**Conclusion:** Data availability, accessibility, and regulatory compliance pose no barriers to implementation.

##### Economic feasibility 

The economic model of LynxSense prioritizes:

- targeted instrumentation limited to selected DRCs,
- autonomous operations reducing labor costs,
- cloud-based scalability,
- and reduction of high-impact wildfire losses through earlier detection and improved decision-making.

Compared to exhaustive monitoring approaches, the DRC strategy significantly lowers deployment and operational expenditures while maximizing predictive value.

**Conclusion:** The solution is economically viable, cost-efficient, and designed to generate measurable savings through avoided damages and optimized resource allocation.


*(Detailed technical specifications provided in Annex A)*


# V. Econometric Evaluation Framework


The LynxSense framework is conceived as a **public decision-support system**, aimed at improving wildfire risk governance by strengthening the **informational environment** in which public authorities operate. The system does not seek to act directly on the physical environment, nor to prevent wildfire occurrence mechanically, but to provide decision-makers with a **Dynamic Risk Map**, accompanied by operational metadata describing the **coverage**, **latency**, and overall quality of the information delivered.

In a context characterized by high environmental uncertainty and binding budgetary and operational constraints, the performance of public action depends less on the quantity of decisions taken than on their **alignment with the level of risk effectively observed**. From an empirical perspective, this implies that the relevant object of evaluation is not the impact of LynxSense on wildfire occurrence—an outcome that is both indirect and difficult to identify—but rather whether the information provided by the system is **effectively integrated into the public decision-making process**.

The econometric evaluation therefore focuses on assessing whether, conditional on a given level of environmental risk, improvements in the informational context delivered by LynxSense lead public authorities to take **more proportionate, more reactive, and better targeted decisions**. In other words, the analysis seeks to determine whether LynxSense improves **decision quality under uncertainty**, rather than increasing decision intensity per se.

The central causal question guiding the econometric analysis is the following:

*To what extent does the use of the Dynamic Risk Map produced by the LynxSense framework improve the alignment of public decisions with the observed level of wildfire risk, by enhancing the sensitivity of public authorities to risk signals under conditions of uncertainty and limited resources?*

Equivalently, the analysis asks whether the **informational shock** generated by LynxSense—through improvements in information coverage and latency—modifies the public decision function by increasing the responsiveness of authorities to environmental risk signals, for a given level of underlying risk.

LynxSense is thus interpreted as an **exogenous informational shock** that affects how decisions are made, without directly affecting the physical environment. The expected effect is not a mechanical increase in public action, but a **systematic change in the relationship between observed risk and decisions taken**.

From an empirical standpoint, an improvement in the decision-making process should manifest itself through :

- a stronger response when risk levels are high,
- a limitation of costly decisions when risk levels are low,
- and an overall improvement in the proportionality of public action.

Econometrically, this translates into testing whether the **slope of the decision–risk relationship** becomes steeper as the informational environment improves.

### 1) Data structure and territorial risk signal 

The econometric analysis relies on a **panel dataset** structured at the level of decision-making territory $j$ over time $t$.

Two main data sources are mobilized :

- operational data and metadata generated by the LynxSense system,
- publicly available data on administrative decisions related to wildfire prevention and preparedness.

#### Territorial Risk Signal from the Dynamic Risk Map

The LynxSense Dynamic Risk Map associates to each spatial cell  $\Omega_i$ $\in \Omega$  a continuous measure of ignition and propagation risk :

$$R(\Omega_i,t) \in [0,1]$$

Public decisions, however, are taken at the level of administrative territories, indexed by $j$, each covering a set of spatial cells. Let :

$$\mathcal{I}(j) = \{ \ i \ | \ \Omega_i \subset j \ \}$$

denote the set of cells belonging to territory $j$.

To link the risk signal to the level at which decisions are made, a **territorially aggregated risk measure** is defined as :

$$Risk_{jt} = \mathcal{A}(\{R(\Omega_i,t) : i \in \mathcal{I}(j) \})$$

where $\mathcal{A}(*)$ is a pre-specified aggregation operator (e.g. maximum risk, high quantile).

The variable $Risk_{jt}$ ​ represents the **effective risk signal perceived by the decision-maker**, and constitutes the core explanatory variable capturing the environmental constraint faced by public authorities.

### 2) Treatment Definition: Information Quality

LynxSense is modeled as a technology that improves the **quality of the informational context** available to public authorities. Accordingly, the econometric treatment corresponds to an exogenous variation in information quality at the territory–time level.

**Information Quality Synthetic Index (IQSI)**

The treatment is defined as a **continuous measure** of information quality, captured through an **Information Quality Synthetic Index (IQSI)**, bounded between 0 and 1.

For each territory $j$ and period $t$, the IQSI measures the effective quality of the risk signal made available to the decision-maker, based on operational metadata generated by the LynxSense platform.

The index relies on two non-redundant and directly observable dimensions :

- $C_{j,t}$ (**effective spatial coverage**): the share of territory $j$ for which a valid risk value $R(\Omega_i,t)$ is available. This component captures the degree of **spatial completeness** of the information transmitted to the decision-maker.
- $L_{j,t}$ (**information timeliness – latency**): the average latency of risk signal dissemination, defined as the time elapsed between data acquisition by the LynxSense system and the effective availability of the information to the decision-maker through the Dynamic Risk Map.

In order to preserve a **monotonically increasing interpretation** of the index, a timeliness measure is defined as:

$$T_{j,t} = 1 - L_{j,t}^{normalized}$$
with $w_C + w_T = 1$.

The weights $(w_C, w_T)$ are fixed ex ante in the analysis to reflect the operational trade-off between spatial completeness and signal timeliness.

As a baseline specification, balanced weights $(0.5, 0.5)$ are adopted, reflecting a neutral weighting scheme.

The relevance of these weights can be discussed and is addressed through **robustness checks**, aimed at assessing the stability of the econometric results under alternative weighting schemes.

Robustness is tested by re-estimating the model using alternative weight configurations favoring timeliness $(0.4, 0.6)$ or spatial coverage $(0.6, 0.4)$, as well as under extreme scenarios prioritizing immediate crisis response or long-term territorial prevention.

A high value of $IQSI_{j,t}$ corresponds to a **high-quality informational environment**, in which the decision-maker benefits from :

- a **spatially complete risk signal**, covering a large share of the decision-maker’s intervention territory, thereby limiting informational blind spots and strengthening the coherence between available operational capacities and perceived risk;

- a **temporally relevant risk signal**, disseminated with low latency, such that the time gap between data acquisition by the system and access to interpretable information by the decision-maker is minimized.

Within this framework, the effective frequency of risk signal updates is not treated as an autonomous dimension, but rather as a **direct consequence of low latency** in the information production and dissemination process.

### 3) Decision-making outcomes  

The objective is to analyze how improvements in information quality affect the decision-making behavior of public authorities, in particular by influencing their **responsiveness** and **resource allocation**, which constitute the main channels through which better information may enhance the effectiveness of public action.

**Decision responsiveness**

The first outcome variable measures the **responsiveness of public decision-makers** to a given risk signal.

For each territory $j$ and period $t$, we define the response delay (in hours or days):

$$Delay_{j,t}$$

This variable corresponds to the time elapsed between the effective availability of a relevant risk signal $Risk_{j,t}$ through the Dynamic Risk Map and the implementation of a first observable public action related to prevention or preparedness.

This delay provides a direct measure of the ability of public authorities to rapidly translate available information into operational decisions. A decrease in $Delay_{j,t}$ therefore reflects an improvement in decision responsiveness.

When a continuous measure of the delay is not available, an alternative binary variable can be used, indicating whether an action is undertaken within a given time window (for instance on the same day or within 24 hours following the observation of the risk signal).

**Resource allocation**

The second outcome variable aims to capture the **intensity of operational effort** mobilized by public authorities in response to the risk signal.

We define the variable:

$$Effort_{j,t}$$

which measures, for each territory and period, the level of resources engaged for prevention or preparedness purposes. This variable can be proxied by observable operational indicators, such as:

- the number or duration of surveillance patrols;
- the number of reconnaissance or aerial monitoring missions;
- the volume of preventive actions triggered;

or any equivalent measure reflecting the deployment of public resources.

This variable allows us to assess not only whether authorities act more intensively, but, more importantly, whether they **adjust the intensity of their action to the observed level of risk**, conditional on the quality of the information available.

In this framework, improvements in information quality provided by LynxSense are not expected to mechanically increase public action, but rather to **improve its targeting and timeliness**. Higher-quality information should translate into faster decisions when risk is high, and into a more proportionate mobilization of resources in response to variations in territorial risk.


### 4) Econometric model and identification strategy  

The objective of the econometric model is to identify to what extent improvements in information quality provided by LynxSense, measured by $IQSI_{j,t}$, modify the way public authorities translate a risk signal $Risk_{j,t}$ into an operational decision.

The goal is therefore not to estimate an average “level effect” of information on public action, but a **conditional effect**: improved information is expected to strengthen the alignment of decisions with the observed level of risk.

For each territory $j$ and period $t$, we estimate a fixed-effects panel model of the following form :

$$Outcome_{j,t} = \alpha + \beta_1 Risk_{j,t} + \beta_2(Risk_{j,t}\times IQSI_{j,t} ) + \beta_3IQSI_{j,t} + \mu_j + \sigma_t + \epsilon_{j,t}$$

where:

- $Outcome_{j,t}$ alternatively denotes decision responsiveness $Delay_{j,t}$ or operational effort intensity $Effort_{j,t}$;
- $Risk_{j,t}$ is the aggregated territorial risk signal derived from the Dynamic Risk Map;
- $IQSI_{j,t}$ measures the quality of the information signal made available to the decision-maker (spatial coverage and timeliness);
- $\mu_j$ captures **territorial fixed effects**, controlling for unobserved and time-invariant characteristics specific to each territory (local organization, topography, structural vulnerability, etc.);
- $\delta_t$ denotes **time fixed effects**, controlling for common shocks and seasonality (high-risk periods, general conditions, regulatory changes, etc.);
- $\epsilon_{j,t}$ is the error term.

The coefficient $\beta_2$ is the **central parameter** of the analysis. It measures the extent to which information quality increases the **sensitivity of public decisions to the observed level of risk**. Formally, the marginal sensitivity of the decision to risk is given by:

$$\frac{\partial Outcome_{j,t}}{\partial Risk_{j,t}} = \beta_1 + \beta_2IQSI_{j,t}$$When $IQSI_{j,t}$ is high, a non-zero value of $\beta_2$ indicates that the decision-maker’s response to risk becomes more pronounced.

- When $Outcome_{j,t} = Delay_{j,t}$, a negative value of $\beta_2$ is expected: for a given level of risk, higher information quality is associated with a **reduction in response delay** as risk increases.

- When $Outcome_{j,t} = Effort_{j,t}$, a positive value of $\beta_2$ is expected: for a given level of risk, higher information quality is associated with a **more intense and better targeted mobilization of resources** as risk increases.

This framework allows LynxSense to be evaluated as an **informational amplifier**: the system does not mechanically increase public action, but improves the ability of public authorities to adjust their decisions to the observed level of risk, which is consistent with a decision-making process under uncertainty and binding resource constraints.


### 5) Assumptions, robustness, and interpretation  






# VI. Implementation Strategy, Timeline, and Teams

# VII. Budget

