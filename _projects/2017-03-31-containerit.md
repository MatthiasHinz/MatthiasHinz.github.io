---
layout: project
title: containerit
subtitle: Reproducible research with Docker and R,
duration: "December 2016 to March 2017"
preview_image: "/img/pexels-photo-165228_resized.jpeg"
---
*"Put your app into a container, and it runs from everywhere!"* — Docker allows packaging data and software into isolated containers that can be ported and shared. While you might spend many hours trying to install a program on your computer until it runs as it should, the container will run immediately. An appealing prospect, especially to data scientists!

Immediately after my graduation, I worked for four months on the project [Opening Reproducible Research (o2r)](http://o2r.info). Together with my supervisor, I created the R extension package `containerit`, which allows users of R to package and share their scientific work using Docker. 

[R](https://www.r-project.org/) is a free software environment and a language that scientists of many disciplines use for statistical computing. It can help solve complex analytical questions (see the  [R Journal](https://journal.r-project.org/) and [Journal of Statistical Software](https://www.jstatsoft.org)) and produce graphics (see the [R graph gallery](http://www.r-graph-gallery.com/)) or even smileys (see my example below <i class="fa fa-smile-o"></i>). To generate this smiley, I wrote a so-called R script, a text file containing a series of expressions in the R language. Ideally, this script would run on any computer with R and thus produce the same smiley. In practice, especially for the more sophisticated analyses and computations, this is rather not the case. 




<div class="w3-card w3-container w3-border-0" style="max-width:350px; float:left">
	<img src="/img/R_Smile.jpg" style="width:100%; max-width:350px" align="left" alt="R Smiley - plot" />
  	<div class="w3-container">
    		<p class=" w3-center"> Plotting graphs with RStudio </p>
  	</div>
 </div>


> *"But it works on my machine!"*

— That is an infamous quote in the field of IT (some shops even sell coffee mugs, T-shirts, etc.). The script works fine on my computer and produces a nice smiley, but it might just produce errors or confused outcomes on yours. Reasons might be that the other machine uses a different operating system (e.g., Windows instead of Linux); a newer or older version of R; different versions of extension packages or external libraries. Even country-specific locales (e.g., language, keyboard and date settings) might have a negative impact on this. As a result, making this kind of scientific work available for others requires intensive testing and regular maintenance on the part of the author or a high threshold of frustration and lots of troubleshooting on the part of the user.

But there is an alternative solution to this problem: [Docker](https://www.docker.com/) provides software containers similar to virtual machines, but they are more lightweight and flexible. It is easy to fetch a so-called Docker image and thus run a container with [Linux and R pre-installed](https://hub.docker.com/r/rocker/). One can manipulate this container so that it contains the R-script and all its dependencies, create a derivate image and share it on the internet. Once the computation works inside the container, it can be executed on any machine with Docker installed. No maintainance, no troubleshooting required.

Still, setting up a proper Docker image with metadata requires some extra work; for instance, learning the [Dockerfile syntax](https://docs.docker.com/engine/reference/builder/) and identifying all dependencies and resources must be packaged. However, using `containerit`, these tasks can be done automatically, using just a few commands in R. `containerit` enables generating a Dockerfile from R workspaces. The Dockerfile provides human-readable instructions on _how_ the Docker image is built; hence, the setup becomes transparent. Docker can process this file and then build the image.

### Example:

```R
	library(containeRit)
	dockerfile_object <- dockerfile("myRscript.R", maintainer = "Matthias Hinz")
	# print out dockerfile:
	print(dockerfile_object)
	# write dockerfile to working directory:
	write(dockerfile_object)
	# build the docker image:
	docker_build(dockerfolder = getwd(), new_image = "image_of_my_analysis")
```

`containerit` is still under development, but the core of it already works and was tested under Linux. In the future, it will hopefully become part of CRAN, the main repository of R extension packages. In the meantime, it can be installed from GitHub. For further information, please have a look at the external links below. 


### Exernal Links:
- [The containerit-package on GitHub](https://github.com/o2r-project/containerit)
- [The o2r project website](http://o2r.info/about/)
- [o2r blog post: Investigating Docker and R](http://o2r.info/2016/12/15/investigating-docker-and-R/)
- [o2r on GitHub](https://github.com/o2r-project)

*Last update on May 4, 2017*


