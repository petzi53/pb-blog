---
title: 'Blogdown tutorial (Part 1)'
author: Peter Baumgartner
date: '2017-09-04'
lastmod: '2021-05-19'
categories:
  - how-to
tags:
  - blogdown
  - installation
slug: blogdown-tutorial-part-1
summary: Part 1 of this tutorial explains how to install a Hugo theme on top of
  R, RStudio and blogdown. For this demonstration I will use the new (preview) version
  of RStudio as it facilitates the installation of Hugo and a theme.
image:
  placement: 2
---

{{% callout note %}} Update 2021-05-19: Even if some screenshots might have changed slightly, this part of the tutorial is -- with one exception ([header 4](#4-create-a-website-using-hugo-and-blogdown)) -- still up to date. But there are now many other resources with the same content available.

Especially I would like to recommend [Up & running with blogdown in 2021](https://alison.rbind.io/post/new-year-new-blogdown/) by Allison Hill, co-author of the [blogdown book](https://bookdown.org/yihui/blogdown/). {{% /callout %}}

In this tutorial I will show how to install the R package `blogdown` with the help of the new version of RStudio and how to link your local blogdown-directory to a remote repository on GitHub. But before we actually start with the installation procedure let us define the different ingredients (tools) we are going to use:

## Tools we are going to use

1.  [Blogdown](https://bookdown.org/yihui/blogdown/) is an R package for creating static websites with R Markdown.
2.  [R](https://www.r-project.org/about.html) is an integrated suite of open source software facilities for statistical computing and includes tools for data manipulation, calculation and graphical display.
3.  [RStudio](https://www.rstudio.com/) is an integrated development environment (IDE) which sits on top of R and facilitates the use of R tremendously.
4.  [R Markdown](http://rmarkdown.rstudio.com/) is a file format for making dynamic documents with R. It is based on Markdown (a lightweight markup language with plain text formatting syntax), but it also can contain chunks of embedded R code.
5.  [Hugo](https://gohugo.io/) is a popular open-source static website generator.
6.  [hugo-academic](https://themes.gohugo.io/academic/) is a theme designed for Hugo to create an academic or personal website. Besides special academic features like sections for publications, projects, teaching it also includes a blog section and supports multilingual usage.
7.  [GitHub](https://github.com/) is an Internet hosting service for distributed version control repositories. Is is mainly used for source code management, but it works also with plain text markup languages. GitHub offers all the functionality of Git as well adding its own features.
8.  [Git](https://git-scm.com/) is a distributed version control system for tracking changes in computer files and coordinating work on those files among multiple people.

All these tools are open source and free available.

## Preliminary preparations: Installing R and RStudio

There are many tutorials to install R and RStudio. See for instance the video [Installing R and RStudio](https://www.youtube.com/watch?v=cX532N_XLIs). But at the moment the new version of RStudio which facilitates the installation procedure of blogdown is still not released as standard version. But you can use all these new features by [downloading the preview release](https://www.rstudio.com/products/rstudio/download/preview/). As these features will be soon the standard version of RStudio I will explain the installation procedure using this upcoming version.[^1]

## Create a blogdown website

### Create a new project

After installing RStudio version greater than v.1.1.28 open the project menu and choose "New Project". {{< figure src="images/create-new-project.png" title="Create a new project" numbered="true" >}}

### Create a new directory

A new window opens up: We are going to create a new local directory for our static blogdown website. Choose "New directory". {{< figure src="images/create-new-directory.png" title="Create a new directory" numbered="true" >}}

### Create a website using blogdown

The selection in the following window is self-explaining: "Website using blogdown". Here it is the last line in the window. But in the future there may added other project types, so that you have to scroll down to see the blogdown-choice.{{< figure src="images/create-website-using-blogdown.png" title="Create a website using blogdown" numbered="true" >}}

### Create a website using Hugo and blogdown

{{% callout warning %}} Update 2021-05-19: The Academic theme is now modularized into [different specialized templates](https://wowchemy.com/templates/) and integrated into the development of the [web builder software wowchemy](https://wowchemy.com/). To get the complete Academic theme, you have now to write into the Hugo theme field "wowchemy/starter-academic" (instead of "gcushen/hugo-academic"). {{% /callout %}}

Lastly we arrive at the final window we have to answer. Here you can choose the name and location of your local directory which will eventually collect all files of your static website. I recommend to leave all check boxes ticked, as this default value will give you the most support to generate the new website. The program for the static website generator Hugo will be installed automatically as well as sample blog posts will be added. Especially important is the possibility to look into the example site of the theme, because this will provide you with clues about the functionality of the theme. {{< figure src="images/create-website-using-hugo-and-blogdown.png" title="Create a website using Hugo and blogdown" numbered="true" >}}

### Choose theme

I have chosen the hugo-academic theme. You can pick your own preferred webdesign via the [Hugo Themes](https://themes.gohugo.io/) page. {{< figure src="images/hugo-themes.png" title="Huge variety of Hugo themes to choose from. " numbered="true" >}}

### Choose Academic (now Wowchemy)

In the "Hugo theme" field you have to insert the URL of the GitHub repository of the theme you would like to use. You will see the address when you click at the thumbnail of the theme and hover your cursor over the "Download"-button. {{< figure src="images/academic-theme.png" title="hugo-academic is as special theme for personal websites in academia. " numbered="true" >}}

### GitHub repor of Academic theme

Clicking on the download button will bring up the developer's repository. This is useful even for beginner as you can have a look of the ongoing discussion under the "issue" tab or to ask your own questions. Experienced users can fork the repository in order to adapt the functionality of the theme and/or to suggest code changes to the developer via the push mechanism. {{< figure src="images/github-gcushen-hugo-academic.png" title="GitHub code repository of the hugo-academic theme. " numbered="true" >}}

### Create project

When you finally click the "Create Project" button you have to wait few seconds until the selected theme is downloaded and Hugo installed. After the installation is finished RStudio opens up a four pane view. We will go more into the details of these different windows in the third part of this tutorial. {{< figure src="images/four-pane-view-after-installation.png" title="RStudio's four pane view immediately after installation. " numbered="true" >}}

## Summary

We have successfully installed the hugo-academic theme in a version controlled local directory. Essentially we could now start to personalize the website and/or write articles resp. posts. But we will continue the installation process with creating a remote GitHub repository which has to be linked to the just created local repository. The remote repository not only operates as backup and as distributed version control (allowing collaboration) but also enables -- beside a manual transfer via ftp -- additional ways of publishing your website. We will cover these possibilities in the following parts of this tutorial.

Go and visit the second part [Creating a GitHub Repository](/2017/09/05/blogdown-tutorial-part-2/) of this tutorial.

<span class='Z3988' title='url_ver=Z39.88-2004&amp;ctx_ver=Z39.88-2004&amp;rfr_id=info%3Asid%2Fzotero.org%3A2&amp;rft_val_fmt=info%3Aofi%2Ffmt%3Akev%3Amtx%3Adc&amp;rft.type=blogPost&amp;rft.title=Blogdown%20tutorial%20(Part%201)&amp;rft.source=Thought%20splinters&amp;rft.rights=CC%20BY-SA%204.0&amp;rft.description=Part%201%20of%20this%20tutorial%20explains%20how%20to%20install%20a%20Hugo%20theme%20on%20top%20of%20R,%20RStudio%20and%20blogdown.%20For%20this%20demonstration%20I%20will%20use%20the%20new%20(preview)%20version%20of%20RStudio%20as%20it%20facilitates%20the%20installation%20of%20Hugo%20and%20a%20theme.&amp;rft.identifier=https%3A%2F%2Fnotes.peter-baumgartner.net%2F2017%2F09%2F04%2Fblogdown-tutorial-part-1&amp;rft.aufirst=Peter&amp;rft.aulast=Baumgartner&amp;rft.au=Peter%20Baumgartner&amp;rft.date=2017-09-04&amp;rft.language=en'></span>

[^1]: To use features supporting blogdown websites the RStudio version has to be higher than v1.1.28: As today (2017-09-04) the actual preview version is v1.1.353.
