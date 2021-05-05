---
title: Images in .md Files
author: Peter Baumgartner
date: '2021-05-02'
categories:
  - blogdown
tags:
  - Hugo
  - knitr
  - Pandoc
  - R Markdown
slug: images-in-md-files
lastmod: '2021-05-02T08:43:11+02:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no

summary: Testing different methods to include images in .md files.
---

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

    .figure, figure {
            border: 1px;
            border-style: groove;
            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px  rgba(0, 0, 0, 0.19);
    }

    .caption {
        text-align: center;
        margin-top: -0.5rem;
        margin-bottom: 0.5rem;
        font-size: smaller;
    }

    figcaption {
    text-align: center;
    padding-top: 1.5rem;
    font-size: smaller;

}

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

![Figure 3: Caption for this figure 3](images/my-image.png "title text and tooltip"){\#figure3}

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

{{< figure src="images/my-image.png" class="center" alt="my-alt text" caption="Figure 4: my title-text" >}}
