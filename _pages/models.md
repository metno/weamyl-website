---
permalink: /models/
title: "Nowcasting models"
---

<!-- ## NowcastX version 0.0.1
NowCastX version 0.0.1 - Incipient Xception-based model trained on a dataset containing 6 days with meteorological events [(thredds)](https://thredds.met.no/thredds/catalog/remotesensing/reflectivity-nordic/catalog.html), selected from the CAP warnings available at [weatherapi](https://api.met.no/weatherapi/metalerts/1.1?show=all&lang=en). The model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values at 5 minutes in the future using the values from the current timestamp. The day used for illustrating the predictions has not been used for training. -->

## NowCastX version 1.0.0

<p class="small">NowCastX version 1.0.0 - Xception-based model trained on a dataset containing 45 days of radar data (thredds). The model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values in the future using radar current radar values. The day used for illustrating the predictions has not been used for training.</p>
<video width="130%" controls>
  <source src="/assets/videos/xnow-4steps-5min-publ.mp4" type="video/mp4">
</video>
<p class="small">NowCastX 5 min - based on currently available radar data predict the radar values 5 minutes in the future. </p>
<video width="130%" controls>
  <source src="/assets/videos/xnow-4steps-15min-publ.mp4" type="video/mp4">
</video>
<p class="small">NowCastX 15 min - based on currently available radar data predict the radar values 15 minutes in the future. <p>


## NowCastX version 0.0.1

<p class="small">NowCastX version 0.0.1 - Incipient Xception-based model trained on a dataset containing 6 days with meteorological events <a href="https://thredds.met.no/thredds/catalog/remotesensing/reflectivity-nordic/catalog.html">(thredds)</a>, selected from the CAP warnings available at <a href="https://api.met.no/weatherapi/metalerts/1.1?show=all&lang=en">weatherapi</a>. The model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values at 5 minutes in the future using the values from the current timestamp. The day used for illustrating the predictions has not been used for training.</p>

<video width="130%" controls>
  <source src="/assets/videos/xnow_5m_with_negative_5minutes_noRMSE_noCM.mp4" type="video/mp4">
</video>
