---
title: "Introduction and Motivation"
teaching: 10
exercises: 10
---

:::::::::::::::::::::::::::::::::::::: questions 

- Why might you want to create an interactive data application or dashboard as a wrapper for your research data?
- What is the *Shiny* package in R?
- What are some examples of data applications or dashboards created with the Shiny package ecosystem? 

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Survey published examples of Shiny applications and dashboards and explore some of their features and properties
- Reflect on what an "ideal" application or dashboard would look like for your particular research data use case
- Appreciate the relevance of data applications and dashboards for Open Science

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction: Interactive Data Applications for Open Science

The practice of open science promotes a global “knowledge commons” that has the potential to support enlightened and informed public discourse. While open scholarly outputs such as open-access publications and research datasets are typically intended for scholarly audiences with specialized training and expertise, the broader public is a critical stakeholder in open science, and researchers may wish to invite non-specialist audiences to engage with their research data and findings for a variety of reasons, such as the following: 

* Some researchers may view it as a civic duty, to the extent that a significant share of scientific research is ultimately funded by the public
* It offers academic researchers an opportunity to build their public profiles beyond their scholarly communities, which allows them to credibly share their expertise 
* It could help to build public appreciation for open science and academic research, which could have valuable downstream impacts (i.e. increased funding)
* The research data may cast important light on issues of public interest or public policy, and making it available to a broad non-specialist audience in an accessible form could contribute to a more informed or enlightened public discourse

In short, the dissemination of research data to non-specialist audiences can be an important and valuable part of scientific communication in the context of open science. However, it can be challenging to present complex research datasets in ways that are intuitive, accessible, and engaging to a broader audience. One way to do so is through the use of digital applications that wrap research datasets into an interactive graphical-user-interface (GUI) that allows non-specialists to explore and query the underlying data. These applications can be constructed in any number of ways. Data dashboards are one example of a GUI-based data exploration application; typically, a dashboard offers an interactive visual display of multiple pieces of information in different formats, arrayed across different sections or "panels" of a rectangular display. One famous example of a data dashboard is the [COVID-19 Dashboard](https://coronavirus.jhu.edu/map.html), developed by the Center for Systems Science and Engineering at Johns Hopkins:

<div class="figure" style="text-align: center">
<img src="fig/fig1-covid-dashboard.png" alt="Figure 1. The Johns Hopkins COVID-19 Dashboard"  />
<p class="caption">Figure 1. The Johns Hopkins COVID-19 Dashboard</p>
</div>

Data dashboards, and interactive data applications more generally, are frequently used in government, public health, and corporate contexts in which important and potentially complex information needs to be communicated with a broad audience in an accessible way. However, they are not used as frequently in the context of communicating information and insights derived from research data. There could be many potential reasons for this, one of which is that the creation of these applications can be time-consuming and resource-intensive for researchers and scientists who do not have previous experience with application development. For such researchers, who would like to develop simple applications that could help foster broader engagement with their research and data, but do not have software expertise or access to specialized programs that facilitate application or dashboard creation, the *Shiny* package ecosystem is an excellent option. 

## The *Shiny* Package Ecosystem for Interactive Application Development

https://shiny.posit.co/r/gallery/#user-showcase 




This is a lesson created via The Carpentries Workbench. It is written in
[Pandoc-flavored Markdown](https://pandoc.org/MANUAL.txt) for static files and
[R Markdown][r-markdown] for dynamic files that can render code into output. 
Please refer to the [Introduction to The Carpentries 
Workbench](https://carpentries.github.io/sandpaper-docs/) for full documentation.

What you need to know is that there are three sections required for a valid
Carpentries lesson template:

 1. `questions` are displayed at the beginning of the episode to prime the
    learner for the content.
 2. `objectives` are the learning objectives for an episode displayed with
    the questions.
 3. `keypoints` are displayed at the end of the episode to reinforce the
    objectives.

:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::: instructor

Inline instructor notes can help inform instructors of timing challenges
associated with the lessons. They appear in the "Instructor View"

::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: challenge 

## Challenge 1: Can you do it?

What is the output of this command?

```r
paste("This", "new", "lesson", "looks", "good")
```

:::::::::::::::::::::::: solution 

## Output
 
```output
[1] "This new lesson looks good"
```

:::::::::::::::::::::::::::::::::


## Challenge 2: how do you nest solutions within challenge blocks?

:::::::::::::::::::::::: solution 

You can add a line with at least three colons and a `solution` tag.

:::::::::::::::::::::::::::::::::
::::::::::::::::::::::::::::::::::::::::::::::::

## Figures

You can also include figures generated from R Markdown:


``` r
pie(
  c(Sky = 78, "Sunny side of pyramid" = 17, "Shady side of pyramid" = 5), 
  init.angle = 315, 
  col = c("deepskyblue", "yellow", "yellow3"), 
  border = FALSE
)
```

<div class="figure" style="text-align: center">
<img src="fig/introduction-rendered-pyramid-1.png" alt="pie chart illusion of a pyramid"  />
<p class="caption">Sun arise each and every morning</p>
</div>

Or you can use standard markdown for static figures with the following syntax:

`![optional caption that appears below the figure](figure url){alt='alt text for
accessibility purposes'}`

![You belong in The Carpentries!](https://raw.githubusercontent.com/carpentries/logo/master/Badge_Carpentries.svg){alt='Blue Carpentries hex person logo with no text.'}

::::::::::::::::::::::::::::::::::::: callout

Callout sections can highlight information.

They are sometimes used to emphasise particularly important points
but are also used in some lessons to present "asides": 
content that is not central to the narrative of the lesson,
e.g. by providing the answer to a commonly-asked question.

::::::::::::::::::::::::::::::::::::::::::::::::


## Math

One of our episodes contains $\LaTeX$ equations when describing how to create
dynamic reports with {knitr}, so we now use mathjax to describe this:

`$\alpha = \dfrac{1}{(1 - \beta)^2}$` becomes: $\alpha = \dfrac{1}{(1 - \beta)^2}$

Cool, right?

::::::::::::::::::::::::::::::::::::: keypoints 

- Use `.md` files for episodes when you want static content
- Use `.Rmd` files for episodes when you need to generate output
- Run `sandpaper::check_lesson()` to identify any issues with your lesson
- Run `sandpaper::build_lesson()` to preview your lesson locally

::::::::::::::::::::::::::::::::::::::::::::::::

[r-markdown]: https://rmarkdown.rstudio.com/
