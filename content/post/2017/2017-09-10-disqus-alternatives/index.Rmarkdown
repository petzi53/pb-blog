---
title: Alternatives for Disqus?
author: Peter Baumgartner
date: '2017-09-14'
categories:
  - web-service
  - review
tags:
  - disqus
lastmod: '2021-05-17'
slug: alternatives-for-disqus
draft: no
summary: Disqus is a top-rated service for hosting and managing comments. But it has as an external service several disadvantages which oppose the philosophy of static websites diametrically. I discuss some alternatives for integrating discussion fora with static websites.
# Featured image: https://wowchemy.com/docs/content/page-features/#page-resources-attachments-and-links
image:
  placement: 2
  caption: "[Screenshot from the Disqus website](https://disqus.com/)."
  alt_text: An optional description of the image for screen readers.
  focal_point: "Center"
  preview_only: false
---

[Disqus](https://disqus.com/) is a top-rated service for hosting and managing comments. But it has as an external service several disadvantages which opposed the philosophy of static websites diametrically. I discuss some alternatives for integrating discussion fora with static websites.

## Disqus has a long list of drawbacks

In [one of my tutorials](/2017/09/10/how-to-install-disqus-on-hugo/) I have explained how to integrate [Disqus](https://disqus.com/) into your static website. But in this article, I recommend looking for alternative comment services. Why this different standpoint? In the meanwhile, I read several articles questioning Disqus. Here is a list of critiques I found on the web (without ranking):

-   Disqus is slow and has a bad (re-)loading behavior.
-   Disqus is tracking many different things for different customers, some of them hidden and unknown.
-   Disqus does not allow `Markdown`.
-   Disqus does not allow anonymous content (IP address, email, and name are recorded).
-   Disqus is hosted in the USA, which is considered to have less strict privacy laws than Europe.
-   Disqus is not open source.
-   Disqus does not allow that users can use free licenses for their comments. It is not clear who has ownership of the comments.
-   Disqus is one central authority collecting all comments of your website visitors and users on *their* servers.

{{< figure src="images/DisqusLoadLogHigh-min.png" title="A graphic showing the request log with Disqus enabled" alt="A graphic showing the request log with Disqus enabled" id="request-log" caption="A typical request log with Disqus enabled: There are 105 network requests vs. 16 without Disqus. Load-time rises between 2 to 6 seconds." width="100%" numbered="true">}}

Especially the first and last bullet points defeat the advantages of a static website: Speed and *all* content always at your disposal. On a static website, data are just plain text files, saved locally on your hard disk. Therefore you can static sites transfer easily: Compress all your data in one zip file and unzip it where ever you want it. With Disqus, these advantages are not valid anymore because your blog text and its comments are hosted separately on different servers.

## What are alternatives for Disqus?

Summarizing the disadvantages, I mentioned above I am looking for a system which is

-   free
-   open source
-   and does not host the user-generated comments centrally

The [Hugo page on comments](https://gohugo.io/content-management/comments/#comments-alternatives) lists six available alternatives for comment on static websites[^1]. On [AlternativeTo](https://alternativeto.net/software/master-comments-system/) you will find 16 systems[^2].

## Cursory review on some services

### Staticman

{{< figure src="images/staticman-min.png" title="Screenshot of Staticman's website" alt="Screenshot of Staticman's website" id="staticman" caption="Screenshot of Staticman's website" width="100%" numbered="true">}}

[**Staticman**](https://staticman.net/) is open source and transforms user-generated content into data files to merge in your [GitHub](https://github.com/) repository, along with the rest of your content. This approach seems promising for me, but until now, I couldn't manage to install it. I have [reported my problem](https://github.com/eduardoboucas/staticman/issues/134), and I am currently waiting for help. As soon as I know how to fix it, I will review the system here on these pages.[^3]

<!--
**[txtpen](https://txtpen.com/)**: txtpen is proprietary software and collects data on its server. e.g., it does not qualify as a better alternative to Disqus. But txtpen is interesting for another reason: It is a service for commenting inline annotation, but not a good one. There are others with better interfaces and more widespread like the proprietary platform [diigo](https://www.diigo.com/) and especially the open source project [hypothes.is](https://web.hypothes.is/). 

<div class="alert alert-warning" role="alert">
<b>Update 2019-05-31:</b> The txtpen link does not work anymore.
</div>
-->

### hyothes.is

{{< figure src="images/hypothesis-min.png" title="Screenshot of hypothe.is' website" alt="Screenshot of hypothe.is' website" id="hypothes.is" caption="Screenshot of hypothe.is' website" width="100%" numbered="true">}}

[**hypothes.is**](https://web.hypothes.is/) wants to provide "a conversation layer over the entire web that works everywhere, without needing implementation by any underlying site". As far as I understand, for this approach, the data has to be stored centrally. So this software again is not an alternative to Disqus. This remark is not a critique of `hypothes.is` because it belongs to another category of software services. It has a new approach worth reviewing later in more detail.

### IntenseDebate

{{< figure src="images/intensedebate-min.png" title="Screenshot of IntenseDebate's website" alt="Screenshot of IntenseDebate's website" id="intensedebate" caption="Screenshot of IntenseDebate's website" width="100%" numbered="true">}}

[**IntenseDebate**](http://intensedebate.com/) is a feature-rich comment system for many blogging resp. CMS platforms. IntenseDebate is developed by the people who are behind many other well-known software services (e.g., WordPress.com, WooCommerce, Jetpack, Simplenote, VaultPress, Akismet, Gravatar, to name a few). It seems a bit odd that I could not find newer information on their blog than [January 2014](https://blog.intensedebate.com/)[^4]. It is [free but not open source](https://intensedebate.com/tos), but it hosts the content centrally in the US. IntenseDebate is, therefore, no candidate for replacing Disqus.

### Graphcomment

{{< figure src="images/graphcomment-min.png" title="Screenshot of Graphcomment's website" alt="Screenshot of Graphcomment's website" id="graphcomment" caption="Screenshot of Graphcomment's website" width="100%" numbered="true">}}

[**Graphcomment**](https://graphcomment.com/) is a beautifully designed commenting service with a (limited) free plan. But it is disqualified under my criteria as the code is not open source and it hosts the comments centrally too.

### MUUT

{{< figure src="images/muut-min.png" title="Screenshot of MUUT's website" alt="Screenshot of MUUT's website" id="muut" caption="Screenshot of MUUT's website" width="100%" numbered="true">}}

[**MUUT**](https://muut.com/) [does not allow pre-moderation](http://learn.muut.com/faq), e.g. every comment is online immediately. This is an interesting approach, but it is no alternative to Disqus: There is no free plan, and all rights of the user-generated content belong to MUUT!

### ISSO

{{< figure src="images/isso-min.png" title="Screenshot of ISSO's website" alt="Screenshot of ISSO's website" id="isso" caption="Screenshot of ISSO's website" width="100%" numbered="true">}}

[**ISSO**](https://posativ.org/isso/) is a lightweight commenting service, programmed in `Python`, which allows anonymous comments. It is free, open-source, and installed locally. So it does qualify! But the installation procedure seems complex as there is no GUI, and one has to use the terminal for the installation. Furthermore, it seems to me that not all operating systems are covered. But I should give it a try anyway and review it.

### Discourse

{{< figure src="images/discourse-min.png" title="Screenshot of Discourse's website" alt="Screenshot of Discourse's website" id="discourse" caption="Screenshot of Discourse's website" width="100%" numbered="true">}}

[**Discourse**](https://www.discourse.org/) is a feature-rich open-source environment, supports `Markdown` and allows anonymous posting. As a hosting service, it has no free plan and costs a minimum of US\$ 100 / month (with ~~80%~~ 85% discount for educational resp. 50% for non-profit institutions.). But you can install Discourse yourself without cost on your server. ~~Alternatively, you can pay a one-time fee of US\$99 for a cloud installation with a US\$10/month hosting fee.~~[^5] With the possibility to install it on your server, `Discourse` is another candidate to try out.

### Using GitHub ()

{{< figure src="images/don-williamson-min.png" title="Screenshot of Gazoo.vrv, Don Williamson's website" alt="Screenshot of Gazoo.vrv, Don Williamson's website" id="gazoo.vrv" caption="Screenshot of Gazoo.vrv, Don Williamson's website" width="100%" numbered="true">}}

[**Using GitHub**](http://donw.io/post/github-comments/): Another website is also recommending to use [GitHub](https://github.com/) for comments. I have no clear idea how these proposed code lines will work in practice, but if it works, then it will certainly qualify: Open source, free, supporting `Markdown` and hosted by the website owner.[^6]

## Summary

I reviewed superficially different commenting systems. I was looking for a free, open source system, allowing anonymous content, `Markdown` and hosted by the website owner. Four services seem to fulfill my criteria: `Staticman`, `ISSO`, `Discourse` and a code proposal by `Don Williamson`. `hypothes.is` is an exciting project, but not a commenting system. It belongs, therefore, to a different category of software (annotation systems).

A competent review of these four systems requires a test installation, which I plan to do in the next few weeks.[^7]

[^1]: Update 2021-05-18: There are now ten services listed.

[^2]: Update 2021-05-18: There are 29 services listed, but not all are open source, and some have already discontinued their service.

[^3]: Update 2021-05-18: Even with some help by the developer I couldn't manage to integrate it. Seems that my knowledge four years ago wasn't enough.

[^4]: Update: 2021-05-18: Their blog is not updated anymore, but the main website has recent information, as the footer with copyright 2021 demonstrates.

[^5]: Update 2021-05-18: I adapted the changes of plans.

[^6]: Update: 2021-05-18: Now - four years later - I understand this approach perfectly. There are, in the meanwhile, already a bunch of different services using GitHub. In the new version of this blog, I am using [utteranc.es](https://utteranc.es/) a lightweight comments widget built on GitHub issues.

[^7]: Update 2021-05-18: I have never done these test installations. But at least I have revised this old article. I am still planning to look into details at least of some of these commenting systems. I am using now utteranc.es, and the Academic theme of this blog provides [commento](https://commento.io/), another alternative to Disqus.
