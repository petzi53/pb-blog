---
title: Images in Different File Formats
author: Peter Baumgartner
date: '2021-05-14'
slug: images-in-different-file-formats
categories:
  - blogdown
tags:
  - Hugo
  - markdown
  - RStudio
subtitle: ''
authors: []
lastmod: ''
featured: no
draft: no
side_toc: no
image:
  position: 2
  caption: 'R Markdown has many outpout formats. [https://rmarkdown.rstudio.com/](https://rmarkdown.rstudio.com/)'
  focal_point: 'Center'
  preview_only: no
projects: []
summary: 'I have investigated the different methods for inserting images into various file formats and conversion procedures. The situation is complex and not easy to grasp. But on a meta-level, the case is pretty straightforward: The decision for a file format is much more important than the details in image handling.'
---

I have investigated the different methods for inserting images into various file formats and conversion procedures.

## Image handling in .Rmd, .md and .Rmarkdown files

-   At first I looked on the various options for [handling of images in .Rmd files](/2021/05/05/images-from-rmd-to-html-format/).
-   Then -- as a contrast program -- I tested the outcomes of [image handling procedures in .md files](/2021/05/06/images-in-md-files/).
-   And finally I investigated the [image procedures in.Rmarkdown files](/2021/05/07/images-in-rmarkdown-files/).

## Observed results

The situation is complex and not easy to grasp. But on a meta-level, the case is pretty straightforward: The decision for a file format is much more important than the details in image handling.

1.  **`.Rmd`**: The window provided via Visual R Markdown provides all its great features only in .Rmd files. With the new page bundle feature in Hugo some disadvantages of .Rmd file disappear: As every file is in its own folder the several files produced by the conversion process do not hamper anymore. But .Rmd files loose some of the nice features of the Academic theme, e.g., the table of contents on the ride side. Also the chunk option `fig.align` does not work with the Academic theme. To date I could not find & solve the annoying problem.

2.  **`.Rmarkdown`**: It turns out that **.Rmarkdown files have the greatest advantages**. They have now almost the same features of R Markdown (writing and applying R code, using references and bibliography), but provides also the benefits of the (Academic) theme via the Goldmark renderer. Yes, you can't use the full functionality of the Visual R Markdown window for including images but you could use instead the Hugo figure shortcode.[^1]

So the situation is pretty straightforward: The Hugo figure shortcode is for all different file formats a good solution. In the case of .Rmd files they have to be embedded in an HTML-chunk as [demonstrated in the .Rmd post](/2021/05/05/images-from-rmd-to-html-format#code-in-html-chunk).

## Additional tip

RStudio markdown snippet do not work in .md files. I do not understand why not. Ok, there is no R programming code but it coud be used for other (text) snippets. RStudio markdown snippet do work with .Rmarkdown files. So I have prepared an snippet to include the [Hugo figure shortcode](https://gohugo.io/content-management/shortcodes/#figure) syntax and saved under 'ff'. So I just need to type `ff + SHIFT-Tab` to get a template with all the parameters .

[^1]: At the moment I do not know if using the `figure` shortcode results in some processing penalties. At least I read and experienced it myself that with many images the standard time-out parameter for Netlify has to be set much higher than the standard 10 seconds.
