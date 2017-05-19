---
layout: project
title: Communicating meaning and purpose of spatio-temporal data analysis
subtitle: Master's Thesis, 
duration: "September 2016"
preview_image: "/img/SPODT-use-case-cropped2.png"
---

In which part of a Malian city do the children suffer more often from malaria? How did the population of an immigrated bird species increase over recent decades? Spatio-temporal statistics can give answers to these questions. On the other hand, even for experts, it can be difficult to interpret the data and to understand how and why they were generated. In my Master's thesis, I followed a semantic approach toward this problem. You can download the text from here.

I probably had to die a thousand deaths until I finished my work, but it succeeded in the end, and I am proud of it. I learned a lot!

The thesis builds upon a paper from Scheider et al. [1], which introduces an algebra that models data generation and describes how datasets are derived, in terms of types of reference systems. As a proof of concept, I adopted the algebra and created a prototypical extension for the [R environment for statistical computing](https://www.r-project.org/). The extension is able to record information in the background while the user sends commands to the R console. 

The result is a data derivation graph that can be visualized and shared, similar to the image above. Users can review this graph and thus retrace processes of data generation and derivation to its origins. Based on the algebra, the graph is (semi-automatically) annotated in a way that enables interpretation in terms of meaning and purpose of the analysis and its results. The extension also contains mechanisms to validate analyses and to monitor whether they are carried out as expected.

The thesis introduces many concepts and ideas that could have an added value for scientists interested in provenance and semantics. In the future, it may be possible to analyze, compare, and validate such data derivation graphs independent from the platform (R, ArcGIS, etc.). The algebra may enable recommendation systems that suggest procedures users can use for processing a given data set, and prompt warnings if a computation is not *meaningful from a scientific point of view*; even if these computations execute without technical or syntactical errors. 


>*“Music is a combination of sounds differing, first, in regard to space, secondly, in
>regard to time. The space between two or more sounds I call the degree of rapidity
>at which the air vibrates, in consequence of some cause which cleaves it. The cause
>of the conception of space is movement; movement necessitates the conception of
>points, or moments.”*

>Leo Tolstoy [2] - July 14th, 1850


### External Links

- [GitHub repository:  The SpatialSemantics package for R](https://github.com/MatthiasHinz/SpatialSemantics)

### References
[1]	S. Scheider, B. Gräler, E. Pebesma, and C. Stasch, “Modeling spatiotemporal information generation,” International Journal of Geographical Information Science, pp. 1–29, Mar. 2016.

[2]	L. Tolstoy, The diaries of Leo Tolstoy: tr. by C. J. Hogarth and A. Sirnia. New York: Dutton, 1917.

<a href="/documents/Hinz-MSc_Thesis.pdf" style="text-decoration: none" download >
<button class="w3-button w3-padding-large w3-margin-top w3-margin-bottom w3-theme-d3">
	<i class="fa fa-download w3-margin-right"></i>Download Master's Thesis
</button> </a>
<a href="/documents/Hinz-MSc_Thesis-Digital_Appendices.zip" style="text-decoration: none" download >
<button class="w3-button w3-padding-large w3-margin-top w3-margin-bottom  w3-theme-d3">
	<i class="fa fa-download w3-margin-right"></i>Download Appendices
</button> </a>

*Last update on May 8, 2017*
