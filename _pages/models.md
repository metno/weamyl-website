---
permalink: /models/
title: "Results"
---
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.collapsible {
  background-color: #2073ac;
  color: white;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
}

.active, .collapsible:hover {
  background-color: #555;
}

.content {
  padding: 0 18px;
  display: none;
  overflow: hidden;
  background-color: #f1f1f1;
}
</style>
</head>

<body>
<a href="https://weamyl.met.no/models1"><button type="button">Machine Learning models for the Nowcasting platform</button></a>
<h2>Overview of the WeaMyL System</h2>
<figure>

  <img src="/assets/images/Container.png" alt="Overview of the WeaMyL System" style="width:100%">
</figure>

<h2>Forecasting Platform</h2>

<a href="https://weamyl.met.no/models1">Machine Learning models for the Nowcasting platform</a>
<br>

<p class="small" align="justify"><b>Video 1.</b> An example illustrating the observed equivalent reflectivity factor (left) versus the forecast of XNow 1.0.0 (middle) versus the forecast of XNow 2.0.3 (right) using the Open GeoWeb mapping service for the weather event on June 28, 2022 at 09:55 UTC. This video is generated using the models, as the platform is intended to be used by meteorologists to analyze the weather 60 minutes into the future.	</p>

<video width="100%" controls>
  <source src="/assets/videos/video29mar.mp4" type="video/mp4">
</video>
<br><br>
<p class="small" align="justify"><b>Video 2.</b> This video is generated using the model XNow version 0.0.1, as the platform is intended to be used by meteorologists to analyze the weather 5 minutes into the future.</p>

<video width="100%" controls>
  <source src="/assets/videos/GeoWeb_demo.mp4" type="video/mp4">
</video>

<br>

<b>Annotated Atlas of Meteorological Observations</b>
<p class="small" align="justify">This component offers a web interface to a search engine connected to a semantic database which contains severe weather warnings. The web interface is easy to use and allows searching/filtering for different types of weather events and also for named weather events. The web interface also offers the possibility to investigate geographical areas affected by annotated and earlier events. In addition, It provides information about where to find the source data files, hence, providing support to the training machine learning models to detect interesting possible weather events.</p>

<img src="/assets/images/atlas1.png"/>

</body>
</html>
