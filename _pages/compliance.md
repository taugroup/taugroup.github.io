---
title: "TAU Group - Lighthouse Project"
layout: textlay
excerpt: "TAU Group - Lighthouse Project"
sitemap: false
permalink: /compliance/
---

<a href="{{ site.url }}{{ site.baseurl }}/images/projects/Lighthouse.png">
      <img src="{{ site.url }}{{ site.baseurl }}/images/projects/Lighthouse.png" 
      class="img-responsive" width="25%" style="float: left" /></a>

<center>
<span style="color: brown; font-size:400%; font-weight: bold;">Lighthouse Project : Red Flag AI Tool</span>

<br />
<br />
<!-- <span style="color: brown; font-size:125%; font-weight: bold;">Placeholder for a one-liner explaining the project</span> -->
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



<br />
<br />



<span style="color: brown; font-size:175%;  font-weight: bold;">Overview</span>

The aim of this project is to develop algorithms and their embodiment in prototype software to implement the categorization.

The software will accept as input the project information and produce as output a profile summarizing the documents relevance to each topic e.g. through a numerical score in each topic, and analysis of the frequencies of keywords in each topic, together with a summary of the set of proposals.

<br />



<span style="color: brown; font-size:175%; font-weight: bold;">Project Objectives</span>

<div style="float: left; width: 50%;">
<ul>
<li>Create analytical dashboard for the Texas A&M research enterprise</li>
<li>Identify Texas A&M research capacity for strategic assessment</li>
<li>Identify Texas A&M subject matter experts and research clusters</li>

</ul>
</div>
<div style="float: right; width: 50%;">
<ul>
<li>Advance opportunities for interdisciplinary research</li>
<li>Strategically map capacity to state/national funding opportunities</li>
<li>Define the Texas A&M global research footprint</li>

</ul>
</div>

<br />
<br />
<br />
<br />

<br />


<center>
<a href="{{ site.url }}{{ site.baseurl }}/images/projects/Lighthouse_6.png">
      <img src="{{ site.url }}{{ site.baseurl }}/images/projects/Lighthouse_6.png" 
      class="img-responsive" width="80%" /></a>
</center>

<span style="color: brown; font-size:175%;  font-weight: bold;">Key Features</span>



* Implementation - Frontend with Web Programming
    * **Interactive dashboard** interface
    * Built with **Django** - a Python-based open source web programming framework that seamlessly integrates with Python-based analysis backend
    * **Authentication** required for internal usage
    * **Model-View-Controller** design pattern to facilitate future development
    * **Modular design** to scale and sustain

<br />


<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="4000" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
        <li data-target="#carousel" data-slide-to="4"></li>
 </ol>

    <!-- Items -->
    <div class="carousel-inner" markdown="0">
        <div class="item active">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_1.png" alt="Slide 1" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_2.png" alt="Slide 2" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_3.png" alt="Slide 3" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_4.png" alt="Slide 4" />
        </div>
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_5.png" alt="Slide 5" />
        </div>  
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_6.png" alt="Slide 6" />
        </div>  
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_7.png" alt="Slide 7" />
        </div>  
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_8.png" alt="Slide 8" />
        </div>  
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_9.png" alt="Slide 9" />
        </div>  
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_10.png" alt="Slide 10" />
        </div>  
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_11.png" alt="Slide 11" />
        </div>  
        <div class="item">
            <img src="{{ site.url }}{{ site.baseurl }}/images/slider_lighthouse/Lighthouse_SS_12.png" alt="Slide 12" />
        </div>  
              
    </div>
  <a class="left carousel-control" href="#carousel" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>

<br />
* Implementation - Backend with Natural Language Processing 
    * **Define Red Flag Lists** There are 6 red flag lists: AWO, Biosafety, HRPP, EHS, Export Control, and Privacy.
    * **Read in PDFs** - Read in and transform PDF files into plain text files for further analysis.
    * **TF-IDF Analysis** The Term Frequency Inverse Document Frequency (TF-IDF) analysis is done to identify representative terms for each proposal.
    * **Similarity Analysis** Carry out similarity analysis between the reg flags and parsed proposals to identify compliance issues.

<center>
<a href="{{ site.url }}{{ site.baseurl }}/images/projects/Lighthouse_5.png">
      <img src="{{ site.url }}{{ site.baseurl }}/images/projects/Lighthouse_5.png" 
      class="img-responsive" width="100%" /></a>
</center>


<br />
<br />

<span style="color: brown; font-size:175%;  font-weight: bold;">Important Links</span>

#### [Lighthouse Website](http://datahub.geos.tamu.edu:8989/) (TAMU CAS protected)    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Documentation of the project](https://notworkinglink-addyourlinkhere.org) (WIP- TauGroup members only)  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Github repository](https://github.com/taugroup/PDFTHT) (TauGroup members only)

<br />

<br />

<br />
<br />



