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
subtitle: ''
summary: ''
authors: []
lastmod: '2021-05-14T18:00:32+02:00'
featured: no
draft: no
side_toc: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

I have investigated the different methods for inserting images into various file formats and conversion procedures. The situation is complex and not easy to grasp. But on a meta-level, the case is pretty straightforward: The decision for a file format is much more important than the details in image handling.

1.  **`.Rmd`**: The window provided via Visual R Markdown provides all its great features only in .Rmd files. With the new page bundle feature in Hugo some disadvantages of .Rmd file disappear: As every file is in its own folder the several files produced by the conversion process do not hamper anymore. But .Rmd files loose some of the nice features of the Academic theme, e.g., the table of contents on the ride side. Also the chunk option `fig.align` does not work with the Academic theme. To date I could not find & solve the annoying problem.

2.  **`.Rmarkdown`**: It turns out that .Rmarkdown files have the greatest advantages. They have now almost the same features of R Markdown (writing and applying R code, using references and bibliography), but provides also the benefits of the (Academic) theme via the Goldmark renderer. Yes, you can't use the full functionality of the Visual R Markdown window for including images but you could use instead the Hugo figure shortcode.[^1]

So the situation is pretty straightforward: Hugo shortcodes are for all different file formats a good solution. In the case of .Rmd files they have to be embedded in an HTML-chunk.

[^1]: At the moment I do not know if using the `figure` shortcode results in some processing penalties. At least I read and experienced it myself that with many images the standard time-out parameter for Netlify has to be set much higher than the standard 10 seconds.
