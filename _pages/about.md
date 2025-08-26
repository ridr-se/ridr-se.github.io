---
permalink: /
title: "RISE DL Research Group"
excerpt: "RISE DL Research Group"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


Welcome to the _RIDR, the Deep Learning Research Group at RISE_.
We're a [team of researchers](https://ridr.se/people/) who work on foundational problems within machine learning,
and apply our expertise on problems related to climate change and ecology. We founded [Climate AI Nordics](https://climateainordics.com/); we also host the weekly
[Learning Machines seminar series](https://www.ri.se/en/what-we-do/educations/learning-machines-seminars) at RISE
-- [have a look](https://www.youtube.com/playlist?list=PLqLiVcF3GKy1tuQFoDu5QKOM6S33t_4R1) at our great collection of talks.

## [News](/news/)

{% for p in site.categories.news limit: 5 %}
* {{p.date | date: '%Y-%m-%d'}}: {{ p.title }} [(Read more)]({{ p.url }})
{% endfor %}


## [People](/people/)

![](/images/people/all.jpg)

* [Olof Mogren, PhD](https://mogren.one/)
* [Aleksis Pirinen, PhD](https://aleksispi.github.io)
* [Maria Bånkestad, PhD](https://scholar.google.se/citations?user=4tKNCSkAAAAJ&hl=sv&oi=ao)
* [John Martinsson, MSc, PhD candidate](https://johnmartinsson.org/)
* [Isabelle Tingzon, MSc, PhD candidate](https://issa-tingzon.github.io)
* Ayush Prasad, MSc
* Fan Wang, MSc

[Visit our Scholar profile](https://scholar.google.com/citations?hl=en&view_op=list_works&gmla=AILGF5UiJtxGkjJ5z3BHO8C37KQwQysUjHyMJAJ1_USVi8t0aoC30hfUabA1jtbynBICV0v_UZzGMFRF8Oq3TtmW4gRaixB3HQ_MIBuoOYsG&user=yc43h58AAAAJ)

<!--## News

**March 2024:** Two papers accepted for the [2nd Machine Learning for Remote Sensing workshop](https://ml-for-rs.github.io/iclr2024/) at ICLR 2024.

*February 2024:* Journal paper accepted for _Remote Sensing_.-->


