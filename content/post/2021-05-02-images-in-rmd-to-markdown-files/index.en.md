---
title: Images in Rmd to markdown Files
author: Peter Baumgartner
date: '2021-05-02'
categories:
  - blogdown
tags:
  - Hugo
  - knitr
  - Pandoc
  - R Markdown
slug: images-in-rmd-to-markdown-files
lastmod: '2021-05-02T08:43:11+02:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no

summary: Testing different methods to include images form .Rmd to markdown files.
---

## Using r chunk with `knitr`

<div class="figure" style="text-align: center">
<img src="images/my-image.png" alt="Caption for this figure 1" width="100%" />
<p class="caption">Figure 1: Caption for this figure 1</p>
</div>

### Code in R Chunk

    ```
    {r img-with-knitr, echo=FALSE, fig.align='center', out.width='100%', fig.cap='Caption for this figure 1'}
    knitr::include_graphics("images/my-image.png")
    ```

### Code in HTML

    ```
    <div class="figure" style="text-align: center">
        <span id="fig:img-with-knitr"></span>
        <img src="images/my-image.png" alt="Caption for this figure 1" width="100%"/>
        <p class="caption">Figure 1: Caption for this figure 1</p>
    </div>

    ```

### CSS

    .figure {
            border: 1px;
            border-style: groove;
            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px  rgba(0, 0, 0, 0.19);
    }

    .figure .caption {
        text-align: center;
        margin-top: -0.5rem;
        margin-bottom: 0.5rem;
        font-size: smaller;
    }

### Summary

-   **Caption**: yes
-   **Format of caption**: no
-   **Caption automatically numbered**: yes
-   **Alt**: yes
-   **Title**: no
-   **Tooltip**: no
-   **Width/Height**: yes
-   **Link to**: no
-   **ID**: yes (format: "fig:\<chunk name\>)
-   **Classes**: yes (with `out.extra`, example: `out.extra='class="border shadowed"'`
-   **CSS style**: yes (with out.extra, example: `out.extra='style="background-color: #9ecff7; padding:10px; display: inline-block;"'` See blog post [Tips and tricks for working with images and figures in R Markdown documents](http://zevross.com/blog/2017/06/19/tips-and-tricks-for-working-with-images-and-figures-in-r-markdown-documents/)
-   **Other** (key=value): no

## Markdown via Addins 'Insert Image'

![**Figure 2:** Caption for this figure 2](images/my-image.png)

### Code in markdown

    ![**Figure 2:** Caption for this figure 2](images/my-image.png)

### Code in HTML

    <div class="figure">
    <img src="images/my-image.png" alt="">
    <p class="caption"><strong>Figure 2:</strong> Caption for this figure 1</p>
    </div>

### CSS

Because of classes figure and caption: Exactly the same as with Addins window.

### Summary

-   **Caption**: yes
-   **Format of caption**: yes
-   **Caption automatically numbered**: no
-   **Alt**: no
-   **Title**: no
-   **Tooltip**: no
-   **Width/Height**: yes
-   **Link to**: no
-   **ID**: no
-   **Classes**: no
-   **CSS style**: no
-   **Other** (key=value): no

## Visual R Markdown via Menu 'Insert ...'

![Figure 3: Caption for this figure 3](images/my-image.png "title text and tooltip"){#figure3}

### Code in markdown

    ![Figure 3: Caption for this figure 3](images/my-image.png "title text and tooltip"){#figure3}

### Code in HTML

    <div class="figure">
    <img src="images/my-image.png" title="title text and tooltip" id="figure2" alt="">
    <p class="caption">Figure 3: Caption for this figure 3</p>
    </div>

### CSS

Because of classes figure and caption: Exactly the same as with Addins window.

### Summary

-   **Caption**: yes
-   **Format of caption**: no
-   **Caption automatically numbered**: no
-   **Alt**: no
-   **Title**: yes
-   **Tooltip**: yes
-   **Width/Height**: yes
-   **Link to**: yes
-   **ID**: yes
-   **Classes**: yes
-   **CSS style**: yes
-   **Other** (key=value): yes

## Hugo figure shortcut

Not working for me: in contrast to [other blog entries](https://ropensci.org/blog/2020/04/23/rmd-learnings/), where a certain html comment preserves the syntax for Goldmark (or is it Blackfriday, and this is the reason why it is not working?).