Taille maximum : 55 000 caractères (espaces inclus)
Présentation orale le 21/01 et rendu du ToR finalisé le 11/01 et du slide correspondant le 16/01
# Plan 

## I/ Introduction

1) Purpose of the ToR
2) Background
3) Institutional Framework
4) Strategic Rationale (introducing the problem)
## II/ Problem statement

1) Operational challenges
2) Limitations of current monitoring and prevention systems
3) Consequences for wildfire management and decision-making

## III/ Proposed Solution : LynxSense Framework

1) Value proposition (Why LynxEye does exists and why LynxSense is a solution)
2) System Overview
3) Unique Data Acquisition Strategy 
4) Multi-Source Intelligence Layer 
## IV/ Methodology, feasibility and evaluation

1) Methodological framework (technical core)

	1) Dynamic Risk Clusters (DRCs)
	2) Analytical Pipeline
	3) Propagation and Spatial Risk Inference Models

2) Feasibility assessment 

	1) Technological feasibility 
	2) Operational feasibility
	3) Data feasibility
	4) Economic feasibility

3) Monitoring and Evaluation : 

	1) Monitoring framework (KPIs)
	2) Econometric impact evaluation


## V/ Implementation and resources

1) Scope of Work
2) Deployment phases and timeline
3) Deliverables
4) Governance and data management
5) Human resources and capacity buildings 

## VI/ Budget and economic rationale

1) Budget structures
2) Economic rationale and ROI


## I/ Introduction
---
#### Purpose of the ToR


This Terms of Reference (ToR) defines the **strategic, technical, and operational framework** for the design and implementation of the **LynxSense Framework**, an integrated, AI-enabled system for **wildfire monitoring, anticipation, and decision support**.

It outlines the project’s **objectives, scope of work, methodological approach, implementation modalities, governance structure, and expected deliverables**. The ToR serves as a **shared reference document** establishing the responsibilities, coordination mechanisms, and performance expectations of all stakeholders involved.

Prepared in the context of a collaboration between **LynxEye**, French national authorities, regional institutions, and European civil protection partners, this document aims to guide the deployment of a **multi-source, real-time wildfire risk intelligence capability** across high-risk Mediterranean territories, with a primary focus on **Southern France**.

The purpose of this ToR is therefore to ensure a **clear, coherent, and transparent foundation** for planning, executing, and evaluating the LynxSense initiative, from early design phases to operational rollout and long-term sustainability.

#### Background 

Over the last decade, **Europe has experienced a marked intensification of wildfire activity**, driven by **climate change, prolonged droughts, recurring heatwaves, and increasing ecosystem stress**.  
These environmental shifts have fundamentally altered fire behavior, leading to **longer fire seasons**, **faster propagation dynamics**, and growing exposure across the **Mediterranean basin**, particularly in **Southern France, Spain, Portugal, Italy, and Greece**.

In France, the 2022 wildfire season — during which more than **60,000 hectares burned** — revealed how quickly extreme conditions can overwhelm existing monitoring and response mechanisms, even in territories historically considered low-risk. This event underscored the limits of current approaches in anticipating ignition conditions and managing large-scale fire dynamics.

At the European scale, efforts to strengthen wildfire monitoring and civil protection capacities have expanded through major strategic initiatives, including:

- the **Plan National d’Adaptation au Changement Climatique (PNACC 2)**,
- the **National Strategy for Forest and Vegetation Fire Risk Management (2023–2030)**,
- the **EU Civil Protection Mechanism (UCPM)** and **RescEU**,
- the **European Forest Fire Information System (EFFIS)**,
- the **Copernicus Emergency Management Service (EMS)**,
- and **Horizon Europe’s climate resilience agenda**.


Despite these strong institutional frameworks and significant improvements in **satellite observation**, **meteorological modeling**, and **civil protection coordination**, authorities still lack a **continuous, multi-source, real-time system** capable of integrating **local environmental conditions**, **high-frequency observation**, and **dynamic short-term risk evolution**.

This structural gap limits the ability of public institutions to:

- **anticipate localized ignition conditions**,
- **adapt rapidly to changing micro-environments**, and
- **transition from reactive response to proactive, data-driven wildfire governance**.

The **LynxSense framework** is conceived precisely within this context. It aims to provide a unified, AI-driven, multi-scale capability delivering **continuous, localized environmental intelligence** to support French and European authorities in strengthening wildfire anticipation, prevention, and strategic decision-making.

#### Institutional framework 

Wildfire monitoring and prevention in France and across the European Union operate within a **multi-level governance architecture**, combining national responsibilities, regional coordination, and European support mechanisms.

At the **national level**, the main actors involved in wildfire risk management include:

- the **Ministère de la Transition Écologique et de la Cohésion des Territoires**, responsible for environmental policies, climate adaptation, and ecosystem management;

- the **Direction Générale de la Sécurité Civile et de la Gestion des Crises (DGSCGC)** under the **Ministère de l’Intérieur**, which oversees civil protection operations, early response coordination, and emergency preparedness;

- the **Office National des Forêts (ONF)**, in charge of forest management and ecological supervision;

- and the **Services Départementaux d’Incendie et de Secours (SDIS)**, responsible for firefighting operations and local crisis response.


At the **regional level**, the territories of **PACA**, **Occitanie**, and **Nouvelle-Aquitaine**—identified as the most exposed to recurring wildfire activity—operate their own risk prevention, forest management, and civil protection structures. These regions coordinate local action, deploy prevention measures, and ensure operational continuity during the fire season.

At the **European level**, several major frameworks support Member States in monitoring and managing wildfire risks:

- the **EU Civil Protection Mechanism (UCPM)** and **RescEU**, which enhance emergency preparedness and cross-border response capacities;

- the **European Forest Fire Information System (EFFIS)**, providing harmonized fire danger indices, monitoring dashboards, and impact assessments;

- and the **Copernicus Emergency Management Service (EMS)**, delivering satellite-based observation and scenario modelling to support prevention and crisis management.


Together, these institutional layers form a **coherent but fragmented operational environment**, where large-scale observation tools coexist with localized response structures.  
This governance landscape underscores the need for a **new generation of monitoring capabilities** that can seamlessly integrate into existing national and European frameworks while delivering **real-time, high-resolution environmental intelligence** at the local level.
#### Rationale : Why a New Monitoring System is needed ? 

Climate change has accelerated wildfire dynamics beyond the capacity of traditional monitoring tools. While national and European systems—such as **Météo-France forecasts**, **Copernicus satellite imaging**, and **EFFIS fire danger indices**—provide essential macro-scale information, they remain **insufficient for capturing the fine-scale, rapidly evolving conditions** that drive wildfire ignition and early-stage propagation.

Current systems face structural constraints: they offer **limited spatial granularity**, rely on **periodic data updates**, and operate mainly through **reactive mechanisms**. As a result, public authorities lack the ability to:

- detect **micro-environmental variations** that precede ignition,
- monitor **risk evolution continuously throughout the day**,
- integrate **heterogeneous data sources** into a unified operational picture,
- anticipate **short-term propagation dynamics** at the local scale.


To address these gaps, a new generation of monitoring capabilities is needed to complement existing national and European infrastructures with **continuous, localized, and data-rich environmental intelligence**. Such a system must combine real-time observations from **ground sensors**, **autonomous drones**, **satellite imagery**, and **meteorological forecasts**, enabling authorities to shift from **reactive response** to **proactive, anticipatory wildfire risk governance**.

The **LynxSense framework** has been conceived precisely to meet this strategic need. By providing a **multi-source, AI-enabled monitoring and analytical capability**, LynxSense supports both **operational decision-making** and **long-term wildfire risk planning**, strengthening national and regional resilience in high-risk Mediterranean territories.

---





## II/ Problem statement
---
#### Operational challenges 

Public authorities responsible for wildfire prevention and response face a number of **operational challenges** that significantly limit their ability to anticipate and mitigate fire risks under rapidly evolving environmental conditions.

First, **monitoring vast forested and mixed-vegetation territories** on a continuous basis remains extremely difficult. Fire-prone areas in Southern France extend across thousands of square kilometers, making it impossible for on-the-ground teams to detect early warning signs or subtle environmental shifts at the right time and at the right spatial resolution.

Second, authorities lack **real-time visibility on micro-environmental dynamics**—such as local humidity drops, vegetation stress, soil temperature changes, and emerging thermal anomalies—that often precede ignition events. These signals evolve rapidly at very small scales and cannot be captured through conventional surveillance means.

Third, **intra-day risk fluctuations** driven by shifting wind conditions, sudden temperature peaks, or local human activity (agricultural work, tourism, transportation corridors) are difficult to monitor and interpret. Fire risk can escalate dramatically within a few hours, but current structures do not allow authorities to track these evolutions continuously.

Fourth, **local human pressure**—including the presence of residents, tourists, road traffic or recreational activities—adds an additional layer of complexity. Regions such as PACA and Occitanie combine high vegetation density with dense seasonal population movement, making ignition conditions more sensitive and more difficult to anticipate.

Finally, **resource prioritization and early response positioning** remain challenging due to limited situational awareness. Without precise, continuously updated information, authorities struggle to determine where to reinforce surveillance, how to pre-position firefighting assets, and when to escalate preparedness levels.

Together, these challenges create a **structural lack of operational intelligence**, increasing uncertainty and reducing the capacity of public institutions to act preventively before fires escalate into critical events.

#### Limitations of current monitoring and prevention systems

Despite significant progress in national and European wildfire management capabilities, **current monitoring and prevention systems remain constrained by structural and technological limitations** that prevent authorities from anticipating ignition conditions and short-term propagation risks with sufficient precision.

**First**, existing systems provide primarily **macro-scale and periodic information**.  
Meteorological forecasts from **Météo-France**, fire danger indices from **EFFIS**, and satellite imagery from **Copernicus** offer essential regional insights, but their temporal resolution (from several hours to several days) and spatial granularity are not sufficient to track the **micro-environmental variations** driving ignition risks.

**Second**, satellite-based observation, while invaluable for large-scale monitoring, is limited by **update frequency, cloud cover interference, orbital constraints**, and the inability to detect **ground-level humidity or sub-canopy conditions**. Critical ignition precursors—such as localized dryness pockets or near-surface thermal anomalies—often remain invisible to orbital sensors.

**Third**, existing ground-based surveillance infrastructures (lookout towers, patrols, forest monitoring teams) provide **intermittent and localized visibility**, but cannot ensure continuous coverage of vast forested territories. These mechanisms often detect risks **late**, once visible smoke or flame appears, significantly reducing the window for preventive action.

**Fourth**, current data ecosystems are **fragmented**, with weather services, satellite systems, forest agencies, civil protection units, and local authorities operating on **parallel information streams**. The absence of a unified, real-time data layer limits the ability to build a coherent and dynamic risk picture.

**Fifth**, most existing models rely on **static or slowly updated fire danger indices** that cannot capture rapid intra-day shifts driven by wind changes, temperature spikes, human activity, or vegetation stress. As a result, short-term risk evolution remains difficult to anticipate.

**Finally**, current systems predominantly support **reactive decision-making**:  
they help guide interventions once a risk has materialized or a fire has already started, but provide **limited support for anticipatory planning**, early asset positioning, or micro-targeted prevention strategies.

Taken together, these limitations result in a **critical intelligence gap**: authorities lack a system capable of delivering **continuous, high-resolution, multi-source wildfire risk assessment** aligned with the pace at which environmental conditions evolve in high-risk Mediterranean landscapes.


#### Consequences for wildfire management and decision-making

The combined effect of these operational challenges and systemic limitations creates a **significant intelligence gap** for public authorities responsible for wildfire prevention and crisis management.  
Without access to continuous, localized, and multi-source environmental information, decision-makers face persistent uncertainty that directly affects their ability to anticipate, prioritize, and respond effectively.

**First, early-warning capacity remains limited.**  
The absence of real-time, fine-scale visibility reduces the ability to detect ignition precursors before they escalate. By the time anomalies become visible through traditional surveillance, the window for preventive intervention has often already closed.

**Second, intervention resources are frequently misallocated or mobilized too late.**  
Firefighting units, surveillance patrols, and aerial assets must cover large territories with incomplete information, resulting in:

- inefficient asset positioning,
- delayed mobilization, and
- unnecessary operational costs.  
    This reactive posture increases exposure for both personnel and communities.


**Third, intra-day changes in fire risk remain poorly captured.**  
Sudden shifts in wind patterns, humidity, or temperature can drastically increase ignition probability or accelerate propagation. Without continuous monitoring, authorities cannot adapt their readiness posture or reassign resources in time.

**Fourth, crisis coordination suffers from fragmented situational awareness.**  
Local authorities, regional crisis units, national operational centers, and European mechanisms often operate on **parallel information flows**, making it difficult to build a **shared, dynamic risk picture**.  
This complicates strategic planning, cross-institutional cooperation, and communication with the public.

**Finally, the inability to anticipate short-term fire behavior increases both environmental and economic losses.**  
When emerging ignition risks go undetected and response is delayed, fires are more likely to:

- grow rapidly,
- threaten human settlements,
- require costly large-scale interventions,
- and cause extensive ecological degradation.

Taken together, these consequences reinforce the need for a **new generation of wildfire intelligence systems** capable of providing continuous, high-resolution, integrative information to support both operational response and long-term risk governance.


---




---


## III/ Proposed Solution : LynxSense Framework
---

#### Value proposition 

In response to the growing complexity of wildfire dynamics and the structural limitations of existing monitoring systems, **LynxEye** was created with a clear mission:  
to provide public authorities with **continuous, high-resolution, multi-source environmental intelligence** capable of supporting proactive wildfire risk management.

Traditional tools offer valuable regional insights but lack the capacity to capture **fine-scale, rapidly evolving micro-environmental conditions**—conditions that determine ignition probability, early-stage propagation, and operational readiness. This gap leaves institutions without a **unified, real-time risk picture**, limiting their ability to anticipate, prioritize, and act preventively.

The **LynxSense Framework** has been designed specifically to address this challenge. It introduces a new operational capability built around three core strengths:

**1. Continuous, localized, high-frequency environmental monitoring**  
Through the integration of autonomous drones, ground-based IoT sensors, meteorological feeds, and satellite imagery, LynxSense provides a level of temporal and spatial precision that current systems cannot achieve.

**2. Multi-source integration into a single analytical ecosystem**  
Instead of fragmented datasets, LynxSense fuses environmental, meteorological, spatial, and thermal information into a coherent and continuously updated representation of risk—eliminating blind spots created by single-source monitoring.

**3. AI-enabled analytics for anticipatory decision-making**  
By combining Dynamic Risk Clusters (DRCs), real-time inference models, and predictive simulations, LynxSense supports operational planning, early warning, and strategic prioritization with unprecedented accuracy.

Together, these capabilities provide authorities with a **new generation of wildfire intelligence**, enabling a shift from reactive intervention toward **proactive, evidence-based risk governance**.  
LynxSense does not replace existing national or European systems; it **enhances and complements** them by supplying the local, real-time, integrative insights required for modern wildfire management.

#### System Overview

The **LynxSense Framework** is a multi-layered wildfire intelligence system designed to provide public authorities with **continuous, localized, and integrative risk assessment**.  
It combines **advanced sensing technologies**, **multi-source environmental data**, and **AI-driven analytical models** to deliver a real-time, operational understanding of wildfire conditions across high-risk territories.

At its core, LynxSense relies on a **distributed data acquisition network**, composed of:

- **ground-based IoT sensors** measuring humidity, soil temperature, and microclimatic variations;
- **autonomous drones** capturing high-resolution RGB and thermal imagery at regular intervals;
- **satellite feeds** from Copernicus for wide-area vegetation and thermal anomaly monitoring;
- and **meteorological data streams** from national and European forecasting systems.

These heterogeneous data sources are integrated into a **centralized analytical environment**, where they undergo continuous fusion to produce a coherent, up-to-date representation of environmental risk conditions. Instead of relying on static fire danger maps, LynxSense adopts a **dynamic monitoring approach**, continuously recalibrating risk indicators based on the latest information from each data stream.

A key component of the system is the use of **Dynamic Risk Clusters (DRCs)**:  
localized environmental units that serve as representative sampling zones for monitoring ignition conditions, vegetation stress, and short-term propagation potential. Each DRC evolves dynamically as new data are collected, allowing the system to reflect **rapid intra-day changes** in fire risk.

On this basis, the framework generates **operational outputs** tailored to the needs of public authorities, including:

- real-time risk maps,
- early-warning alerts based on threshold exceedance,
- short-term propagation scenarios,
- and decision-support dashboards integrating both micro- and macro-level intelligence.

The system is designed to **complement national and European infrastructures**, enhancing situational awareness, improving preventive posture, and strengthening the capacity of authorities to anticipate fire behavior under fast-changing environmental conditions.


#### Unique Data Acquisition Strategy

Effective wildfire anticipation requires continuous environmental monitoring at a level of **spatial granularity** and **temporal frequency** that existing systems cannot provide. The LynxSense Framework introduces a **unique, multi-source data acquisition strategy** designed to capture high-resolution information from the ground to the canopy and across the landscape.

This strategy is built on four complementary data sources, each contributing a distinct layer of environmental intelligence.

##### 1) Ground-Based IoT Sensors: Microclimatic Intelligence

IoT sensors deployed within selected **Dynamic Risk Clusters (DRCs)** provide continuous measurements of:

- soil moisture and dryness,
- near-surface temperature,
- relative humidity,
- fuel moisture proxies,
- and localized environmental anomalies.

These indicators are **critical for detecting ignition precursors** and are not measurable through satellite imagery or meteorological forecasts.  
Their high-frequency updates (minute-level or hourly) ensure permanent visibility on **micro-environmental variations** that often precede fire outbreaks.

##### 2) Autonomous Drones: High-Resolution Visual and Thermal Data

Autonomous drones equipped with **RGB and thermal cameras** conduct scheduled flyovers during peak risk hours. They capture:

- high-resolution imagery of vegetation conditions,
- thermal hotspots invisible to the naked eye,
- canopy dryness patterns,
- and early signs of combustion or stress.

Drones act as **mobile, responsive sensing units**, bridging the gap between coarse satellite observation and static ground sensors.  
They provide a unique combination of **precision**, **coverage**, and **flexibility**, enabling LynxSense to detect emerging risks before they become visible from the ground or from space.

##### 3) Satellite Observation (Copernicus, MODIS, Sentinel)

Satellite imagery offers large-scale visibility on:

- vegetation indices (NDVI, LAI, VCI),
- thermal anomalies from canopy to surface level,
- burn scars and propagation patterns,
- and macro-level fire danger conditions.

Though less frequent and less granular than drone or IoT data, satellite products allow LynxSense to contextualize each DRC within the **broader regional ecosystem**, improving understanding of structural vulnerabilities and long-range propagation drivers.

##### 4) Meteorological and Atmospheric Data

The system continuously integrates forecasts and historical datasets from:

- **Météo-France**,
- **ECMWF (ERA5)**,
- **Copernicus Atmosphere Monitoring Service (CAMS)**.

These sources provide meteorological variables essential for both ignition and propagation modelling:

- wind speed and direction,
- temperature peaks and heatwaves,
- precipitation deficits,
- atmospheric dryness,
- and boundary-layer instability.

They allow LynxSense to link **local observations** with **regional atmospheric dynamics**, ensuring coherence between micro- and macro-scale risk assessments.

#### Multi-Source Intelligence Layer

The LynxSense Framework integrates all collected data into a **unified intelligence layer** that provides public authorities with a coherent, continuously updated view of wildfire risk conditions.  
Rather than relying on any single source, the system combines **local ground observations**, **aerial imagery**, **satellite products**, and **meteorological forecasts** to deliver a **multi-dimensional understanding** of ignition potential and short-term propagation dynamics.

This intelligence layer does not describe the technical mechanisms of data fusion or modelling—which are detailed in Part IV—but provides the conceptual foundation of the system:  
the ability to transform heterogeneous environmental data into **real-time operational insights** through a unified analytical environment.

By consolidating micro-scale, meso-scale, and regional information into a single platform, the Multi-Source Intelligence Layer ensures that decision-makers benefit from **comprehensive, consistent, and actionable wildfire intelligence**, bridging the gap between local observations and broader climatic conditions.

---

## IV/ Methodology, feasibility and evaluation

#### Methodological framework 

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
- **Autonomous drones** (RGB imagery, thermal data, canopy stress indicators)
- **Satellite imagery** (Copernicus Sentinel, MODIS, EFFIS vegetation indices)
- **Meteorological feeds** (Météo-France, ECMWF, atmospheric models)

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

As new data arrive, the LynxSense engine automatically recalibrates:

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

#### Monitoring and Evaluation

To ensure accountability, measure performance, and assess the added value of the LynxSense Framework, a dedicated **Monitoring and Evaluation (M&E) system** will be implemented.  
It is structured around two complementary components:

- **a Monitoring Framework**, based on operational and analytical Key Performance Indicators (KPIs);
- **an Econometric Impact Evaluation**, designed to measure the causal effect of LynxSense on wildfire management outcomes and economic efficiency.

##### Monitoring framework (KPIs)

The Monitoring Framework will assess the performance of LynxSense across three dimensions: **operational reliability**, **predictive performance**, and **institutional benefits**.

###### 1) Operational Reliability

- Sensor uptime and data availability
- Drone mission completion rates
- Latency between data ingestion and updated risk scores
- DRC monitoring coverage

###### 2) Predictive Performance

- Accuracy of ignition probability estimates
- Accuracy of propagation forecasts
- False positive / false negative alert rates
- Stability of model recalibration over time

###### 3) Institutional and Decision-Making Value

- Reduction in detection latency
- Improvements in surveillance and resource pre-positioning
- Alignment of preventive actions with high-risk zones
- Adoption and satisfaction among operational units (SDIS, ONF, regional crisis teams)

These KPIs will support **continuous improvement**, guide operational adjustments, and inform the authorities about the effectiveness of the system during and after deployment.


#### Econometric impact evaluation v0

The objective of the econometric impact evaluation is to determine whether the deployment of LynxSense **causally improves wildfire prevention, operational decision-making, and economic efficiency**, relative to a credible counterfactual.  
This section lays out the **outcomes to measure**, the **identification strategy**, the **estimation methods**, and the **economic valuation**, ensuring that results can directly support policy decisions.

##### **Outcomes and Indicators**

The evaluation will rely on observable variables grouped into three categories:

###### A) Decision-Making Behavior

- Decision latency (time from risk signal to preventive action)
- Targeting accuracy of preventive deployments
- Proportion of resources assigned to DRCs classified as high-risk

###### B) Operational and Risk Outcomes

- Burned area per incident
- Number and share of “large fires” (>100 ha)
- Intervention costs (firefighting, logistics)

###### C) Economic and Social Outcomes

- Estimated economic losses per incident
- Expected losses avoided (treated vs. non-treated areas)
- Quantifiable indirect benefits (CO₂ avoided, tourism disruption avoided)

##### Causal Identification: Demonstrating That LynxSense Is the Cause

Establishing causality—determining whether measured improvements are **directly attributable to LynxSense**—is a core requirement for public-sector evaluation.  
The identification strategy combines several complementary quasi-experimental methods to ensure that results are **credible**, **robust**, and **policy-relevant**.

###### Difference-in-Differences (DiD): Core Causal Design

DiD is the primary identification tool.  
It compares changes over time between:

- **treated areas** (zones equipped with LynxSense), and
- **comparable untreated areas** (not yet equipped).

It automatically controls for:

- structural differences between zones,
- time-varying shocks affecting all regions (e.g., heatwaves, drought episodes),
- baseline divergence in vegetation or land use.

It ensures that estimated effects reflect **changes uniquely associated with the introduction of LynxSense**, after accounting for broader environmental and institutional trends.

$$Y_{it​}=α+βLynxSense_{it}​+γX_{it}​+δ_t​+μ_{i}​+ε_{it}​$$
	- $β$ measures the **average treatment effect**.
	- $X_{it}$​ controls for weather, vegetation, human activity.
	- Fixed effects control for structural differences across locations and over time.



#### e-Conometric Impact Evaluation 

The purpose of the econometric evaluation is to assess whether the deployment of the LynxSense Framework **effectively improves wildfire prevention and preparedness**, by enhancing **situational awareness**, **decision-making**, and ultimately **reducing fire-related impacts**.  
Since LynxSense does not extinguish fires directly, the evaluation focuses on its ability to **transform the information available to authorities**, allowing them to anticipate risks earlier, target actions more precisely, and allocate resources more efficiently.

LynxSense operates by improving **information quality and granularity**, which in turn improves **decisions**, and ultimately **risk outcomes**.  
The econometric evaluation assesses this chain through three sequential steps:

##### 1) What do we evaluate 

###### **1.1 Improved information**

The system provides:

- more frequent readings of local environmental conditions,
- high-resolution thermal and visual imagery,
- continuous updates on risk evolution.

This results in **earlier and more reliable awareness** of emerging risks.

###### **1.2 Improved decisions**

Better information enables:

- **faster preventive actions**,
- **more accurately targeted deployments**,
- **better prioritization** of surveillance and intervention zones.

###### **1.3 Improved outcomes**

If decisions improve, authorities should observe:

- fewer situations where risk escalates into uncontrolled fires,
- smaller burned areas per incident,
- lower operational and economic losses.

The evaluation measures each stage of this progression.



##### **Evaluation Outcomes**

###### **2.1 Decision-making outcomes**

These metrics capture the behavioural response of institutions to better information:

- reduction in detection-to-action latency,
- improved alignment between preventive actions and high-risk periods or zones,
- more efficient allocation of patrols, aerial surveillance, and resources.

###### **2.2 Risk and operational outcomes**

These outcomes reflect the effect of improved decisions on fire behaviour and response:

- reduction in the burned area per incident,
- lower probability of “large fires” (>100 ha),
- reduction in intervention costs and suppression efforts.

###### **2.3 Economic outcomes**

These indicators quantify the public value of LynxSense:

- avoided damages to forestry, agriculture, and infrastructure,
- reduced emergency costs,
- avoided indirect losses (CO₂ emissions, tourism disruptions).



##### **Evaluation Unit and Definition of Treatment**

The evaluation considers **territories**, not DRCs, as the unit of treatment.

###### **3.1 Treatment = territory equipped with LynxSense**

A treated area is a commune, forest district, massif or region where LynxSense is operational.

###### **3.2 DRCs = technical monitoring units**

Dynamic Risk Clusters are **not** statistical units in the evaluation:  
they provide **data**, but the evaluation measures impact at the **territorial level**.

###### **3.3 Comparison logic**

Impact is estimated by comparing:

- **equipped territories** vs. **non-equipped territories**,
- before and after deployment.

##### **4. Causal Identification Strategy**

The evaluation uses robust quasi-experimental methods to ensure that measured effects are **attributable to LynxSense**, and not to weather variation, seasonal patterns, or unrelated interventions.

###### **4.1 Difference-in-Differences (DiD)**

The core identification method compares treated and control territories across time.  
DiD controls for:

- structural differences between territories,
- time shocks (heatwaves, drought),
- environmental seasonality.

###### **4.2 Synthetic Control**

For large pilot regions, a synthetic counterfactual is constructed from weighted non-treated areas, providing a credible estimate of what the territory would have experienced without LynxSense.

###### **4.3 Propensity Score Matching (PSM)**

Matching ensures that treated and control territories are comparable in vegetation structure, drought exposure, fire history, and human pressure.

###### **4.4 Robustness checks**

- placebo assignments,
- pre-trend verification,
- alternative model specifications,
- sensitivity to extreme climatic events.

###### **4.5 Spatial spillover assessment**

Given spatial fire dynamics, the evaluation identifies whether LynxSense in one territory generates benefits for neighbouring areas.

##### **Analytical Approach**

###### **1) Fixed-effects panel models**

Used to estimate the average effect of LynxSense while controlling for unobserved territorial characteristics and time shocks.

###### **2) Event-study analysis**

Shows how outcomes evolve around the deployment of the system, and whether benefits grow as institutions adapt.

###### **3) Spatial Difference-in-Differences**

Accounts for dependence between neighbouring territories and corrections for spillovers.

###### **4) Heterogeneous treatment effects**

Identifies where LynxSense is most effective:

- dense forests vs. open shrublands,
- peri-urban vs. rural zones,
- tourism-intensive areas,
- regions with strong drought exposure.

###### **5) Environmental controls**

All models integrate meteorological and ecological variables (temperature, humidity, NDVI, soil moisture, wind conditions) to isolate the effect of LynxSense from climatic variability.

##### **Economic Valuation**

To support public budgeting and investment decisions, econometric results will be translated into financial indicators:

###### **1) Losses avoided**

Comparison between observed damages and estimated counterfactual damages.

###### **2) Cost-Benefit Ratio (B/C)**

Assesses the net economic return of the system relative to its total cost.

###### **3) Return on Investment (ROI)**

Measures how much value is created per euro invested.

###### **4) Multi-year projection**

Evaluation of cumulative benefits over 5–10 years, considering improvements in model accuracy and institutional learning.


##### **7. Policy Applications**

Econometric results will be used by authorities to:

- prioritize territories for future deployment,
- optimize investments in drones, IoT sensors, and satellite reliance,
- refine preventive strategies,
- justify long-term public funding for the system,
- support coordination between regions and European partners.


# **V/ Implementation and Resources**

L’implémentation du framework LynxSense repose sur une approche progressive et modulaire permettant d’assurer une intégration fluide avec les infrastructures existantes, de limiter les risques opérationnels et d’assurer une montée en charge pleinement maîtrisée.  
La méthodologie de déploiement a été conçue de manière à garantir :

- la cohérence technique,
- la continuité opérationnelle,
- l’interopérabilité avec les partenaires institutionnels, 
- et la robustesse du système dans la durée.


Cette section détaille :

1. le **Scope of Work**,
2. les **phases d’implémentation**,
3. les **livrables attendus**,
4. la **gouvernance du projet**,
5. les **besoins en ressources opérationnelles** (hors aspects RH détaillés).

