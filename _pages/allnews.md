---
title: "News"
layout: textlay
excerpt: "TAU Group at Texas A&M University"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
{{ article.date }} <b>[{{ article.type | upcase }}]</b><br/>
{{ article.headline}}
{% endfor %}