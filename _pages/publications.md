---
title: "NILab - Publications"
layout: gridlay
excerpt: "NILab -- Publications."
sitemap: false
permalink: /publications/
---

<br>
# Publications

For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.com/citations?hl=it&user=5g4UY4MAAAAJ&view_op=list_works&sortby=pubdate) or [PubMed](https://pubmed.ncbi.nlm.nih.gov/?term=Avesani+P&cauthor_id=27747500). Code is available on our [GitHub repo](https://github.com/FBK-NILab).

## Highlights

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well" style="height: 300px; overflow: hidden; position: relative;">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <div style="overflow: hidden; height: 100%;">
   <p><em>{{ publi.authors }}</em></p>
   <p>{{ publi.journal }}, {{ publi.year }}</p>
   <p>{{ publi.description }}</p>
   <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
   <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
   <p> {{ publi.news2 }}</p>
  </div>
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


## Full List

{% for publi in site.data.publist %}

  {{ publi.authors }} ({{ publi.year }}). {{ publi.title }}. <em>{{ publi.journal }}</em>.<br>
  {% if publi.doi == 1 %}DOI: <a href="{{ publi.link.url }}">{{ publi.link.display }}</a>{% endif %}
{% endfor %}
<br>
