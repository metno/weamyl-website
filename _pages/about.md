---
permalink: /about/
title: "About WeaMyL"
---

WeaMyL project aims at enhancing the accuracy, performance and reliability of national nowcasting warning systems by the use of machine learning (ML) techniques applied on radar, satellite and weather stations’ observations. The focus will be on obtaining higher precision in predicting the occurrence and the areas affected by severe meteorological phenomena, as well as attaining lower decision times (compared to current, exclusively human decision times). The project’s main goal is to automate the nowcasting warning systems by creating a ML driven platform for early and accurate forecast of severe phenomena. Thus, it is aimed to be the backbone of a new framework for imminent severe weather detection adapted to current technological possibilities.

## Main objectives

The main objectives of the project are  the following:

* Development and scientific validation of novel ML computational models and techniques
  specially tailored for accurate nowcasting. Unsupervised Learning (UL) models such as Principal Component Analysis, T-distributed Stochastic Neighbor Embedding, clustering, and auto-encoders are envisaged as intelligent tools for analyzing multiple data sources which may be relevant for accurate nowcasting: meteorological data (radar, satellite, weather stations’ observations) and geographical data (elevation, exposure, vegetation, hydrological features, anthropic features). Following unsupervised data analysis, both off-line and on-line Supervised Learning methods such as Convolution Neural Networks, U-Nets, Long Short Term Memory Networks, XGBoost, and Restricted Boltzmann Machines will be developed to assist meteorologists in providing precise nowcasting alerts.

* Development and user evaluation of the Annotated Atlas of Meteorological Observations, a large database containing meteorological data (radar, satellite and other relevant meteorological observations) being used as a data source for the Deep Learning techniques developed within the project (data extraction, processing and classification). After project completion, the Annotated Atlas will be available for meteorological data analyses, authoring of scientific papers, personnel training and public dissemination of meteorological data. The Atlas will offer: (1) management of annotated meteorological observations (add, update, save, load, annotate and validate meteorological records) and (2) intelligent information retrieval techniques for retrieving historical information relevant for meteorologists in real-time. This includes early identification of areas prone to convection initiation based on statistical data as well as identification of convective storm patterns based on historical data. Different queries and visualizations for specific observations will be accessible and will include those provided by the unsupervised methods developed as part of O1 together with different reporting results.

* Development of the open-source WeaMyL platform for early forecast of severe weather phenomena. The objective is to provide a big-data based forecasting platform that includes the Supervised Learning methods developed and which supports meteorologists in improving the quality of nowcasting alerts.
* Integration of the WeaMyL platform within the national weather warning systems of Norway and Romania. The WeaMyL platform will be integrated with the relevant software systems of the National Meteorological Services. This integration will directly facilitate the meteorologists’ activity by assisting them in the nowcasting decision process and will accelerate alert issuing procedures.
* Contribute to the development of scientific knowledge by disseminating the obtained scientific results through scientific publications, the project website and social media.

## WeaMyL software platform

The WeaMyL software platform consists of three components such as the,

* **Forecasting Platform**. Given that the accuracy of the prediction module is paramount for the system’s precision, this is WeaMyL’s central component. The forecasting platform employs historical and real-time data and is responsible with estimating the location, time and severity of meteorological phenomena expected to take place in the near future (0-6 hours). Our algorithms will model the meteorological situation based on the earlier meteorological situations. The employed learning models will find patterns in the meteorological data which apply to specific circumstances and thus improve themselves as increasingly more data becomes available, hence making the forecasting module self-adaptive. To process the available amount of meteorological data and to accelerate scientific analysis and information extraction, big data approaches will be targeted.
* **Annotated Atlas of Meteorological Observations** The Annotated Atlas component will provide a semantic database over the large volume of historical data from varying  sources, including weather stations’ observations, radar and satellite imagery. Its main objectives are to facilitate the study of past conditions using statistical and comparative analyses, provide intelligent information retrieval based on a semantic data model, and provide a custom, extensible annotation model across observation types and sources. The Atlas component will offer two main functionalities: (a) management of the Atlas and (b) visualizations, statistics and reports based on the historical meteorological data stored in the Atlas.
* **Integration Module**. In order for the above components to provide actionable
information, they must be integrated with the software systems already deployed on location. The purpose of this module is to provide a number of data consumer and data provider connectors that can be integrated within existing systems. Both the Forecasting Platform and the Annotated Atlas will act as consumers for real-time generated meteorological data, while the Forecasting Platform will provide data relevant to upcoming severe weather.

## Work Packages

The work programme is divided into five work packages (WPs), following the usual stages needed to reach the main research objective, namely to develop the WeaMyL software platform. These are:

### WP1 - Documentation, system requirements and architecture
In this work package, we will first conduct a documentation, study and literature analyses. Then, we will identify the limitations of existing state-of-the-
art approaches and solutions in nowcasting. Afterwards, we aim at defining the functional and nonfunctional requirements for WeaMyL including the end-user requirements, as well as the main conditions for the system's proper functioning in order to establish the general architecture and design of the WeaMyL software platform.

### WP2 - Machine learning models for weather nowcasting
The second work package consists of defining a theoretical model for nowcasting along with (2) Develop specially tailored scalable ML models for accurate
nowcasting. (3) Scientifically validate developed ML models using experimental results analysis and
interpretation, as well as comparison to related work.

### WP3 - Software development, testing and integration
WP3 is focused on software development, testing, and platform integration with national warning systems. The Forecasting Platform is comprised of the ML components (accessible via an API) together with the front-end. An effort is made concerning the integration of WeaMyL with national warning systems. The platform prototype will be developed in an incremental, iterative manner, having as final objective its successful integration with Romanian and Norwegian weather warning systems.

### WP4 - Meteorological evaluation, interpretation and analysis
WP4 activities include extracting, annotating and validating relevant meteorological data from NMA and MET databases and piloting the platform within NMA and MET locations. These activities will be coordinated by NMA in close cooperation with MET-MT. Results concerning the accuracy, performance and reliability of the platform will be discussed with MET-IT and BBU. The feedback will be used to continuously improve the ML modules, front-end components and the Annotated Atlas.
