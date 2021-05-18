---
title: 'What is obvious, and for whom?'
author: Peter Baumgartner
date: '2017-10-17'
lastmod: '2021-05-18'
categories:
  - reflection
  - teaching strategies
  - philosophy
tags:
  - bookdown
  - complexity
  - hierarchy
  - mental model
  - multiple representations
slug: what-is-obvious-and-for-whom
summary: 'Inspired by a blog post by Yihui Xie, I reflect in this post about communications difficulties between experts (e.g., software engineers) and laypersons (users). Starting position is my fault in providing the complete and correct information when filing issues about bookdown and blogdown. Be aware: This is a somewhat theoretical/philosophical discussion.'
draft: no
bibliography: ["../../../../static/media/references.bib"]
image:
    placement: 2   
    caption: "[Everything is obvious: Wallpaper](https://www.wallpaperflare.com/)"
    alt_text: "Black background with white inscription: 'Everything is obvious'"
    focal_point: "Center"
    preview_only: false
---

In the last few weeks, I tried to work with [bookdown](https://bookdown.org/yihui/bookdown/), an R package developed by Yihui Xie. This program is/was for me much harder to understand, unlike [blogdown](https://bookdown.org/yihui/blogdown/) by the same author. In blogdown, I could even – after some initial problems – write a tutorial which even [the developer applauded](https://yihui.name/en/2017/10/bloggers-vs-book-authors/) :sweat\_smile:.

But with bookdown, it was different: Not only that I misunderstood some program functions but more importantly, I could not adequately report my problems in one case, [I did not communicate vital information](https://github.com/rstudio/bookdown/issues/474) in the other case [I did not look at the right place](https://stackoverflow.com/questions/46742700/is-it-possible-to-change-to-documentclass-scrbook-in-bookdown) where my question was explicitly addressed. It is not a surprise that Yihui Xie got angry with me and even wrote a [blog post about the incident](https://yihui.name/en/2017/10/not-obvious/). He gave me the advice:

## Please do not make these assumptions when filing issues

<div class="alert alert-info" role="alert">

Be aware: This is a somewhat theoretical/philosophical discussion.

</div>

For me, as a professional educator, this is a fundamental question. Where to start with explanations and where to stop? Should I provide just the information to solve the problem, or should I give some background information? What kind of advice should I give to prevent similar issues in the future? These are examples of questions I have to consider as a teacher all the time. But this time, I am on the other side of this communication exchange - I am the learner and student, and I am the one who has to ask the expert.

Yihui Xie is not blaming me as a user, as he wrote in his last paragraph of the mentioned blog post. You can see his positive attitude in the post on [The Minimal Reproducible Example Paradox](https://yihui.name/en/2017/09/the-minimal-reprex-paradox/) where he is complaining that many users do not provide a minimal reproducible example or do not know how to produce one. He comes to a somewhat depressing conclusion:

> How many times have I reminded a user of posting a minimal, self-contained, and reproducible example (*reprex*)? Probably 500 times. How many times do I think I will still need to remind users of this? Perhaps 5000 times.

But again: This is a typical situation we have in education as well. We are explaining the same thing over and over *but* — to *different* people, students, learners, classes, etc. Even if we explicitly mention common errors and misunderstandings, some learners will always commit these mistakes. When we describe operations you should *not* undertake, you can be sure there are one or two who will follow precisely these wrong paths.

## Tacit knowledge and language games

So what? Are people dumb? Do they deliberately ignore advice? I don’t think so, but instead, there is a gap which cannot be overcome only with linguistic means. It is also a question of transferring *tacit knowledge’* to use a notion introduced by Michael Polanyi:

> I shall reconsider human knowledge by starting from the fact that {{&lt; hl &gt;}}we know more than we can tell{{&lt; /hl &gt;}}.(Polanyi 2009)

Many philosophers (e.g., Søren Kirkegaard, Ludwig Wittgenstein, Gregory Bateson, Susan Langer, Jürgen Habermas, Nelson Goodman, to name a few) have reflected about the limitation of linguistic expressions. Wittgenstein, for example, has pointed out that we cannot explain the meaning of every word or sentence because we have to use language with other words and sentences. It is an endless regress that we cannot solve with language alone. We have to share a common ground, and we have to know how “to play the language game.” Following some quotes to give you a flavor of the argument:

> One has already to know (or be able to do) something to be capable of asking a thing’s name. But what does one have to know? ([Philosophical Investigations 30](http://www.postmoderntherapy.com:80/Wittgenstein/lw21-30c.htm)) … When one shows someone the king in chess and says: “This is the king,” this does not tell him the use of this piece-unless he already knows the rules of the game up to this last point. ([31](http://www.postmoderntherapy.com:80/Wittgenstein/lw31-38c.htm)) … Someone coming into a strange country will sometimes learn the language of the inhabitants from ostensive definitions that they give him; and he will often have to ‘guess’ the meaning of these definitions; and will guess sometimes right, sometimes wrong. (Wittgenstein 1961)

To use a famous philosophical example (Quine 1960): If I point to a white rabbit and say in my foreign language, “Gavagai!” you have to guess the meaning. Do I say, “There is a rabbit!” or “Look at the nice white color!” So even an ostensive definition is under-determined and does not help to choose the right interpretation and to solve the ambiguity of meaning in our speech acts.

One proposal which could serve as an avenue of escape for this gap or paradox is to invent a special kind of notational system. Common examples to demonstrate this strategy is chess notation or musical notation. I believe that a minimal reproductive example or to deliver the `sessionInfo()` is also a kind of notational system. But the problem is the same: One has to learn this (new) language to use it correctly.

## Many different layers

The malice of the situation is the assumption that from the fact that we are using the same (English) words and sentences that we communicate the same meaning and understand to each other. The expert believes that (s)he has expressed every necessary information and so the novice in asking a question. – And this is mostly correct – from his/her point of view or understanding.[^1]

I have reflected why for me, using bookdown was so much more complicated than blogdown. I started several months ago with `bookdown`, but I gave up and started another trial *after* I had some success with `blogdown`. This sequence seems weird as it appears that for Yihui Xie, the situation was inverse.[^2]

I think there are different reasons:

1.  Blogdown was written together with [Amber Thomas](https://proquestionasker.github.io/) and [Alison Presmanes Hill](https://apreshill.rbind.io/). It was an excellent inventive and successful strategy to integrate authors who can provide the perspective of the user side. In the blogdown book, there are some beneficial chapters about action strategies. They give, on the one hand, practical tips and contain, on the other hand, some (technical) simplification. We, educationalists, call this method “pedagogical reduction”). I refer to chapters like [A quick example](https://bookdown.org/yihui/blogdown/a-quick-example.html) or [A recommended workflow](https://bookdown.org/yihui/blogdown/workflow.html).

2.  The success in working with blogdown is more straight and comes in smaller bits and pieces. You write a sentence with Markdown in your blog, and you can see the result immediately. It seems - at least for laypeople like me - that in blogdown, there are not so many hidden conversion processes as this appears to be the case in bookdown. Bookdown, by definition, provides the means for cross-media publishing resulting in three different products (website, PDF, and ePub), all three with their underlying structure and rules.

## The importance of mental models

But there is one common point why both blogdown and bookdown are intrinsically difficult to understand for novices: Many different layers of software are working together to produce the result. I am not sure if I am even able to enumerate these different layers correctly: There is

-   the used hardware,

-   the operating system,

-   R with all its various packages,

-   the programming and writing environment RStudio,

-   Rmarkdown using pandoc,

-   knitr,

-   blogdown or bookdown,

-   the used theme,

-   with needs for adoption CSS knowledge,

-   git and GitHub,

-   and last but not least, Netlify.

All of these different tools work on top of each other and/or together. And all of these different levels have their complexities, laws, functions, manuals, commands, etc.

As long as everything works fine, there is no need to understand the different parts and their interaction and/or synergy. But when something breaks down, then a shift of focus occurs, or as Heidegger says, the worldliness becomes obvious, changing tool usage from “ready-to-hand” to “present-at-hand”(Heidegger 2008). In “ready-to-hand” awareness, you are using tools to fulfill their purpose (to write a blog post); in a breakdown (= “ready-to-hand” awareness), you get consciousness of the complexities inside your tools machinery.[^3]

But here comes now the problem: As users, we are only experts in “ready-to-hand” awareness, and we have no clue about the functionality inside the black box. We can only report some weird behavior about some experienced phenomenon from the “ready-to-hand” perspective. We, laypersons, have constructed a mental model about the functionality of our tools, and we are reporting about the problems with the underlying implicit assumptions of our mental model. The mental model functions as a world view: We see all the different objects, people, etc., under a particular perspective guided by our underlying tacit assumptions.

After the breakdown, we should question our mental model, but this is very difficult: Our worldview has worked successfully so far. One will not change the world view with just one different fact. The same happens with scientific theories: One other point is a challenge to elaborate on the theory, improve it, and incorporate the anomaly into the argument. Maybe the problem lies in the reluctant fact itself (e.g., the software has a bug, or the author misreported the effect).

## Lesson learned

So what the fuss with all these abstract ideas? Where is the practical impact of all these considerations? — I make the case in this article that we should focus separately on two different kinds of explanations:

1.  On the one hand, we users need “ready-to-hand” reasons which are easy to follow even if they are simplified and do not cover all eventualities. We need guidelines, step-by-step (video)-tutorials, etc. Are there shortcuts, tips, and rules of thumb one could follow? And we would need tons of examples! But people who provide this kind of explanation should be aware: This explanation *always* is under-determined and cannot prevent misunderstandings. Lacking the necessary knowledge, we still have to interpret what “Gavagai!” means.

2.  On the other hand, we users need at the same time “present-to-hand” explanations to build up correct mental models of the inherent complexities and functionalities of the tools. Which software components rely on which other parts? What is the task of component X, and how is it related to the ready-to-hand functionality? But people who provide this kind of explanation should be aware: This level of explication is not a technical one, not directed to other experts. (This is another critical third level of description and documentation, one I will not cover here in this article). So we would need individual formats like diagrams of the interconnectedness and synergistic effects. The result is a kind of *multiple representations* and would provide additional access to discover the functionality of different parts of the software machinery.[^4]

3.  A piece of advice like “Please do not make this assumption when filing issues.” are basic ethical guidelines but not very practical and helpful. We are *always* using (implicit) assumptions. In stating one proposition, we rely on a set of different assumptions; otherwise, we could not use language and construct meaningful sentences. The problem is to know *what assumptions are to test and what assumptions are to rely on.*[^5]

There is no possibility to examine all belief systems at the same time. The whole book “On Certainty” by Ludwig Wittgenstein Wittgenstein (1975) is full of aphorisms about tacit assumptions we rely on. Our knowledge does not consist of separated propositions but is a system of interconnected views/opinions. I will close this post with some quotes by Wittgenstein to illustrate this point.

> §139. Not only rules, but also examples are needed for establishing a practice. Our rules leave loop-holes open, and the practice has to speak for itself."

> §142. It is not single axioms that strike me as obvious, it is a system in which consequences and premises give one another *mutual* support.

> §144. The child learns to believe a host of things. I.e. it learns to act according to these beliefs. Bit by bit there forms a system of what is believed, and in that system some things stand unshakeably fast and some are more or less liable to shift. What stands fast does so, not because it is intrinsically obvious or convincing; it is instead held fast by what lies around it.[^6]

[StackOverflow](https://stackoverflow.com/) for instance, is very, very good for “ready-to-hand” explanations but does - as far as I know - a lousy job for building up mental models. Discussions about different but similar software packages, their advantages and disadvantages are forbidden.[^7]

## References

<span class='Z3988' title='url_ver=Z39.88-2004&amp;ctx_ver=Z39.88-2004&amp;rfr_id=info%3Asid%2Fzotero.org%3A2&amp;rft_val_fmt=info%3Aofi%2Ffmt%3Akev%3Amtx%3Adc&amp;rft.type=blogPost&amp;rft.title=What%20is%20obvious,%20and%20for%20whom?&amp;rft.source=Thought%20splinters&amp;rft.rights=CC%20BY-SA%204.0&amp;rft.description=Inspired%20by%20a%20blog%20post%20by%20Yihui%20Xie,%20I%20reflect%20in%20this%20post%20about%20communications%20difficulties%20between%20experts%20(e.g.,%20software%20engineers)%20and%20laypersons%20(users).%20Starting%20position%20is%20my%20fault%20in%20providing%20the%20complete%20and%20correct%20information%20when%20filing%20issues%20about%20bookdown%20and%20blogdown.%20Be%20aware:%20This%20is%20a%20somewhat%20theoretical/philosophical%20discussion.&amp;rft.identifier=https%3A%2F%2Fnotes.peter-baumgartner.net%2F2017%2F10%2F17%2Fwhat-is-obvious-and-for-whom&amp;rft.aufirst=Peter&amp;rft.aulast=Baumgartner&amp;rft.au=Peter%20Baumgartner&amp;rft.date=2017-10-17&amp;rft.language=en'></span> 

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-heidegger2008" class="csl-entry">

Heidegger, Martin. 2008. *Being and Time*. Reprint. New York: Harper Perennial Modern Classics.

</div>

<div id="ref-polanyi2009" class="csl-entry">

Polanyi, Michael. 2009. *The Tacit Dimension*. University of Chicago Press.

</div>

<div id="ref-quine1960" class="csl-entry">

Quine, Willard Van Orman. 1960. *Word and Object*. The Mit Press.

</div>

<div id="ref-wittgenstein1961" class="csl-entry">

Wittgenstein, Ludwig. 1961. *Philosophical investigations*. New York: Macmillan.

</div>

<div id="ref-wittgenstein1975" class="csl-entry">

———. 1975. *On Certainty*. Revised ed. Oxford: John Wiley; Sons Ltd.

</div>

</div>

[^1]: I could tell some jokes about misunderstandings between Germans and Austrians, both using German as their native language.

[^2]: He said that blogdown was especially complicated to develop, but I cannot find the place at the moment to quote it correctly.

[^3]: For an understandable description of the philosophical concept of ‘breakdown’ read this [example on Human-Computer Interaction](https://www.interaction-design.org/literature/book/the-glossary-of-human-computer-interaction/breakdowns)

[^4]: An essential step for me in understanding the complex template structure of Hugo was to write in every template the sentence: “This here is the template <name of the file>” and to see what happens in different situations

[^5]: BTW: This is the same conclusion as Yihui Xie has drawn: “To clarify, I’m not blaming this user. I can totally understand it. Many users do the same thing. The problem is that there are so many possibilities for software to screw up, so you have to describe everything clearly to eliminate as many possibilities as possible.”— So we do have the same analysis. Still, I propose (in addition to reflect and report all hidden assumptions) another new long-term strategy (namely helping to build up correct mental models about the complex software dependencies) to prevent similar faults as I have committed.

[^6]: To prevent a possible misunderstanding: I do not think that only or even predominantly software engineers are responsible for the two mentioned explanation levels. Their expertise is to develop programs, document them, and resolve bugs. I just want to point out that there should be more focus on these two levels and that more people should be concerned about providing information on these two levels.

[^7]: At least this is \*my\* mental model from [StackOverflow](https://stackoverflow.com/) For instance, the moderator closed my question about the difference between [packrat](https://rstudio.github.io/packrat/) and [checkpoint](https://cran.r-project.org/web/packages/checkpoint/index.html) as off-topic.
