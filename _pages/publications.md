---
layout: page
permalink: /publications/
title: publications
description: Here are my publications by categories in reversed chronological order.
journals_years: [2021, 2020, 2018, 2013, 2012, 2009]
conferences_years: [2020, 2019, 2018, 2016, 2014, 2013, 2011, 2010, 2009, 2008, 2005, 2004, 2002, 2000]
bc_years: [2010]
pa_years: [2018, 2017]
nav: true
---

<div class="publications">

<H1>Journals</H1>

{% for y in page.journals_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<H1>Book Chapters</H1>

{% for y in page.bc_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f bc -q @*[year={{y}}]* %}
{% endfor %}

<H1>Patents</H1>

{% for y in page.pa_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f pa -q @*[year={{y}}]* %}
{% endfor %}

- Anallely Olivares Toledo and Sonia Mendoza, Patent number: 352343, Name: "Sistema y método para coordinación y sincronización de actividades en un entorno colaborativo", Instituto Mexicano de la Propiedad Industrial, Date of issuance: October 13, 2017, Expiration date: June 27, 2033.

<H1>Conferences</H1>

{% for y in page.conferences_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>