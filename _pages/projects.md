---
title: Projects
permalink: /projects/
author_profile: true
---
{% if author.googlescholar %}
{% endif %}
{% include base_path %}

## Ongoing Projects

### Active learning for ecological monitoring

* People: John Martinsson, Olof Mogren.
* Funded by Vinnova.
* 2023-2024

### Structural Causal Models for Distributional Shift in Federated Learning

* People: Edvin Listo Zec, Olof Mogren.
* Funded by Vinnova.
* [More information](https://www.vinnova.se/en/p/structural-causal-models-for-distributional-shift-in-federated-learning/)
* 2023-2024

### Towards efficient computational fluid dynamics simulations with physics-informed machine learning

* People: Maria Bånkestad, Aleksis Pirinen
* Funded by Vinnova.
* [More information](https://www.vinnova.se/en/p/towards-efficient-computational-fluid-dynamics-simulations-with-physics-informed-machine-learning/)
* 2023-2024

### Data Efficient Machine Learning for Earth Observation

* Publications:
    - [Martin Willbo, Aleksis Pirinen, John Martinsson, Edvin Listo Zec, Olof Mogren, Mikael Nilsson, Impacts of Color and Texture Distortions on Earth Observation Data in Deep Learning, 2nd ML4RS Workshop at ICLR 2024](https://arxiv.org/abs/2403.04385)
* People: Martin Willbo, Olof Mogren, Aleksis Pirinen

### Soundscape Analysis

* PhD project.
* People: John Martinsson, Olof Mogren.
* Selected publications
    - John Martinsson and Maria Sandsten. DMEL : The differentiable log-Mel spectrogram as a trainable layer in neural networks. In ICASSP 2024 - 2024 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), 2024.
    - [John Martinsson, Martin Willbo, Aleksis Pirinen, Olof Mogren, and Maria Sandsten. Few-shot bioacoustic event detection using an event-length adapted ensemble of prototypical networks. In The 7th Workshop on Detection and Classification of Acoustic Scenes and Events, number November, pages 2--6, 2022.](https://dcase.community/documents/workshop2022/proceedings/DCASE2022Workshop_Martinsson_13.pdf)

### AI for Porcelain Recognition

* Partners: [Rörstrand Museum](https://rorstrand-museum.se/)
* Funded by: Riksantikvarieämbetet (RAÄ) and Västra Götalandsregionen (VGR)
* People: Martin Willbo, Olof Mogren

### Agrifood TEF

* People: Aleksis Pirinen
* More information: [agrifoodtef.eu](https://www.agrifoodtef.eu/).

### Digital Earth Sweden

* More information: [digitalearth.se](https://digitalearth.se).
* People: Aleksis Pirinen

### Dense Stream Flow Forecasting

* Publications 
    - [Pirinen, Mogren, Västerdal, Fully Convolutional Networks for Dense Water Flow Intensity Prediction in Swedish Catchment Areas](https://arxiv.org/abs/2304.01658)
* People: Aleksis Pirinen, Olof Mogren

## Finished Projects

### 2023: ML for cloud optical thickness estimation

* Project partners: [Swedish Meteorological and Hydrological Institute (SMHI)](https://www.smhi.se/en/about-smhi/who-we-are/who-we-are-1.83748), [AI Sweden](https://www.ai.se/en), [Luleå University of Technology](https://www.ltu.se/?l=en) and the [Swedish Forestry Agency](https://www.skogsstyrelsen.se/).
* The work was published in the journal Remote Sensing (2024), got accepted as an oral at the 2nd ML-for-RS Workshop at ICLR 2024, and was presented as a poster at EUMETSAT 2023. Funded by Vinnova. One of the project deliverables was a developer event (Hackathon) for university students.
* Code & data available on [github](https://github.com/aleksispi/ml-cloud-opt-thick).
* Publications:
    - [Aleksis Pirinen, Nosheen Abid, Nuria Agues Paszkowsky, Thomas Ohlson Timoudas, Ronald Scheirer, Chiara Ceccobello, György Kovács, Anders Persson, Creating and Leveraging a Synthetic Dataset of Cloud Optical Thickness Measures for Cloud Detection in MSI, Journal of Remote Sensing (2024)](https://doi.org/10.3390/rs16040694)
    - [2nd ML4RS Workshop 2024](https://ml-for-rs.github.io/iclr2024/)
    - [EUMETSTAT 2023](https://www.eumetsat.int/eumetsat-meteorological-satellite-conference-2023)


{% for p in site.categories.projects %}

### {{p.date | date: '%Y'}} {{ p.title }}

  {% if p.description %}
{{ p.description }}
  {% endif %}

  {% if p.partners %}
* Partners: {{ p.partners }}
  {% endif %}
  {% if p.funders %}
* Funded by {{ p.funders }}
  {% endif %}
  {% if p.publications %}
* Publications:
  {% for pub in p.publications %}
    - {{ pub }}
  {% endfor %}
  {% endif %}
  {% if p.people %}
* People: {{ p.people | join: ", " }}
  {% endif %}
  {% if p.code %}
* Code: {{ p.code }}
  {% endif %}
{% endfor %}

