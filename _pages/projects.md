---
title: Projects
permalink: /projects/
author_profile: true
---
{% if author.googlescholar %}
{% endif %}
{% include base_path %}

<!-- NOTE! NEW PROJECTS ARE ADDED AS POSTS IN projects/_posts! //-->
<!-- THIS FILE NEEDS EDITING ONLY IF THE PRESENTATION OF THE PROJECTS NEED TO CHANGE. //-->

{% capture nowunix %}{{'now' | date: '%s'}}{% endcapture %}

{% assign headlines = "Ongoing Projects, Finished Projects" | split: ", " %}

{% for h in headlines %}

## {{ h }}

  {% for p in site.categories.projects %}
    {% capture enddatetime %}{{p.enddate | date: '%s'}}{% endcapture %}
    {% assign crit1 = enddatetime < nowunix and h == "Finished Projects" %}
    {% assign crit2 = enddatetime >= nowunix and h == "Ongoing Projects" %}
    {% if crit1 or crit2 %}

### {{p.date | date: '%Y'}} {{ p.title }}

{% if p.description %}{{ p.description }}{% endif %}

{% if p.partners %}* Partners:{% for part in p.partners %}
    - {{ part }}{% endfor %}
{% endif %}
{% if p.funders %}{% if p.funders.first %}* Funded by:{% for funder in p.funders %}
    - {{ funder }}{% endfor %}
{% else %}* Funded by {{ p.funders }}{% endif %}{% endif %}
{% if p.publications %}* Publications:{% for pub in p.publications %}
    - {{ pub }}{% endfor %}{% endif %}
{% if p.people %}* People: {{ p.people | join: ", " }}{% endif %}
{% if p.code %}* Code: {{ p.code }}{% endif %}

    {% endif %}
  {% endfor %}
{% endfor %}

