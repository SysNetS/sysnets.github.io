---
title: "Khwarizmi Lab - News"
layout: textlay
excerpt: "News @ Khwarizmi Lab"
sitemap: true
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p><b>{{ article.date }}</b> <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
