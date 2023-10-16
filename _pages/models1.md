---
permalink: /models1/
title: "Models"
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



<h2>Deep learning models for the Forecasting platform</h2>

<button type="button" class="collapsible">MET - Deep learning models on radar data</button>
<div class="content">



<h3>XNow 3.0.0</h3>
<p class="small" align="justify">XNow 3.0.0 - Xception-based ensemble of 3 models trained on a dataset containing 102 days of radar data (thredds). Each model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values in the future using current radar values and an improved loss function. The day used for illustrating the predictions has not been used for training.</p>

<video width="100%" controls>
  <source src="/assets/videos/V5_102Days.mp4" type="video/mp4" >
</video>

<h3>XNow 2.0.4</h3>
<p class="small" align="justify">XNow 2.0.4 - Xception-based ensemble of 3 models trained on a dataset containing 45 days of radar data (thredds). Each model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values in the future using current radar values and an improved loss function. The day used for illustrating the predictions has not been used for training.</p>

<video width="100%" controls>
  <source src="/assets/videos/V4_new_01_07_2021.mp4" type="video/mp4" >
</video>

<h3>XNow 2.0.3</h3>
<p class="small" align="justify">XNow 2.0.3 - Xception-based ensemble of 3 models trained on a dataset containing 45 days of radar data (thredds). Each model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values in the future using current radar values. The day used for illustrating the predictions has not been used for training.</p>

<video width="100%" controls>
  <source src="/assets/videos/V3_old_01_07_2021.mp4" type="video/mp4" >
</video>



<h3> XNow version 1.0.0</h3>

<p class="small" align="justify">XNow 1.0.0 - <a href="https://ieeexplore.ieee.org/document/9118849">Xception-based model</a> trained on a dataset containing 45 days of radar data <a href="https://thredds.met.no/thredds/catalog/remotesensing/reflectivity-nordic/catalog.html">(thredds)</a>. The model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values in the future using current radar values. The day used for illustrating the predictions has not been used for training.</p>
<video width="100%" controls>
  <source src="/assets/videos/xnow-4steps-5min-publ.mp4" type="video/mp4">
</video>
<p class="small">XNow 5 min - based on currently available radar data predicts the radar values 5 minutes in the future. </p>
<video width="100%" controls>
  <source src="/assets/videos/xnow-4steps-15min-publ.mp4" type="video/mp4">
</video>
<p class="small">XNow 15 min - based on currently available radar data predicts the radar values 15 minutes in the future. </p>

<h3> XNow version 0.0.1</h3>

<p class="small" align="justify">XNow 0.0.1 - Incipient Xception-based model trained on a dataset containing 6 days with meteorological events <a href="https://thredds.met.no/thredds/catalog/remotesensing/reflectivity-nordic/catalog.html">(thredds)</a>, selected from the CAP warnings available at <a href="https://api.met.no/weatherapi/metalerts/1.1?show=all&lang=en">weatherapi</a>. The model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values at 5 minutes in the future using the values from the current timestamp. The day used for illustrating the predictions has not been used for training.</p>

<video width="100%" controls>
  <source src="/assets/videos/xnow_5m_with_negative_5minutes_noRMSE_noCM.mp4" type="video/mp4" >
</video>

</div>


<button type="button" class="collapsible">NMA - Deep learning models on radar data</button>
<div class="content">

<h3>SepConv 2.0.0</h3>
<p class="small" align="justify">SepConv 2.0.0 - Separable Convolutional Neural Network-based ensemble of 3 models trained on a dataset containing 211 days with convective events (from 2020, 2021 and 2022) that occurred in central Romania, on an area defined by a 230 km radius relative to the radar site. To predict the maximum reflectivity for 6 to 48 minutes ahead, the DL model uses the radar reflectivity from four previous timestamps as input. The examples below show the radar - DL model prediction comparison for May 7, 2023, for an interval of 22.7 hours (6 min ahead) and 22.3 hours (20 min ahead), respectively.
 </p>
<video width="100%" controls>
  <source src="/assets/videos/anm_V2_wl32_3ani_6min.mp4" type="video/mp4" >
</video>
<p class="small">SepConv 2.0.0 6 min - based on currently available radar data predicts the  maximum reflectivity values 6 minutes ahead.</p>

<video width="100%" controls>
  <source src="/assets/videos/anm_V2_wl32_3ani_20min.mp4" type="video/mp4" >
</video>
<p class="small">SepConv 2.0.0 20 min - based on currently available radar data predicts the  maximum reflectivity values 20 minutes ahead.</p>
<h3>SepConv 1.0.0</h3>
<p class="small" align="justify">SepConv 1.0.0 - Improved Separable Convolutional Neural Network-based model trained using a customized weighted loss on a dataset containing 20 days with convective events that occurred in central Romania, on an area defined by a 230 km radius relative to the radar site. To predict the maximum reflectivity for the next scan (~ 6 minutes), the DL model uses the radar reflectivity from four previous timestamps as input. The day used for illustrating the maximum radar reflectivity predictions has not been used for training. The example below shows the radar - DL model prediction comparison for 22.5 hours (May 7, 2023).</p>
<video width="100%" controls>
  <source src="/assets/videos/anm_V2_wl32.mp4" type="video/mp4" >
</video>

<h3>SepConv 0.0.1</h3>
<p class="small" align="justify">SepConv 0.0.1 - Incipient Separable Convolutional Neural Network-based model trained on a dataset containing 20 days with convective events that occurred in central Romania. The radar data set used for training consists of radar reflectivity sampled at 6 elevation angles, while the deep learning (DL) model output consists in maximum radar reflectivity, computed from all 6 elevations, for each grid cell, on an area defined by a 230 km radius relative to the radar site. To predict the maximum reflectivity for the next scan (~ 6 minutes), the DL model uses the radar reflectivity from four previous timestamps as input. The day used for illustrating the maximum radar reflectivity predictions has not been used for training. The example below shows the radar - DL model prediction comparison for a two-hour time span.</p>
<video width="100%" controls>
  <source src="/assets/videos/anm_V1_xnow.mp4" type="video/mp4" >
</video>
</div>

<button type="button" class="collapsible">Deep learning models on satellite data </button>
<div class="content">
<h3>ConvSNow 1.0.0</h3>
<p class="small" align="justify">ConvSNow 1.0.0 - Convolutionary LSTM model trained on satellite imagery spanning Europe collected by EUMESAT's Meteosat-11 satellite utilizing the Severe Storms RGB product. The model was trained on 24 days from June 2021. The day used for illustrating the predictions is a day from June 2021 that has not been used for training.</p>

<img src="/assets/images/ConvSNow.gif" style="width:50%">

<p class="small" align="justify">ConvSNow 15 min - based on currently available satellite data predicts the Severe Storms RGB product 15 minutes in the future. The top side animation represents the model prediction, while the bottom side animation represents the actual (real) observation.</p>

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
