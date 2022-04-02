---
title: 'Introduction to R for Social Scientists (I2RSS)'
author: Peter Baumgartner
date: '2022-04-02'
slug: book-review-introduction-to-r-for-social-scientists
categories:
  - data-science-education
  - review
tags:
  - r
subtitle: 'Book review'
summary: 'I was pleased finally to see a
new R introduction especially directed at social scientists. The book title "Introduction to R for Social Scientists: A Tidy
Programming Approach" (abbreviated I2RSS) was promising for me for two
reasons. Read the full book review.'
authors: [Peter Baumgartner]
lastmod: '2022-04-02'
bibliography:
  - ../../../../static/media/references.bib
featured: no
commentable: yes
side_toc: yes
draft: no
image:
  placement: 2
  caption: 'Book cover, CRC Press'
  alt_text: 'Book cover for "Introduction to R for Social Scientists"'
  focal_point: Center
  preview_only: no
---

# Acclamations for I2RSS

From my training (Ph.D. in sociology) but also from my different
professorship on educational sciences, I was pleased finally to see a
new R introduction especially directed at social scientists. The book
title "Introduction to R for Social Scientists: A Tidy Programming
Approach" (abbreviated I2RSS) was promising for me for two reasons.

## Authors experienced in political, social & dats science

The book is written by <a href="https://ryanpkennedy.weebly.com/">Ryan
Kennedy</a> and <a href="https://pdwaggoner.github.io/">Philip
Waggoner</a>, two prestigious scientists involved in political and
social research. Whereas Ryan has an astonishing career in political
science, is Philip exceptionally experienced at an academic level in
computational social science and data science. Philip is also a member
of
<a href="https://easystats.github.io/easystats/index.html">easystats</a>
(a software group that tends to an ecosystem of packages making
statistics in R easy).

## Promoting the modern tidyverse approach

The book features the <a href="<https://www.tidyverse.org/">tidyverse
approach</a> a modern collection of R packages that share an underlying
design philosophy, grammar, and data structures.

## Real data, results discussed and gentle dialog with reader

Without doubts, the book has several other merits: It uses real data
sets, e.g., from the
<a jref="https://electionstudies.org/data-center/anes-2016-pilot-study/">American
National Election Studies</a> (ANES) and teaches data management,
visualizations, exploratory data analysis (EDA), and statistical
modeling not in an abstract way, but also discusses the exciting results
with their data sets. It talks to the reader in a very sympathetic and
comforting way to master the (still very) steep learning curve for R
beginners.

# Some drawbacks and failures

But unfortunately, there are also two significant drawbacks to this
introduction:

## Educational inconsistencies

The book has several weaknesses from an educational point of view:

-   With some exceptions (data classes, data structures, and the map
    function from the <i>purrr</i> package is the chapter on "Essential
    programming," in my personal view to advanced for R beginners,
    especially for people from the social sciences with no programming
    background.
-   Comparing the same results with base R and tidyverse code may be
    interesting for intermediate users. Still, it is a waste of time and
    complicates things for beginners. It is also misusing the sparse
    place in the book, which has only 198 pages.
-   The book uses R scripts and does not feature Rmd files. This is
    strange as literary programming is an essential step for
    reproducibility, and RMarkdown also facilitates interactive use of
    the program code.
-   Sometimes, the results of the code chunks are missings (e.g.,
    graphs, tables, or reports). The explaining text under the code is,
    therefore, abstract. There are also some link errors, providing an
    URL starting with "www" where the referring webpage does not
    need/accept this addition.

These above weaknesses result in the deduction of one of the five stars.

## Not a role model for Open Science

The second star deduction is motivated by missing teaching modern
scientific behavior for early career researchers (ECRs). This
shortcoming includes the prominent use of R Markdown and the use of
collaboration and Open Science. I think that after the publication of <a
href="https://happygitwithr.com/">Happy Git</a>, there is no excuse
anymore to teach Git and GitHub (or similar systems) even for R
beginners. Another big mistake is not using the open-access politics of
the bookdown.org infrastructure for the online version of the book.

In the book, the authors promote the friendliness and importance of the
R community several times. They even mention that the book was initially
written with the help of the bookdown package (page 2). So why not
supply a role model for R beginners and young researchers?
