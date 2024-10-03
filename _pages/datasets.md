---
title: "NILab - Datasets"
layout: datasets
excerpt: "NILab - Datasets"
sitemap: false
permalink: /datasets/
---
<br>
# Datasets

<!-- {% for dataset in site.data.datasets %} -->
 <!-- <div class="card mb-4"> -->
 <!-- <div class="row no-gutters"> -->
  <!--Column for the image
   <!-- <div class="col-md-4"> -->
   <!-- <img src="{{ site.url }}{{ site.baseurl }}/images/datasets/{{ dataset.image }}" class="img-responsive" width="100%" style="float: left" alt="{{ dataset.title }}"> -->
   <!-- </div> -->
   <!--Column for the text
   <!-- <div class="col-md-8 d-flex align-items-center"> -->
   <!-- <div class="card-body"> -->
   <!-- <h3>{{ dataset.title }}</h3> -->
   <!-- <p>{{ dataset.description }}</p> -->
   <!-- {% if dataset.badge_ == 1 %} -->
   <!-- <img src="{{ site.url }}{{ site.baseurl }}/images/datasets/{{ dataset.badge }}" class="img-responsive" width="30%" style="float: left" alt="{{ dataset.title }}"/> -->
   <!-- {% endif %} -->
   <!-- <div style="clear: left;"> -->
   <!-- <p><strong><a href="{{ dataset.link.url }}">{{ dataset.link.display }}</a></strong></p> -->
   <!-- </div> -->
   <!-- </div> -->
   <!-- </div> -->
 <!-- </div> -->
 <!-- </div> -->
<!-- {% endfor %} -->

{% for dataset in site.data.datasets %}
 <div class="card mb-4" style="width: 971px; border: 1px solid #ddd; padding: 25px; border-radius: 8px;">
  <div class="row no-gutters">
   <!-- Column for the image -->
   <div class="col-md-4">
   <img src="{{ site.url }}{{ site.baseurl }}/images/datasets/{{ dataset.image }}" class="img-responsive" width="90%" style="float: left" alt="{{ dataset.title }}">
   </div>
   <!-- Column for the text -->
  <div class="col-md-8 d-flex align-items-center">
  <div class="card-body">
  <h3 style="margin-bottom: 1px;">{{ dataset.title }}</h3>
  <p style="margin-top: -20px;">{{ dataset.description }}</p>
  {% if dataset.badge_ == 1 %}
  <a href="{{ dataset.link.url }}"><img src="{{ site.url }}{{ site.baseurl }}/images/datasets/{{ dataset.badge }}" class="img-responsive" width="30%" style="float: left" alt="{{ dataset.title }}"/></a>
  {% endif %}
  <div style="clear: left;">
  {% if dataset.badge_ == 0 %}
  <p><strong><a href="{{ dataset.link.url }}">{{ dataset.link.display }}</a></strong></p>
  {% endif %}
  </div>
  </div>
  </div>
  </div>
 </div>
 <br>
{% endfor %}

<p> &nbsp; </p>
