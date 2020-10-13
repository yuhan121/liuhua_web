---
title: "Research"
layout: gridlay
excerpt: "Research"
sitemap: false
permalink: /research/
---
<p><br/></p>
My research focuses on employing massive datasets, including satellite-retrieved high resolution exposures and health data of all Medicare beneficiaries, to investigate how climate change and air pollution influence seniors' health. More specifically, my research is focused on: <br/>
<p></p>
(1) application of remote sensing in environmental exposure modeling (e.g., predicting high-resolution PM2.5 and components, ozone, NO2, and temperature); <br/>
(2) estimating the health consequences of exposure to air pollution and climate change; <br/>
(3) estimating the link between climate change and air quality, and the mediated health impacts; <br/>
(4) estimating the joint and independent health effects of air pollutant mixtures; <br/>
(5) statistical modeling, e.g., causal modeling and big data approach. <br/>

### Highlights

{% assign number_printed = 0 %}
{% for publi in site.data.publist1 %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="wellpub">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="95%" style="margin:2 auto;" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>
