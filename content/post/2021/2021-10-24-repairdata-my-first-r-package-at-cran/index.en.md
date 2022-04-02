---
title: repairData - My First R Package at CRAN
author: Peter Baumgartner
date: '2021-10-24'
slug: repairdata-my-first-r-package
categories:
  - package
  - open-data
  - data science
tags:
  - repair café
subtitle: ''
summary: ''
authors: [Peter Baumgartner]
lastmod: ''
bibliography:
  - ../../../../static/media/references.bib
featured: no
commentable: yes
side_toc: yes
draft: no
image:
  placement: 2
  caption: 'Photo by energepic.com from Pexels'
  alt_text: 'Different tools (hammer, screwdriver, plier, measuring tape, wall plugs, dowels) jumbled at a dirty floor.'
  focal_point: Center
  preview_only: no
output:
  blogdown::html_page:
    fig_caption: true
    toc: true
    toc_depth: 4
---

## R Packages book as a valuable assistance

I am pleased: [`repairData` is on
CRAN](https://cran.r-project.org/web/packages/repairData/index.html)
(The Comprehensive R Archive Network!
[`repairData`](https://petzi53.github.io/repairData/) is my first
package; offers only five data sets and is therefore not a brilliant
feat. The real achievement for me was that I successfully completed the
complex submission process for the first time. Without [R
Packages](https://r-pkgs.org/), the still not finished but already
publicly accessible 2nd edition by [Hadley Wickham](http://hadley.nz/)
and [Jenny Bryan](https://jennybryan.org/), I wouldn't have succeeded --
at least not relatively easy on my second trial.

{{< figure src="images/cover-r-packages-min.png" id="r-packages" alt="Book Cover of 'R Packages'" title="Book Cover of 'R Packages'" caption="Book Cover of 'R Packages'" width="70%" numbered="true">}}

## Goal of the datasets

`repairData` offers the dataset of the [Open Repair
Alliance](https://openrepair.org/) (ORA), from February 21, 2021. The
data set corresponds to the [Open Repair Data
Standards](https://standard.openrepair.org/) (ORDS) developed by the ORA
in its last version, 0.2.1.

Data from five providers can currently [downloaded
separately](https://openrepair.org/open-data/downloads/) from the Open
Repair Alliance (ORA) website. When I developed repairData, I thought
that it would be an advantage for users if they had the data already
aggregated and available. Users can separate the different databases
again via the "Data provider ID" category.

On the [GitHub repository of the Open Repair
Alliance](https://github.com/openrepair/data), I also found four other
data sets on
[batteries](https://github.com/openrepair/data/tree/master/quests/batteries),
[printers](https://github.com/openrepair/data/tree/master/quests/printers),
[smartphones](https://github.com/openrepair/data/tree/master/quests/mobiles),
and
[tablets](https://github.com/openrepair/data/tree/master/quests/tablets).
Data sets with the corresponding categories were extracted from the
database and examined separately as part of a concerted online campaign.

The main aim of these excerpts is to find out the causes of the defects
and what obstacles arose during the repair. At the repair events, there
is usually not enough time to investigate such more targeted questions.
In principle, these database extracts differ from the primary data
record only by an additional column to categorize the errors.

The goal of the various initiatives in the ORA is to collect repair data
in a standardized manner and make them publicly available. The dataset
should provide evidence of shortcomings in our affluent society: Planned
obsolescence, wasted energy, filigree construction, and limited access
to repairs. The collected data should help build up pressure against
companies and the government for changes in production and regulations.

## Five data providers

The five organizations of the ORA are:

### Repair Café International

The Dutch journalist [Martine
Postma](https://en.wikipedia.org/wiki/Martine_Postma) started the Repair
Café movement by establishing the first Repair Café on October 18, 2009,
in Amsterdam. On March 2, 2010, the [Repair Café
International](https://repaircafe.org/) Foundation was founded as an
umbrella organization based in Amsterdam. There are now 2196 members
(Repair Cafés) in this network worldwide. 23,048 data sets, almost half
of all data, come from this network alone.

{{< figure src="images/repair-cafe-wide-min.png" id="repair-cafe-map" alt="Google map with repair cafés" title="Google map with global distribution of 2.196 repair cafés (October 23, 2021)." caption="Google map with global distribution of 2.196 repair cafés (October 23, 2021)." width="100%" numbered="true">}}

Community repair data is collected for the Repair Café International
foundation via the RepairMonitor platform. The
[RepairMonitor](https://repairmonitor.org/en/node/61) is the online tool
for collecting and sharing repair data. The Repair Café International
website has an excellent [2-minute
video](https://www.youtube.com/watch?v=WP24o2FEmvA) that explains repair
customers' processes in the repair cafés.

### anstiftung

[anstiftung](https://anstiftung.de/) is a non-profit foundation based in
Munich that, in addition to repair initiatives, also promotes other
movements to revitalize neighborhoods or interventions in public spaces,
such as intercultural and urban gardens, open workshops, and open source
projects.

anstiftung is also active as a funding company. It researches,
publishes, and organizes the independent German network of over 1,000
repair initiatives. Repair cafés are held online continuously (weekly!)

{{< figure src="images/anstiftung-pictures-min.png" id="anstiftung-pictures" alt="Collection of different posters for anstiftung events." title="Collection of different posters for anstiftung events." caption="Collection of different posters for anstiftung events." width="100%" numbered="true">}}

The community repair data will be collected in the [repair initiatives
platform](https://www.reparatur-initiativen.de/) from June 2018 (see the
[repo on GitHub](https://github.com/anstiftung/mapped-repair-events)).
anstiftung has 4,798 records to the collective database contributed so
far.

{{< figure src="images/reparatur-initiativen-min.png" id="anstiftung-reparatur-initiativen" alt="Screenshot of startpage of the reparatur-initiativen network." title="Screenshot of startpage of the reparatur-initiativen network." caption="Screenshot of startpage of the reparatur-initiativen network." width="100%" numbered="true">}}

### Fixit Clinic

[Fixit Clinic](https://fixitclinic.blogspot.com/) is a US initiative
that "got out of hand as a hobby" (founder [Peter
Mui](https://%20www.youtube.com/watch?v=qJtNrsgtAs0) in a YouTube video
(00: 21-00: 24)). Fixit Clinic is a "pop-up" activity where people take
their broken things apart. The Fixit Clinic provides coaches who guide
the participants through the repair process and provide the special
tools for the repair.

In addition, Fixit Clinic is known worldwide for its [ifixit
website](https://www.ifixit.com/), which provides "repair instructions
for everything, written by everyone". The website is an extensive
collection of advice and community forums in several languages ​​and
offers an online shop for repair tools.

{{< figure src="images/fixit-website-min.png" id="fixit-websites" alt="Screenshot of fixit website." title="Screenshot of fixit website." caption="Screenshot of fixit website." width="100%" numbered="true">}}

The data is collected using the [Broken Item
Report](https://fixitclinic.blogspot.com/p/item-re.html) form as part of
the Fixit Clinic's community repair events. In addition to the usual
information (article, brand, model, year of construction, problem), [the
form](https://goo.gl/qhpUkR) also asks other questions about the
defective device, such as information on the exchange of repair
experience, the status of the spare parts, and what experiences there
were with the support of the manufacturer. The form is a kind of
"routing slip" with a constantly updated status report on the item. Both
-- successful and unsuccessful --repair attempts at the events are
entered. Even the owners document their experiences of the daily uses.
Fixit Clinic has so far participated in the shared database with 487
data records.

{{< figure src="images/ifitxit-clinic-item-report-min.png" id="broken-item-report" alt="Screenshot of ifixit webpage with link to the broken item report." title="Screenshot of ifixit webpage with link to the broken item report." caption="Screenshot of ifixit webpage with link to the broken item report." width="100%" numbered="true">}}

### Repair Café Wales

[Repair Café Wales](https://repaircafewales.org/) opens and supports
repair cafés across Wales. Unlike the other grassroots initiatives, this
project is funded by the Welsh Government (Welsh Government's Landfill
Disposal Tax Community Scheme) and administered by the Wales Council for
Voluntary Action.

{{< figure src="images/Repair-Cafe-Wales-min.png" id="repair-cafe-wales" alt="Screenshot of website of the Repair Café Wales." title="Screenshot of website of the Repair Café Wales." caption="Screenshot of website of the Repair Café Wales." width="100%" numbered="true">}}

Customers fill out a form after arriving at the repair café. There are
[different forms to
access](https://repaircafewales.org/what-are-you-having-repaired-today/)
depending on the repair item: Apparel/Textiles, Bag/Luggage/Purse,
Bicycle, Bicycle Accessory, Car Accessory, Furniture, Heater, Home
Decor, Jewelry/Accessory, Manual Tool, Misc, Scooter, Electrical Item.
As far as I can see from the first page, only the form for the
electrical items is different, sporting a list of categories.

So far, 2505 records are documented via the Repair Cafés Wales.

### The Restart Project

[The Restart Project](https://therestartproject.org/) is a London-based
social enterprise. It organizes regular restart parties where
participants teach each other how to repair or get their broken or slow
devices back on the road. The Restart project specializes in electrical
appliances, with the joint training and repair campaign ranging from
toasters to headphones to iPhones and tablets.

{{< figure src="images/restart-project-min.png" id="restart-project" alt="Screenshot of homepage of The Restart Project." title="Screenshot of homepage of The Restart Project, 'a people-powered social enterprise that aims to fix our relationship with electronics'." caption="Screenshot of homepage of The Restart Project, 'a people-powered social enterprise that aims to fix our relationship with electronics'." width="100%" numbered="true">}}

The Restart Project also works with schools and other organizations and
is co-founder of the [European Right to Repair
Campaign](https://repair.eu/). This global movement advocates that
everyone has the right to repair the products they own themselves[^1].
The move aims to change the rules for making the devices so that they
are easy and affordable to repair. Another concern of Restart is to
protect or expand the owners' rights after the purchase and to combat
the planned obsolescence[^2].

[^1]: <i>"We are people, we are repairers, we are sustainability
    activists, we are community. ------ We believe products should last
    longer, and therefore when broken, they should be repaired. This
    requires products to be designed for repair as well as support for
    repairers of all kinds. ------ We are asking for the right to
    repair."</i>

[^2]: We talk about planned obsolescence when a manufacturer consciously
    makes design and manufacturing decisions that results in a limited
    product life. This doesn't necessarily mean that products are made
    to break after a certain period. If a manufacturer designs a product
    in such a way that it cannot be disassembled, or if they decide not
    to make spare parts, repair information, or software updates
    available, they are making a deliberate choice that result in a
    limited product life -- the product becomes obsolete due to the
    manufacturer's decision not to support its prolonged use.

{{< figure src="images/right-to-repair-min.png" id="right-to-repair" alt="Screenshot of the 'Right to Repair Initiative' homepage." title="Screenshot of the 'Right to Repair Initiative' homepage." caption="Screenshot of the 'Right to Repair Initiative' homepage." width="100%" numbered="true">}}

Data is collected at community repair events and recorded in the
[Restarters.net](https://restarters.net/about) Fixometer module.
[Fixometer](https://therestartproject.org/fixometer-2/) is the software
and database for recording the effects of community repair activities
(see also the [repository on
GitHub](https://github.com/TheRestartProject/restarters.net)). The
Restart Project is known for its scientifically-based calculation of the
CO2 savings by extending the life cycles of the repaired devices (see
the FAQ on the three topics:

How is data collected? How are the calculations made? What can we learn
from the data?

{{< figure src="images/C02-emissions-min.png" id="co2-emissions" alt="Banner of the Restarters website, which compiles and continuously updates the successes of the repair efforts. 11,035 devices repaired, 445,782 kg CO2 saved, 27,602 kg. Rubbish prevented, 2,252 events held." title="Banner of the Restarters website, which compiles and continuously updates the successes of the repair efforts." caption="Banner of the Restarters website, which compiles and continuously updates the successes of the repair efforts." width="100%" numbered="true">}}

Due to their strict methodical approach, only the organizers of the
restart parties log the item's status of the appliances brought to the
event for repair. The organizers are also the ones who then enter the
results in the Fixometer online database. The Restart Project has
already contributed 17,840 data records to the joint data acquisition.

## Aim of repairData package

With the data preparation for the large R community, I hope that the
data set will attract more attention and be examined more closely by
statistics, visualization, and modeling experts. I myself also plan to
take a closer look at the data as part of a planned R tutorial project.

{{< figure src="images/repairData-screenshot-min.png" id="repair-data" alt="Screenshot of the repairData documentation page." title="Screenshot of the repairData documentation page, written with the pkgdown package." caption="Screenshot of the repairData documentation page, written with the pkgdown package." width="100%" numbered="true">}}
