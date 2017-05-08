---
layout: project
title: Rice Mapping in Europe
subtitle: External studies in Spain, 
duration: "October 2014 till July 2015"
preview_image: "/img/rice_field_sollana.jpg"
comments: true
---

During my Master's, I spent ten months at the University Jaume I in Castellón, Spain. It was an exciting time, as I could join the european research projects GI-N2K and ERMES. ERMES built up a rice information service that assists the European farmers and rice industry; GI-N2K provides guidance to the European education system of geospatial professionals.

Castellón de la Plana, the city where I stayed, is the capital of the province Castellon and belongs to the Valencian Community. When people ask me if I enjoyed staying there, I would usually reply with *"sometimes"* -- indeed, it was an unforgettable experience: I had fun and met interesting people, enjoyed the culture, habits, and climate. On the other hand, I experienced being a stranger in a foreign country and what it means being regarded as a stranger by others. That wasn't always easy to get along with.

Unlike Germany, Spain is stuck in an economic crisis. Appalling is the effect of the crisis on the younger generation, with a country-wide [youth unemployment rate over 50%](http://www.tradingeconomics.com/spain/youth-unemployment-rate) between 2012 and 2015. Young people seem to internalize the lack of opportunities as a permanent state in their way of thinking. Bearing that in mind, still, I would always go to Spain again, and I will always feel an emotional connection to the country and the people that live there.


### ERMES: A European Rice Information Service

<div class="w3-card w3-container w3-border-0 w3-padding" style="max-width:300px; float:left; text-align: center">
	<img src="/img/storymap.jpg" style="width:100%; max-width:500px" align="left" alt="Screenshot" />
  	<a href="http://arcg.is/2fYsveL" target="_blank" style="text-decoration: none" >
		<button class="w3-button w3-padding-large w3-margin-top w3-margin-bottom w3-theme-d3" align="middle">
			<i class="fa fa-eye w3-margin-right"></i>Display ESRI Story Map
		</button> </a>
 </div>
 
The European Union produced about 2.9 billion tons of rice in 2014. Most of it comes from Italy (48.3%), Spain (30.1%) and Greece (9.4%). A large district of rice fields, one  of three study areas of ERMES, is situated near Valencia, in the [Albufera freshwater lagoon](https://en.wikipedia.org/wiki/Albufera). Because the lagoon is not far from where I stayed, I went one day by myself to the fields and made a collection of 290 photos, which I [uploaded on Flickr](https://www.flickr.com/photos/54794825@N08/sets/72157654436183118). Later on, I made a selection of the best and created an **ESRI Story Map**, an interactive photo album, where you can see the exact GPS location from which I took each image. 

<div class="w3-card w3-container w3-border-0 w3-padding" style="max-width:300px; float:right; text-align: center">
	<img src="/img/Regional_Geoportal_rezised.jpg" style="width:100%; max-width:500px" align="left" alt="Screenshot" />
		<div class="w3-container w3-center">
		<p>The ERMES Geoportal</p>
		</div>
 </div>

ERMES brought together research institutions and companies from different countries in order to create an **E**arth obse**R**vation **M**odel-based ric**E** information **S**ervice. From many sources, they collected map data, satellite imagery, and sensor data from rice fields. Processed by different geostatistical models, information about plant growth, rice blast infection risk, and meteorological information are visualized in interactive maps and statistics. Furthermore, the project created a mobile app for farmers, which allows them to collect information directly from their fields (in-situ). It works even offline, i.e. when no internet connection is available. 


I highly recommend you to try out the Geoportal and app prototypes on [this website](http://http://ermes.dlsi.uji.es). Also, if you're interested in details of the project, please visit [the official project website](http://www.ermes-fp7space.eu/en/homepage/). 

While I was involved in the project, I administrated the server and created map services on using ArcGIS for Server. I created detailed project report about all my activities, which you can download at the and of this page.

### Geographic Information: Need to Know

GI-N2K is another EU-funded research project in which I was briefly involved during my stay. It targets the European education and training system of *Geographic Information Science and Technology (GI S & T)*: While GI S & T worldwide a growing industry, many employers have difficulties finding adequately skilled staff. The project aims to specify a consent between the labor market and education institutions upon what professionals need to learn.

 <div class="w3-card w3-container w3-border-0 w3-padding" style="max-width:350px; float:left; text-align: center">
	<img src="/img/gi-n2k-demo.jpg" style="width:100%; max-width:500px" align="left" alt="Screenshot" />
	<a href="/GIN2K-BOK-Tool-SNAPSHOT/" target="_blank" style="text-decoration: none">
	<button class="w3-button w3-padding-large w3-margin-top w3-margin-bottom w3-theme-d3">
		<i class="fa fa-eye w3-margin-right"></i>Display GI-N2K Demo
	</button> </a>
 </div>
 
The result is a so-called **Body of Knowledge (BoK)**, a modular compendium that covers knowledge areas, units, topics and education objectives. It is based on a similar compendium of the US-American [University Consortium for Geographic Information Science (UCGIS)](http://www.ucgis.org/), which you can find [here](http://gistbok.ucgis.org/). The GI-N2K project adopted this Body of Knowledge to the European marked by conducting [intensive surveys](http://www.gi-n2k.eu/surveys-results/) accoring to which the BoK was refined and updated.

The concept of a BoK is not just specific to Geographic Information Science and Technologies; it exists for  [different other professions](https://en.wikipedia.org/wiki/Body_of_knowledge) as well. The BoK can be a comprehensible guide to the following interest groups: educational institutions use it for developing study and training programs, as well as for evaluation and accreditation purposes. Professionals can use it for planing a successful career and lifelong learning. Employers can use it for screening applicants and recruiting staff according to relevant experience. They can even derive job descriptions and interview protocols from it.

My contribution to the GI-N2K project is an interactive browser application that displays the BoK as an expandable bubble chart. The application is based on the JavaScript library [d3.js](https://d3js.org/). It was planned that the visualization becomes part of a tool for curriculum planning at universities, although I've got no recent information about such follow-up activities. However, you can fork or download the source from my [GitHub repository](https://github.com/MatthiasHinz/GIN2K-BOK-Tool).


### External Links

- [The ERMES project](http://www.ermes-fp7space.eu/en/homepage/)
- [The ERMES Prototypes (GeoPortal and SmartAPP)](http://ermes.dlsi.uji.es/)
- [Flickr photo collection: Rice fields near Sollana, Valencian Comunity, Spain](https://www.flickr.com/photos/54794825@N08/sets/72157654436183118)
- [The GI-N2K project](http://www.gi-n2k.eu/)
- [GitHub repository of the BoK curriculum tool](https://github.com/MatthiasHinz/GIN2K-BOK-Tool)
- [The Geotec research group at University Jaume I](http://geotec.uji.es/)

<a href="/documents/Hinz-external_studies-final_report.pdf" style="text-decoration: none" download >
<button class="w3-button w3-padding-large w3-margin-top w3-margin-bottom w3-theme-d3">
	<i class="fa fa-download w3-margin-right"></i>Download Final Project Report
</button> </a>

*Last update on May 8, 2017*