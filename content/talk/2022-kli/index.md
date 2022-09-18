---
title: R Markdown Workshop
draft: false
event: 'Educational Series for Behavioral Researchers in the Netherlands, Kurt-Lewin Institute'
event_url: 
location: remote
summary: "A workshop on data analysis, reporting, and collaboration using R, R Markdown, osf, blogdown, and GitHub."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2022-05-24T09:00:00Z"
date_end: "2022-05-25T15:00:00Z"
all_day: true
publishdate: "2022-05-24"

categories:
  - panel
featured: no
image:
  focal_point: 'center'
  preview_only: no
projects: []
links:
- icon: images
  icon_pack: fas
  name: slides
  url: https://anneokk.netlify.app/slides/day_one.html
- icon: github
  icon_pack: fab
  name: materials
  url: https://github.com/AnneOkk/Workshop_Rmarkdown/tree/master/content/blog/Workshop_day_one
---

# Preparation 

#### 1) Install R 

Please make sure that you have a [recent R version](https://cran.rstudio.com/) installed (>= 4.0.0 is recommended). 
You can check your R Version in the Console (in RStudio) by typing:
`R.version.string`

<img src="images/rvers.png" width="50%" />


If you are using an older R version, please install the [newest R version](https://cran.rstudio.com/). 

#### 2) Install R Studio 

Go to the [RStudio website](https://www.rstudio.com/) and download the newest version if you are using an older version of RStudio (if in doubt, better update!). Simply follow the download instructions. The new version will be available next time you open RStudio. 


#### 3) Install necessary packages 

You need several R packages for the workshop. Please make sure to install these packages before the workshop. The easiest way to do so is by running this code in R:

```tpl
cran_packs <- c("learnr", "bookdown", "stargazer",
                "officer", "rticles", "webshot",
                "tidyverse", "remotes", "magick", 
                "kableExtra", "vtable", "devtools")
```

```tpl
install.packages(cran_packs, dependencies = TRUE)
```

```tpl
github_packs <- c('rstudio/blogdown',
                  'haozhu233/kableExtra', 'crsh/papaja')
```

```tpl
remotes::install_github(github_packs, dependencies = TRUE)
```

Once these packages are installed, you may use blogdown to install the Hugo package. Hugo is a static site generator that we will use to build blogdown paged. You may install Hugo using blogdown, like so: 

```tpl
blogdown::install_hugo()
```

You can check whether the installations were successful by running ```library(package_name)```. All installed packages must be loaded before we can use them during the workshop. 


<img src="images/library.png" width="50%" />

#### 4) Set up Git and GitHub


To make the most out of the workshop, I highly encourage you to install Git and to create a GitHub account for version control. 
Follow the instructions from the [Happy Git with R Book](https://happygitwithr.com/) and the official [GitHub guides](https://docs.github.com/en/get-started/quickstart/set-up-git): 


1. [Register a GitHub account](https://happygitwithr.com/github-acct.html)

2. [Install Git](https://docs.github.com/en/get-started/quickstart/set-up-git). Follow the instructions under **Setting up Git** (do not use the Desktop client). For **Windows Users**: Follow the installation instructions for Git [here](https://www.computerhope.com/issues/ch001927.htm). 

#### Once this is done, you are all set for the workshop! 🎉

#### 5) Sign up on osf


Many social scientists use osf to store their data or code. It is possible to integrate your GitHub repositories into osf.
Please [sign up on osf](https://osf.io/) before the workshop. 


#### 6) Install TeX

- Windows: [MikTeX](https://miktex.org/)
- Mac: [MacTeX](http://www.tug.org/mactex/)


# Slides 

#### [Day 1](https://anneokk.netlify.app/slides/day_one.html)


<iframe src="https://anneokk.netlify.app/slides/day_one.html#1" width="672" height="400px" data-external="1"></iframe>

 
#### [Day 2](https://anneokk.netlify.app/slides/day_two.html)


<iframe src="https://anneokk.netlify.app/slides/day_two.html#1" width="672" height="400px" data-external="1"></iframe>


# Schedule

#### 🗓️ Dates: 

24th & 25th May 2022


#### 🕛 Timetable for Day 1:

| Unit          | When          | What   |
|---------------|---------------|--------|
|                | 09:00-09:30   |🖐 WALK-IN and final installation support|
| Session #1  | 09:30-10:15   |**Introduction to R Markdown**|
|               | 10:15-10:30 |🍵 BREAK   |
| Session #2  | 10:30-11:15 |**R Markdown - Text, code, reference management**|
|               | 11:15-11:30 |🍵 BREAK   |
| Session #3  | 11:30-13:00   |**R Markdown - extended options and project organisation** |
|               | 13:00-13:40  |🍔 LUNCH BREAK |
| Session #4  | 13:40-15:00   |**R Markdown - building your own project** |


#### 🕛 Timetable for Day 2:

| Unit          | When          | What   |
|---------------|---------------|--------|
|                | 09:00-09:30   |❓ Q & A|
| Session #1  | 09:30-10:15   |**Version control with Git & GitHub - the basics**|
|               | 10:15-10:30 |🍵 BREAK   |
| Session #2  | 10:30-11:15 |**Version control with Git & GitHub - collaborating; Integration with osf**|
|               | 11:15-11:30 |🍵 BREAK   |
| Session #3  | 11:30-13:00   |**Blogdown - build your own project websites** |
|               | 13:00-13:40  |🍔 LUNCH BREAK |
| Session #4  | 13:40-15:00   |**Other R (Markdown) tools, final Q & A** |
