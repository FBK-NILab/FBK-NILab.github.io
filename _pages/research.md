---
title: "NILab - Research"
layout: textlay
excerpt: "NILab - Research"
sitemap: false
permalink: /research/
---
<br>
# Research


{% assign number_printed = 0 %}
{% for proj in site.data.projlist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if proj.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well" style="height: 570px;">
  <pubtit class="text-center">{{ proj.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/{{ proj.image }}" class="img-responsive" width="200%" style="float: center" />
  <p>{{ proj.description }}</p>
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

# Collaborations

<div>
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_cismed.png" style="width: 90px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_apss.jpg" style="width: 140px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_ospedale_bambino_gesu.png" style="width: 140px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_medea.png" style="width: 140px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_chu.jpeg" style="width: 140px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_iit.png" style="width: 140px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_uniss.png" style="width: 140px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_bordeaux.png" style="width: 140px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_cnrs.png" style="width: 140px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_indiana.png" style="width: 190px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_lubeck.png" style="width: 210px">
</div>

# Funding

<div>
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_pnrr.png" style="width: 270px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_mariecurie.png" style="width: 120px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_pat.png" style="width: 120px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_caritro.png" style="width: 120px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_fondazione_VRT.png" style="width: 120px">
  &nbsp;
  &nbsp;
  <img src="{{ site.url }}{{ site.baseurl }}/images/research/collab_funds/logo_cloudify.png" style="width: 120px">
</div>
