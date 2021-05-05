---
title: Images in Different File Formats - a Comparison
author: Peter Baumgartner
date: '2021-05-02'
categories:
  - blogdown
tags:
  - Hugo
  - knitr
  - markdown
  - Pandoc
  - R Markdown
slug: images-in-different-formats
lastmod: '2021-05-02T21:41:30+02:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
---

## Experimental design

Today I have systematically experimented with images in different blogdown file formats: Rmd, R Markdown, md. I have inspected the possibilities and the resulting code.

I looked into:

-   `knitr`
-   'Insert Image' window via blogdown Addins
-   'Image ...' window vial Visual R Markdown
-   Hugo shortcode

## Results

| Tag     | .Rmd knitr | .Rmd Addin | .Rmd Visual | RMark knitr | Rmark Addin | Rmark Visual | .md shortc | .md Addin | .md Visual |
|---------|:----------:|:----------:|:-----------:|:-----------:|:-----------:|:------------:|:----------:|:---------:|:----------:|
| Caption |     ✅      |     ✅      |      ✅      |      ✅      |      ❌      |      ❌       |     ✅      |     ❌     |     ❌      |
| C. form |     ❌      |     ✅      |      ❌      |      ❌      |      ❌      |      ❌       |     ❌      |     ❌     |     ❌      |
| C.num   |     ✅      |     ❌      |      ❌      |      ✅      |      ❌      |      ❌       |     ❌      |     ❌     |     ❌      |
| Alt     |     ✅      |     ❌      |      ❌      |      ✅      |      ❌      |      ❌       |     ✅      |     ❌     |     ❌      |
| Title   |     ❌      |     ❌      |      ✅      |      ❌      |      ❌      |      ❌       |     ✅      |     ❌     |     ❌      |
| Tooltip |     ❌      |     ❌      |      ✅      |      ❌      |      ❌      |      ❌       |     ✅      |     ❌     |     ❌      |
| W / H   |     ✅      |     ✅      |      ✅      |      ✅      |      ✅      |      ✅       |     ✅      |     ✅     |     ✅      |
| Link to |     ❌      |     ❌      |      ✅      |      ❌      |      ❌      |      ✅       |     ✅      |     ❌     |     ❌      |
| ID      |     ✅      |     ❌      |      ✅      |      ✅      |      ❌      |      ❌       |     ✅      |     ❌     |     ❌      |
| HTML    |     ✅      |     ❌      |      ✅      |      ✅      |      ❌      |      ✅       |     ✅      |     ❌     |     ❌      |
| CSS     |     ✅      |     ❌      |      ✅      |      ✅      |      ❌      |      ✅       |     ✅      |     ❌     |     ❌      |
| Other   |     ❌      |     ❌      |      ✅      |      ❌      |      ❌      |      ✅       |     ✅      |     ❌     |     ❌      |
