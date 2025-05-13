---
title: "INSIGHTLLM: Intelligent System for Integrating Global Human & Animal Health Technology"
layout: textlay
excerpt: "INSIGHTLLM: Bridging Animal Science and Human Nutrition through AI"
sitemap: false
permalink: /insightllm/
---

<a href="{{ site.url }}{{ site.baseurl }}/images/projects/insightllm_logo.png">
  <img src="{{ site.url }}{{ site.baseurl }}/images/projects/insightllm_logo.png" 
  class="img-responsive" width="20%" style="float: left" />
</a>

<center>
<br /><br />
<span style="color: brown; font-size:250%; font-weight: bold;">INSIGHTLLM: Intelligent System for Integrating Global Human & Animal Health Technology</span>
</center>

<br /><br /><br />

<span style="color: brown; font-size:175%;  font-weight: bold;">Team Members</span>


{% assign number_printed = 0 %}
{% for member in site.data.insightllm %}

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

<span style="color: brown; font-size:175%; font-weight: bold;">Overview</span>

The INSIGHTLLM project aims to develop a Retrieval-Augmented Generation (RAG) system that serves as a bridge between animal science and human nutrition research. By leveraging the latest reasoning language models, various RAG techniques, and document retrieval techniques, the system delivers precise, cited responses to complex queries with respect to both domains.

It is designed to empower researchers with fast, contextualized access to a vast corpus of scientific literature, streamlining interdisciplinary insights.

<br />

<span style="color: brown; font-size:175%; font-weight: bold;">Project Objectives</span>

<div style="float: left; width: 50%;">
<ul>
  <li>Bridge the gap between animal science and human nutrition through AI</li>
  <li>Implement a custom RAG architecture tailored for scientific query resolution</li>
  <li>Enable citation-backed answers derived from peer-reviewed literature</li>
</ul>
</div>

<div style="float: right; width: 50%;">
<ul>
  <li>Support interdisciplinary research through smart document retrieval</li>
  <li>Design an intuitive user interface for query-answer interaction</li>
  <li>Facilitate reproducible, scalable deployment via modular components</li>
</ul>
</div>

<br /><br /><br /><br />

<center>
<a href="{{ site.url }}{{ site.baseurl }}/images/projects/animal_rag_architecture.png">
  <img src="{{ site.url }}{{ site.baseurl }}/images/projects/animal_rag_architecture.png" 
  class="img-responsive" width="80%" />
</a>
</center>

<br />

<span style="color: brown; font-size:175%; font-weight: bold;">Key Features</span>

* **Query Translation & Expansion**: Prompted query is rewritten clearly and broken down into multiple sub-queries
* **Hybrid Retrieval**: Combines **vector embeddings** (dense) with **BM25 keyword search** (sparse)
* **LLM Integration**: Uses your local Ollama LLM (e.g., LLaMA3.1, DeepSeek-R1) to answer scientific queries
* **Cross-Encoder Reranking**: Improves result accuracy using **semantic scoring** (MiniLM L6 v2)
* **Adaptive Top-k Selection**: Top-k docs are selected upon reranking, given that k changes dynamically based on reranking scores
* **Deduplication & Filtering**: Ensures clean, diverse, and relevant chunk selection
* **Chain-of-Thought Reasoning**: LLMs are prompted to think step-by-step
* **Self-Verification**: Final answers are reviewed by a smaller lightweight LLM for consistency and accuracy, also called LLM-as-a-Judge

<br />

<span style="color: brown; font-size:175%; font-weight: bold;">Important Links</span>

<!-- [InsightLLM Webpage](/insightllm/) (internal only for now) <br /> -->
[Source Code Repository](https://github.com/taugroup/AnimalRAG) (WIP - access required) <br />

<br /><br />

