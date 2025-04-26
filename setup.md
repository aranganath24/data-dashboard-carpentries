---
title: Setup
---

This Workshop provides a gentle introduction to [Shiny](https://shiny.posit.co), which is a package that allows users to write and publish 
web applications in R or Python that allow users to interact with your research data through intuitive and interactive interfaces that facilitate
engagement and exploration. Writing applications in Shiny does not require web development or software engineering experience, which makes it an attractive
option for researchers and data scientists who are already familiar with R or Python, and would like to use these coding skills to develop web applications
based on their research data. 

The lessons (or episodes) in this Workshop can be taught in a half-day session (with periodic breaks), and will focus exclusively on working with Shiny in R (even though it is compatible,
as we have noted, with Python as well). They start with a general introduction to the potential
importance of web applications and dashboards for applied researchers working with research data, before turning to an introduction to the 
Shiny package and the package's basic syntax and vocabulary. After becoming familiar with the structure and logic of a basic Shiny app, we turn to a consideration of 
the concepts and functions that allow for interactive applications, in which applications respond to user-defined specifications or "inputs". We will then apply these techniques
to the development of applications that allow users to intuitively interact with datasets through a graphical user interface (GUI). 
Finally, the last episode focuses in more detail on one specific type of application--the data dashboard, which can be created using the principles of 
Shiny application development that are discussed in earlier episodes. This Episode introduces and uses the Shiny-based *shinydashboard* package, a package within the Shiny ecosystem that
facilitates dashboard creation. 

It's important to emphasize that the Shiny ecosystem is vast, and that programming in Shiny involves a learning curve even for researchers with experience programming in R and Python (though
the learning curve is considerably less steep than that for web development or software engineering). Our goal is not to provide participants with a comprehensive treatment of application development in Shiny, 
but with an introduction that demonstrates the value of Shiny to applied researchers, and gives them a basic foundation for continuing to explore Shiny on their own upon the Workshop's conclusion. 

Before proceeding, participants are requested to consider the prerequsites and software requirements discussed below. 

## Prerequisites

The workshop presupposes some prior experience using the R programming language, and the R Studio interface. Participants should be comfortable writing basic custom functions,
and should also be familiar with the *tidyverse*. This workshop is NOT an appropriate introduction to R and R Studio for beginners, especially because programming in Shiny using
reactive logic is different in important ways from more traditional R programming; before diving into Shiny, it's important to understand the basic principles of R programming, which 
this workshop will not explicitly review. If you have not previously used R and R Studio, but would like to learn Shiny, please consider first working through other introductory Carpentries lessons on R/R Studio,
such as [Programming with R](https://swcarpentry.github.io/r-novice-inflammation/), which covers the topic of writing custom functions, and [Data and Visualization with R for Social Scientists](https://datacarpentry.github.io/r-socialsci/),
which offers an extensive treatment of useful data wrangling and visualization functions from the *tidyverse*. 

## Software Setup

It is possible to develop Shiny applications in both Python and R, but in this Workshop, we will focus exclusively on working with Shiny in R.
In order to fully participate, therefore, you must have both [R and R Studio installed](https://posit.co/download/rstudio-desktop/#download) before the Workshop begins. 

## Libraries

We will work with a variety of R libraries over the course of the Workshop. You can install (if necessary) and load these libraries
now, or as they are needed over the course of the various episodes. They are: *shiny*, *shinydashboard*, the *tidyverse*, and 
*fivethirtyeight*, and *rsconnect*. We'll discuss these libraries at greater length as we proceed through the various episodes.  

## Data Sets

We will work with a variety of datasets over the course of the lesson. Most of these datasets are built into 
R packages that you loaded in the previous section, but we will also work with a dataset outside of the package ecosystem,
which you can load below. 

<!--
FIXME: place any data you want learners to use in `episodes/data` and then use
       a relative link ( [data zip file](data/lesson-data.zip) ) to provide a
       link to it, replacing the example.com link.
-->
Download the [data zip file](https://example.com/FIXME) and unzip it to your Desktop


