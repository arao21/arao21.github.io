---
layout: single
title: "Mentoring & Service"
permalink: /teaching/
author_profile: true
---

{% assign teaching_items = site.teaching | where: "type", "teaching" | sort: "date" | reverse %}
{% assign service_items  = site.teaching | where: "type", "service"  | sort: "date" | reverse %}

## Mentoring & Tecahing
{% for post in teaching_items %}
  {% include archive-single.html %}
{% endfor %}

## Service
{% for post in service_items %}
  {% include archive-single.html %}
{% endfor %}
