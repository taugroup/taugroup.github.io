---
title: "TAU Group - Projects"
layout: textlay
excerpt: "TAU Group - Projects"
sitemap: false
permalink: /projects/
---

# Current Projects
Below are some of our current projects

{% assign number_printed = 0 %}
{% for res in site.data.projects %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ res.title }}</pubtit>
  <a href="{{ site.url }}{{ site.baseurl }}/images/projects/{{ res.image }}">
      <img src="{{ site.url }}{{ site.baseurl }}/images/projects/{{ res.image }}" 
      class="img-responsive" width="50%" style="float: left" /></a>
  <p>{{ res.description }}</p>
  {% if res.pis %} <p><strong>PI: </strong><em>{{ res.pis }}</em></p> {% endif %}
  {% if res.collaborators %} <p><strong>Collaborators: </strong><em>{{ res.collaborators }}</em></p> {% endif %}
  {% if res.tags %} <p><strong>Technologies: </strong><em>{{ res.tags }}</em></p> {% endif %}
  <p><strong>Members: </strong><em>{{ res.members }}</em></p>
  <p><strong><a href="{{ site.url }}{{ site.baseurl }}{{ res.link.url }}">{{ res.link.display }}</a></strong></p>
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
