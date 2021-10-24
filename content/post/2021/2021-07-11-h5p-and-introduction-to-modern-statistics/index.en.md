---
title: "H5P and Introduction to Modern Statistics"
author: "Peter Baumgartner"
date: '2021-07-11'
slug: h5p-and-introduction-to-modern-statistics
categories: H5P
tags: ims
subtitle: ''
summary: ''
authors: []
lastmod: ''
bibliography: ../../../../static/media/references.bib
featured: no
commentable: yes
side_toc: yes
draft: no
image:
  placement: 2
  caption: ''
  alt_text: ''
  focal_point: Center
  preview_only: no
---

Three week ago I received via amazon [the paperback version of Introduction to Modern Statistics via Amazon](https://smile.amazon.de/Introduction-Modern-Statistics-Mine-%C3%87etinkaya-Rundel/dp/1943450145/). This is one of the rare exceptions where I need --- in addition to the online and/or ebook version --- the print edition as well. I didn't buy the textbook just for reading but for adding educational tools, especially to this book and generally for the overall [OpenIntro project](https://openintro.org/).

## How to integrate H5P exercises into statistics?

### 

My idea is to generate exercises with [H5P](https://h5p.org/) for statistics and/or data science courses applying R.

> H5P is a free and open-source content collaboration framework based on JavaScript. H5P is an abbreviation for HTML5 Package and aims to make it easy for everyone to create, share and reuse interactive HTML5 content. ([Wikipedia](https://en.wikipedia.org/w/index.php?title=H5P&oldid=1021454577))

I am convinced that the many sophisticated but easy-to-use H5P content types are an excellent choice to support textbooks with interactive exercises. Adding H5P exercises is especially valuable for those (predominantly theoretical) textbooks in statistics that are agnostic to a particular computing language.

But my opinion is not very relevant, as I am not teaching statistics or related subjects. My conviction is motivated by my general educational expertise but not by subject knowledge on statistics or data science. As for any educational design only a cooperation between domain and didactic expert results in valuable educational interactions.

But what about books using statistical software to apply theoretical knowledge?

This question is especially relevant with R as there are some R packages designed to generate R tutorials ([swirl](https://swirlstats.com/) and [learnr](https://rstudio.github.io/learnr/)). The motto here is: Learning statistics with R through R. In addition to these specialized packages there is also the widely used educational strategy to disseminate R Markdown files where textual guidance and R programming chunks are intermingled to form a kind of lab for statistical computing.

H5P exercises cannot replace these very practical and domain specific tutorials. At the moment I see three possible targets to add H5P exercises:

## Narrative Part

Exercises for the narrative part of statistics textbooks are often sparse. In ims-book there are the formatting vehicles of examples and guided practices.

### Examples

Examples will provide an understanding how methods should be applied. The textual answer (solution) follows the problem statement immediately, only separated by a line.

### Guided Practices

When reader should find the solution on their own they will be presented by a Guided Practice. A footnote provides the textual answer (solution).

With online-exercises there is no place restriction. One can provide not only a multitude of exercises but also use with different media. Besides text and graphic for exercises to the narrative part also animation and video are useful educational methods. Many different types of interactions are available (click, write, drag & drop, selection, ...) in different question formats (single choice, multiple choice, true/false, ...).

I am also a supporter of the old but time-proven concept of multiple representations (Ainsworth 1999; van Someren et al., n.d.): The same content is learned/experienced with several distinctive exercises. This approach is not redundant as each activity addresses the brain capacity in different ways.

I developed all exercises with self-detemined respecticvely self-directed learners in mind (Ryan and Deci 2018; Deci and Ryan 2008; Knowles 1975; Mezirow 1985). Learners should solve the task to their likening. I chose the educational settings toward the highest possible freedom supported by the software (H5P content type).

Learners can choose the order of the exercises, repeat them as often as they want, and even view the solution before they start with the activity. The idea behind this strategy of maximizing educational freedom is that adult self-learners don't want to fool themselves and are to respect in their self-organizing learning endeavor. There is one exception to the general rule of educational liberty: All activities under the sections Assessment have somewhat limited freedom so that learners could get some overall feedback about their performance.
