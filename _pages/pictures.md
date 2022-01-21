---
title: "TAU Group - Gallery"
layout: piclay
excerpt: "TAU Group -- Gallery"
permalink: /gallery/
---

[comment]: <> (#### Autopilot in Virtual RELLIS [&#40;visit V-RELLIS&#41;]&#40;https://sites.google.com/tamu.edu/rellisvirtualmap/&#41;:)

[comment]: <> (<iframe width="560" height="315" src="https://www.youtube.com/embed/6TEmWmkSpAQ" frameborder="0" allowfullscreen></iframe>)

# Gallery

{% assign number_printed = 0 %}
{% for pic in site.data.gallery %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-fluid" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>

