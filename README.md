# ISRO-Bharatiya-Antariksh-Hackathon-2026
🌍 AgriTwin India

AI-Driven Crop Type Identification, Moisture Stress Detection & Irrigation Advisory System

Bharatiya Antariksh Hackathon 2026 | Team: Cosmic Compile
📌 Problem Statement

AI-Driven Automated Crop Type, Moisture Stress Detection and Irrigation Advisory Across Growth Stages Using Moderate Resolution Spectral Signatures (Optical & Microwave Satellite Data)

Traditional agricultural monitoring tools are largely descriptive — they report what already happened rather than predicting what's coming. This leaves farmers and irrigation authorities reacting to water stress and crop failure instead of preventing it. AgriTwin India flips this paradigm using satellite Earth Observation and AI.


🚀 About the Project

AgriTwin India transforms multi-source satellite observations into a living digital twin of India's farmlands. Every field is continuously monitored, every crop's growth stage is intelligently tracked, and every irrigation decision is guided by predictive, explainable AI — enabling proactive, water-efficient agriculture at national scale.


"AgriTwin India is a state-adaptive AI Digital Twin converting satellite telemetry into explainable, predictive irrigation advisories and precision water management."

✨ Key Differentiators

Descriptive → Predictive: Simulates upcoming irrigation shortages and crop risks instead of only reporting historical stress.
State-Specific AI Engines: Localized crop calendars, climate cycles, and irrigation command targets replace one-size-fits-all national models.
Optical + SAR Microwave Fusion: Cloud-penetrating radar (SAR) keeps monitoring active even through heavy monsoon cloud cover.
Explainable AI: Every stress rating is backed by transparent physical indicators (NDWI shifts, SAR dB drops) — not a black box.
Command-Area Optimization: Ranks canal networks and irrigation gates by severity, aligned with PMKSY (Pradhan Mantri Krishi Sinchayee Yojana) goals.


🧩 Core Features

#FeatureDescription1Crop Type IdentificationAutomatically identifies crop varieties using fused Optical + SAR satellite imagery2Moisture Stress DetectionDetects water deficiency early, before visible crop symptoms appear3Growth Stage MonitoringTracks crop development from sowing to harvest using an AI phenology engine4Irrigation AdvisoryDelivers field-specific recommendations — how much, when, and where to irrigate5Multi-Source Satellite FusionCombines Optical and SAR data for uninterrupted monitoring, even in cloudy/monsoon conditions6Smart DashboardVisualizes crop health, moisture maps, irrigation alerts, and insights for farmers & officials


🔄 Processing Pipeline

Optical + SAR Satellite Data
        │
        ▼
Image Pre-processing (cloud masking, noise removal, geometric correction)
        │
        ▼
AI Crop Classification (field-level crop type detection)
        │
        ▼
Moisture Stress Detection (NDVI + NDWI + SAR features)
        │
        ▼
Growth Stage Identification (AI Phenology Engine: Sowing → Vegetative → Flowering → Maturity)
        │
        ▼
AI Irrigation Recommendation (volume, timing, method)
        │
        ▼
Farmer & Irrigation Dashboard (Mobile App + Web Portal)

Data Inputs: Optical Data (Sentinel-2, Resourcesat) · SAR Data (Sentinel-1, RISAT) · Weather Data (rainfall, temperature, humidity) · Ground Data (soil, field observations)


🏗️ System Architecture


Data Sources — Satellite (Sentinel-1/2, Landsat, LISS, AWiFS, MODIS), Weather, and auxiliary data (soil, DEM, land use, canal/reservoir boundaries, historical crop data)
Ingest & Store — Real-time/batch ingestion into cloud data lake storage
Preprocess & Fuse — Cloud masking, SAR speckle filtering, geo-correction, multi-source fusion
AI Digital Twin Engine — Crop classification, growth stage detection, moisture stress prediction, water deficit estimation via state-adaptive AI models
Decision & Advisories — Irrigation recommendations, water allocation priority, canal command optimization, monsoon intelligence, risk alerts, yield forecasts
Platform & Data Infrastructure — Cloud infrastructure, spatial database, AI/ML services, analytics engine, security & access control
Users & Stakeholders — Farmers, government & policy makers, irrigation departments, researchers, NGOs, and private organizations
Application & Visualization Layer — Interactive GIS dashboard, mobile app, time-series analytics, reports, and scenario simulation

Feedback Loop: Field feedback and ground truth continuously retrain and validate the AI models, improving future advisories.


🛠️ Tech Stack

ComponentTechnologies / ToolsPlatforms / LibrariesPurposeProgrammingPythonJupyter Notebook, Google ColabCore development & experimentationSatellite & Geospatial ProcessingGoogle Earth Engine (GEE)GDAL, Rasterio, GeoPandasAccess, preprocess, and analyze satellite imageryData SourcesSentinel-1 & Sentinel-2Landsat-8/9, MODIS, ISRO Bhuvan/BhoonidhiMulti-source optical & SAR dataMachine LearningRandom ForestXGBoost, LightGBMCrop classification & suitability analysisDeep LearningLSTMTemporal CNN, U-NetTime-series forecasting & pixel-level mappingFeature EngineeringNumPyPandas, SciPyIndex computation & data processingDatabase & StoragePostgreSQL + PostGISMongoDB, AWS S3Store spatial & tabular dataVisualizationPlotlyMatplotlib, FoliumInteractive charts & mapsDashboard/UIStreamlitPlotly Dash, React + LeafletUser-facing dashboard & advisoriesDeployment & CloudAWSDocker, Google CloudScalable deploymentCollaboration & Version ControlGitGitHub ActionsTeam collaboration & CI/CD


💰 Estimated Implementation Cost

Prototype Phase (Command Area Pilot)

ComponentTech Stack / InfrastructureCost (INR)Cloud ComputeOn-demand VMs & Serverless APIs₹15,000 – ₹25,000Data PipelineGIS processing & spatial DB hosting₹5,000 – ₹10,000Web DashboardInteractive GIS hosting & UI deployment₹5,000 – ₹10,000AI/ML EnginesTensorFlow, PyTorch, Scikit-learnOpen SourceSatellite ImagerySentinel-1/2, Landsat, MODIS, GEEOpen AccessRegional ImageryISRO Bhuvan / Bhoonidhi portalsGov AccessEstimated Prototype TotalServerless on-demand architecture₹25,000 – ₹45,000

National Scale Deployment (Indicative)

₹50 Lakhs – ₹2 Crores — scales seamlessly to state/national architectures using government cloud infrastructure (NIC / MeghRaj Cloud) without core software re-engineering.


Open-Source Core: Uses GDAL, Rasterio, and Python frameworks to avoid proprietary GIS licensing fees
Free Earth Observation: Processes ESA and ISRO open satellite data, minimizing acquisition costs
On-Demand Compute: Serverless architecture triggers analysis only on satellite overpasses, eliminating idle costs
Modular Scaling: Decoupled microservices allow scaling from pilot sectors to entire states incrementally



🖥️ Proposed Prototype

The prototype includes:


Farmer Dashboard with real-time crop health, weather, and an Expert Chat feature connecting farmers directly with agronomists, plant pathologists, soil scientists, and irrigation experts
Phenology Monitoring panel tracking crop lifecycle stage (e.g., Flowering) with NDVI/LAI metrics and next-stage forecasts
National Agricultural Digital Twin view showing aggregated crop health, moisture stress, water deficit, and irrigation demand across India
Canal Network Topology view for reservoir capacity, live flow telemetry, and AI-driven water routing strategy
Monsoon Intelligence panel tracking onset, rainfall anomalies, dry-spell districts, and flood probability



👥 Team — Cosmic Compile

RoleNameCollegeTeam LeaderPriyan SaxenaJaypee Institute of Information Technology, NoidaTeam MemberAkansha NagarJaypee Institute of Information Technology, NoidaTeam MemberMadhav KansalJaypee Institute of Information Technology, Noida


🇮🇳 About Bharatiya Antariksh Hackathon 2026

Welcome to the third edition of the Bharatiya Antariksh Hackathon — a national innovation initiative by the Indian Space Research Organisation (ISRO), powered by Hack2skill.

Bringing together student innovators from across India, the hackathon invites undergraduates, postgraduates, research scholars, and aspiring problem-solvers to tackle real-world challenges inspired by India's growing ambitions in space technology and exploration.

More than a competition, Bharatiya Antariksh Hackathon 2026 is an opportunity to innovate for the nation's future in space. Collaborate with brilliant minds, learn from ISRO scientists and domain experts, and build impactful solutions that can contribute to the next era of India's space-tech ecosystem.


📄 License

This project was created as a submission for the Bharatiya Antariksh Hackathon 2026 (ISRO × Hack2skill).


