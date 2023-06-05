---
title: "TAU Group - RDash Project"
layout: textlay
excerpt: "TAU Group - RDash Project"
sitemap: false
permalink: /rdash/
---

<a href="{{ site.url }}{{ site.baseurl }}/images/projects/Rdash_1.png">
      <img src="{{ site.url }}{{ site.baseurl }}/images/projects/Rdash_1.png" 
      class="img-responsive" width="20%" style="float: left" /></a>

<center>
<span style="color: brown; font-size:250%; font-weight: bold;">RDash: An Organizational Intelligence Platform for Institutional Research</span>
</center>

<br />
<br />

<br />
<br />
<span style="color: brown; font-size:175%;  font-weight: bold;">Team Members</span>

{% assign number_printed = 0 %}
{% for member in site.data.compliance %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="20%" style="float: left" />
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


<br />
<br />

<span style="color: brown; font-size:175%;  font-weight: bold;">Overview</span>

A recommendation system that captures the opportunities for pursuing external research funds through grants, contracts, and subcontracts based on the scholar’s research profile. RDash-Grants entails analyzing a massive set of solicitations and funding opportunities and selecting the most appropriate one or group of relevant grants by considering the scholar’s preferences and research profile.

<!-- # Capabilities

* Feature 1 [Click_here_for_Demo](https://notworkinglink-addyourlinkhere.org) - Description 1 
* Feature 2 [Click_here_for_Demo](https://notworkinglink-addyourlinkhere.org) - Description 2 
* Feature 3 [Click_here_for_Demo](https://notworkinglink-addyourlinkhere.org) - Description 3 
* Feature 4 [Click_here_for_Demo](https://notworkinglink-addyourlinkhere.org) - Description 4  -->

<span style="color: brown; font-size:175%;  font-weight: bold;">Poster</span>

Below is the poster we presented in 'Advances In Data Science Theory Methods and Computation' at Texas A&M University, 2022

<div >
  <img src="{{ site.url }}{{ site.baseurl }}/images/posters/RDASH-Grants_poster.jpg" class="img-responsive" 
  width="200%" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  <ul style="overflow: hidden">

  </ul>
</div>



<span style="color: brown; font-size:175%;  font-weight: bold;"> Important Links </span>

Documentation of the project : 
[Documentation (TAU Group members only)](https://documentation-rdash.readthedocs.io/en/latest/) 

Link to github repository : 
[RDash Project (TAU Group members only)](https://github.com/taugroup/RDASH) 

<br />
<br />
