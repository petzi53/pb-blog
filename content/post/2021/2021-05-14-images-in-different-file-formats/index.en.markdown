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

<span class='Z3988' title='url_ver=Z39.88-2004&amp;ctx_ver=Z39.88-2004&amp;rfr_id=info%3Asid%2Fzotero.org%3A2&amp;rft_val_fmt=info%3Aofi%2Ffmt%3Akev%3Amtx%3Adc&amp;rft.type=blogPost&amp;rft.title=Images%20in%20Different%20File%20Formats&amp;rft.source=Thought%20splinters&amp;rft.rights=CC%20BY-SA%204.0&amp;rft.description=I%20have%20investigated%20the%20different%20methods%20for%20inserting%20images%20into%20various%20file%20formats%20and%20conversion%20procedures.%20The%20situation%20is%20complex%20and%20not%20easy%20to%20grasp.%20But%20on%20a%20meta-level,%20the%20case%20is%20pretty%20straightforward:%20The%20decision%20for%20a%20file%20format%20is%20much%20more%20important%20than%20the%20details%20in%20image%20handling.&amp;rft.identifier=https%3A%2F%2Fnotes.peter-baumgartner.net%2F2021%2F05%2F14%2Fimages-in-different-file-formats&amp;rft.aufirst=Peter&amp;rft.aulast=Baumgartner&amp;rft.au=Peter%20Baumgartner&amp;rft.date=2021-05-14&amp;rft.language=en'></span> 

[^1]: At the moment I do not know if using the `figure` shortcode results in some processing penalties. At least I read and experienced it myself that with many images the standard time-out parameter for Netlify has to be set much higher than the standard 10 seconds.
