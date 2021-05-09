---
permalink: /models/
title: "Nowcasting models"
---


## NowcastX version 0.0.1
NowCastX version 0.0.1 - Incipient Xception-based model trained on a dataset containing 6 days with meteorological events [(threds)](https://thredds.met.no/thredds/catalog/remotesensing/reflectivity-nordic/catalog.html), selected from the CAP warnings available at [weatherapi](https://api.met.no/weatherapi/metalerts/1.1?show=all&lang=en). The model has been trained on a region of approximately 300km x 300km surrounding Oslo for predicting the composite reflectivity values at 5 minutes in the future using the values from the current timestamp. The day used for illustrating the predictions has not been used for training.

<video width="130%" controls>
  <source src="/assets/videos/xnow_5m_with_negative_5minutes_noRMSE_noCM.mp4" type="video/mp4">
</video>
