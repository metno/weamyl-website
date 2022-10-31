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

<figure>
  <center><figcaption>The WeaMyL System</figcaption></center>
  <img src="/assets/images/Container.png" alt="The WeaMyL System" style="width:100%">
</figure>


<button type="button" class="collapsible"><h1>Nowcasting models</h1></button>
<div class="content">

<h2> NowCastX version 1.0.0</h2>

<p class="small" align="justify">NowCastX version 1.0.0 - <a href="https://ieeexplore.ieee.org/document/9118849">Xception-based model</a> trained on a dataset containing 45 days of radar data <a href="https://thredds.met.no/thredds/catalog/remotesensing/reflectivity-nordic/catalog.html">(thredds)</a>. The model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values in the future using current radar values. The day used for illustrating the predictions has not been used for training.</p>
<video width="100%" controls>
  <source src="/assets/videos/xnow-4steps-5min-publ.mp4" type="video/mp4">
</video>
<p class="small">NowCastX 5 min - based on currently available radar data predicts the radar values 5 minutes in the future. </p>
<video width="100%" controls>
  <source src="/assets/videos/xnow-4steps-15min-publ.mp4" type="video/mp4">
</video>
<p class="small">NowCastX 15 min - based on currently available radar data predicts the radar values 15 minutes in the future. </p>

<h2> NowCastX version 0.0.1</h2>

<p class="small" align="justify">NowCastX version 0.0.1 - Incipient Xception-based model trained on a dataset containing 6 days with meteorological events <a href="https://thredds.met.no/thredds/catalog/remotesensing/reflectivity-nordic/catalog.html">(thredds)</a>, selected from the CAP warnings available at <a href="https://api.met.no/weatherapi/metalerts/1.1?show=all&lang=en">weatherapi</a>. The model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values at 5 minutes in the future using the values from the current timestamp. The day used for illustrating the predictions has not been used for training.</p>

<video width="100%" controls>
  <source src="/assets/videos/xnow_5m_with_negative_5minutes_noRMSE_noCM.mp4" type="video/mp4">
</video>
</div>

<button type="button" class="collapsible"><h1>Annotated Atlas of Meteorological Observations</h1></button>
<div class="content">

<p class="small" align="justify">This component offers a web interface to a search engine connected to a semantic database which contains severe weather warnings. The web interface is easy to use and allows searching/filtering for different types of weather events and also for named weather events. The web interface also offers the possibility to investigate geographical areas affected by annotated and earlier events. In addition, It provides information about where to find the source data files, hence, providing support to the training machine learning models to detect interesting possible weather events.</p>

<img src="/assets/images/Atlas.png"/>
</div>

<button type="button" class="collapsible"><h1>Forecasting Platform</h1></button>
<div class="content">

<p class="small" align="justify">The forecasting platform consists of the following components:</p>
<ul>
<li> <p class="small" align="justify"> GeoWeb - A web application used to visualize all kinds of meteorological data. That includes output from the machine learning algorithm and CAP warnings.</p></li>

<li style="small"><p class="small" align="justify">  WebMapService providing data from the ML algorithms - Services providing all kinds of meteorological data, including model output satellite images, radar data, in situ observations as images that can be displayed on a map.</p></li>

<li > <p class="small" align="justify"> Machine Learning Algorithms - producing forecasts based on the latest recorded radar data sets.</p></li>

<li> <p class="small" align="justify"> WebMapServices - Services providing all kinds of meteorological data, including model output, satellite images, radar data, in situ observations, as images that can be displayed on a map.</p></li>

<li > <p class="small" align="justify"> CAP editor - editor used by the forecaster to produce CAP warnings.</p></li>

<li> <p class="small" align="justify"> CAP feed - service providing all issued CAP warnings.</p></li>

</ul>

<p class="small" align="justify">Below is an example of visualizing the ML output as forecast (left) versus observed (right) equivalent reflectivity factor using the Open GeoWeb mapping service for the weather event on April 08, 2022 at 18:05 UTC. This visualization is based on data assimilated every 5 to 10 minutes.</p>

<img src="/assets/images/demo_GeoWeb.png" />

<p class="small" align="justify">The video</p>

<video width="100%" controls>
  <source src="/assets/videos/GeoWeb_demo.mp4" type="video/mp4">
</video>

</div>

<script>
var coll = document.getElementsByClassName("collapsible");
var i;

for (i = 0; i < coll.length; i++) {
  coll[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var content = this.nextElementSibling;
    if (content.style.display === "block") {
      content.style.display = "none";
    } else {
      content.style.display = "block";
    }
  });
}
</script>



</body>
</html>
