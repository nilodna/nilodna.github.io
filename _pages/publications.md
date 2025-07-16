---
layout: page
permalink: /publications/
title: publications
nav: true
description: My publications in reverse chronological order with highlights in <strong>bold</strong>. Papers with a journal listed means they are already submitted.
years: [2025, 2024, 2023, 2022, 2021, 2019]
order: 7
---

<h5 class="year">In prep.</h5>
{% bibliography -f preprints %}

{% for y in page.years %}
<h5 class='year'>{{y}}</h5>
{% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}



