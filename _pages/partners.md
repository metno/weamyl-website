---
permalink: /partners/
title: "Team"
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


<h2>The consortium members</h2>

<button type="button" class="collapsible">Babeș-Bolyai University (BBU)</button>
<div class="content">
<!--## Babeș-Bolyai University (BBU)-->
<p class="small" align="justify">Babeș-Bolyai University is a public comprehensive university, being today the largest university in Romania and one of the best and most representative Romanian universities. At national level, BBU has been awarded the title of intensive-research university and was ranked the best Romanian university in the metaranking of <a href="https://cwur.org/2019-2020.php">CWUR World University Rankings 2019-2020</a>. The Computer Science research team from BBU is a research group in ML (MLyRE – www.cs.ubbcluj.ro/ml) from the Faculty of Mathematics and Computer Science formed by members with high expertise and valuable scientific results in the artificial intelligence field, particularly in ML. Please see the <a href="https://weamyl.met.no/bbu">partner page</a> for further details.</p>
<table style="width:100%">
  <tr>
    <td><img src="/assets/images/ubb/UBB7.png"></td>
    <td><img src="/assets/images/ubb/UBB2.png"></td>
  </tr>
  <tr>
    <td><img src="/assets/images/ubb/UBB5.png"></td>
    <td><img src="/assets/images/ubb/UBB1.png"></td>
  </tr>
</table>


</div>

<button type="button" class="collapsible">The National Meteorological Administration of Romania (NMA)</button>
<div class="content">
<!--## The National Meteorological Administration of Romania (NMA)-->
<p class="small" align="justify">The National Meteorological Administration (NMA) is the National Meteorological Service of Romania responsible for providing services for the protection of life and property in the form of weather and climate-related information, including warning of severe meteorological events that could endanger public safety. Also, NMA provides a wide range of operational meteorological services for various users in agriculture, maritime and air navigation, national defense, transport, energetics, tourism and environment</p>


<p class="small" align="justify">NMA holds high expertise in meteorological research (severe weather, weather numerical modelling, climate variability and climate change, physics of the atmosphere and air pollution, remote sensing and GIS) and operational domains. Regarding education and training, NMA is deeply involved in activities within its National Meteorological School as well as in international training courses. Please see the <a href="https://weamyl.met.no/anm">partner page</a> for further details.</p>

<table style="width:100%">
  <tr>
    <td><img src="/assets/images/anm/anm2.jpg"></td>
    <td><img src="/assets/images/anm/anm3.jpg"></td>
  </tr>
  <tr>
    <td><img src="/assets/images/anm/anm9.jpg"></td>
    <td><img src="/assets/images/anm/anm4.jpg"></td>
  </tr>
</table>

</div>
<button type="button" class="collapsible">The Norwegian Meteorological Institute (MET Norway)</button>
<div class="content">
<!--## The Norwegian Meteorological Institute (MET Norway)-->
<p class="small" align="justify">The Norwegian Meteorological Institute (MET Norway) is a state agency from Norway, a leading international centre of expertise responsible for public meteorological services for civil and military purposes. It forecasts weather, monitors the climate and conducts research. MET Norway is actively involved in the work of the WMO, the European Centre for Medium Range Weather Forecasts, and the European Organization for the Exploitation of Meteorological Satellites (EUMETSAT). The main research and development activities include atmospheric, oceanic and climatological research and involve both models and observations. MET Norway has also a long record of participation in regional and EEA/Norway Grant programmes in addition to EU-grants, projects funded by external organisations, and projects funded by the Norwegian Research Council and the Nordic organisation NordForsk. Please see the <a href="https://weamyl.met.no/metno">partner page</a> for further details.</p>

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
