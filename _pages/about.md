---
permalink: /
title: "FAMLE Lab"
excerpt: "FAMLE Lab"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


Welcome to _FAMLE: Foundational and Applied Machine Learning for the Earth Lab_.
We're a [team of researchers](https://famle-lab.org/people/) who work on foundational problems within machine learning,
and apply our expertise on problems related to climate change and ecology.

## [News](/news/)

{% for p in site.categories.news limit: 3 %}
* {{p.date | date: '%Y-%m-%d'}}: {{ p.title }} [(Read more)]({{ p.url }})
{% endfor %}


## [FAMLE People](/people/)

* [Olof Mogren, PhD](https://mogren.one/)
* [Aleksis Pirinen, PhD](https://aleksispi.github.io)
* [Edvin Listo Zec, MSc, PhD candidate](https://edvinli.github.io/)
* [John Martinsson, MSc, PhD candidate](https://johnmartinsson.github.io/)
* [Maria Bånkestad, MSc, PhD candidate](https://scholar.google.se/citations?user=4tKNCSkAAAAJ&hl=sv&oi=ao)
* [Martin Willbo, MSc](https://scholar.google.se/citations?hl=sv&user=uuxnINUAAAAJ)

[Visit our Scholar profile](https://scholar.google.com/citations?hl=en&view_op=list_works&gmla=AILGF5UiJtxGkjJ5z3BHO8C37KQwQysUjHyMJAJ1_USVi8t0aoC30hfUabA1jtbynBICV0v_UZzGMFRF8Oq3TtmW4gRaixB3HQ_MIBuoOYsG&user=yc43h58AAAAJ)

<!--## News

**March 2024:** Two papers accepted for the [2nd Machine Learning for Remote Sensing workshop](https://ml-for-rs.github.io/iclr2024/) at ICLR 2024.

*February 2024:* Journal paper accepted for _Remote Sensing_.-->


