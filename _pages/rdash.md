---
title: "TAU Group - RDash Project"
layout: textlay
excerpt: "TAU Group - RDash Project"
sitemap: false
permalink: /rdash/
---

# About the Product

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

# Capabilities

* Feature 1 [Click_here_for_Demo](https://notworkinglink-addyourlinkhere.org) - Description 1 
* Feature 2 [Click_here_for_Demo](https://notworkinglink-addyourlinkhere.org) - Description 2 
* Feature 3 [Click_here_for_Demo](https://notworkinglink-addyourlinkhere.org) - Description 3 
* Feature 4 [Click_here_for_Demo](https://notworkinglink-addyourlinkhere.org) - Description 4 

# Poster

Below is the poster we presented in 'Advances In Data Science Theory Methods and Computation' at Texas A&M University, 2022

<div >
  <img src="{{ site.url }}{{ site.baseurl }}/images/posters/RDASH-Grants_poster.jpg" class="img-responsive" 
  width="200%" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">

  </ul>
</div>


# For Developers

Documentation of the project : 
[Click_here_for_source_code](https://notworkinglink-addyourlinkhere.org) 

Link to github repository : 
[RDash Project](https://github.com/taugroup/RDASH) 


# Team Members


{% assign number_printed = 0 %}
{% for member in site.data.compliance %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">

  </ul>
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

