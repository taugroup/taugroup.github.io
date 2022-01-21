---
title: "TAU Group - Research"
layout: textlay
excerpt: "TAU Group -- Research"
sitemap: false
permalink: /research/
---

# Research
Our group develops and utilizes machine learning algorithms and tools to carry out 
simulations, data analytics, and visualization on both parallel and distributed computing 
systems.

{% assign number_printed = 0 %}
{% for res in site.data.research %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ res.title }}</pubtit>
  <a href="{{ site.url }}{{ site.baseurl }}/images/research_pic/{{ res.image }}">
      <img src="{{ site.url }}{{ site.baseurl }}/images/research_pic/{{ res.image }}" 
      class="img-responsive" width="50%" style="float: left" /></a>
  <p>{{ res.description }}</p>
  {% if res.pis %} <p><strong>PIs: </strong><em>{{ res.pis }}</em></p> {% endif %}
  <p><strong>Members Involved: </strong><em>{{ res.members }}</em></p>
  <p><strong><a href="{{ res.link.url }}">{{ res.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{  }}</strong></p>
  <p> {{ res.news }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
