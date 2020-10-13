---
title: "Publications"
layout: gridlay
excerpt: "Publications"
sitemap: false
permalink: /publications/
---

### Full List   
<p></p>

<div class="col-sm-12 clearfix">
#### In review

{% for publi in site.data.publist1 %}

{% if publi.first_or_cor == 1 %}
  <b>{{ publi.title }}</b><br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}

{% if publi.first_or_cor == 0 %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}

{% endfor %}
</div>
<div class="col-sm-12 clearfix">
####  Peer-reviewed articles<br/>
####  2020

{% for publi in site.data.publist2 %}

{% if publi.first_or_cor == 1 %}
  <b>{{ publi.title }}</b><br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}

{% if publi.first_or_cor == 0 %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}

{% endfor %}
</div>

<div class="col-sm-12 clearfix">
####  2019 and earlier

{% for publi in site.data.publist3 %}

{% if publi.first_or_cor == 1 %}
  <b>{{ publi.title }}</b><br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}

{% if publi.first_or_cor == 0 %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}

{% endfor %}
</div>
