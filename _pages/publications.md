---
title: "TAU Group - Publications"
layout: gridlay
excerpt: "TAU Group -- Publications."
sitemap: false
permalink: /publications/
---


# Publications

## Group highlights

(For a full list of publications and patents see [below](#patents) or go to [Google Scholar](https://scholar.google.com/citations?user=f_gkIjQAAAAJ&hl=en), [ResearcherID](https://www.researcherid.com/rid/N-2421-2015))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
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

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Patents
<em>Lorem ipsum dolor sit amet, </em><br />consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.<br /> PCT/NL20-20/050797 (2020)

<em>Lorem</em><br /> ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor <br /> <a href="https://patents.google.com/patent/US10439125B2/en?inventor=Milan+ALLAN&oq=inventor:(Milan+ALLAN)">US10439125B2 (2016)</a>

