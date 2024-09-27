---
title: "NetNeuroLab - Datasets"
layout: datasets
excerpt: "NetNeuroLab - Datasets"
sitemap: false
permalink: /Datasets/
---

# Datasets

{% for dataset in site.data.datasets %}
 <div class="card mb-4">
  <div class="row no-gutters">
  <!-- Column for the image -->
   <div class="col-md-4">
   <img src="{{ site.url }}{{ site.baseurl }}/images/datasets/{{ dataset.image }}" class="img-responsive" width="100%" style="float: left" alt="{{ dataset.title }}">
   </div>
   <!-- Column for the text -->
   <div class="col-md-8 d-flex align-items-center">
   <div class="card-body">
   <h3>{{ dataset.title }}</h3>
   <p>{{ dataset.description }}</p>
   {% if dataset.badge_ == 1 %}
   <img src="{{ site.url }}{{ site.baseurl }}/images/datasets/{{ dataset.badge }}" class="img-responsive" width="30%" style="float: left" alt="{{ dataset.title }}"/>
   {% endif %}
   <div style="clear: left;">
   <p><strong><a href="{{ dataset.link.url }}">{{ dataset.link.display }}</a></strong></p>
   </div>
   </div>
   </div>
  </div>
 </div>
{% endfor %}

<p> &nbsp; </p>