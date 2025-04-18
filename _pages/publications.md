---
title: "SysNetS Lab - Publications"
layout: gridlay
excerpt: "SysNetS Lab -- Publications."
sitemap: true
permalink: /publications/
---


# Publications

## Highlights

**At the end of this page, you can find the [full list of publications](#full-list-of-publications).**

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}
  {% if publi.link.pdf %}[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.pdf }}" target="_blank">PDF</a>]{% endif %}
  {% if publi.link.slides %}[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.slides }}" target="_blank">Slides</a>]{% endif %}
  </pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}" target="_blank">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


<!-- ## Patents  -->

## Full List of publications
### Papers

{% for publi in site.data.publist %}

  <b>{{ publi.year }}:</b> {{ publi.title }}
  <!-- Check if file links exist -->
  {% if publi.link.pdf %}<b>[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.pdf }}" target="_blank">PDF</a>]</b>{% endif %}
  {% if publi.link.slides %}<b>[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.slides }}" target="_blank">Slides</a>]</b>{% endif %}


  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% if publi.award == 1 %}<h4 style="color:Tomato;"><strong>Distinguished Paper Award</strong></h4>{% endif %}
  {% if publi.nomination == 1 %}<h4 style="color:Tomato;"><strong>Best Paper Award nomination </strong></h4>{% endif %}
{% endfor %}



### Book

{% for publi in site.data.publist_book %}

  <b>{{ publi.year }}:</b> {{ publi.title }}
  <!-- Check if file links exist -->
  {% if publi.link.pdf %}<b>[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.pdf }}" target="_blank">PDF</a>]</b>{% endif %}
  {% if publi.link.slides %}<b>[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.slides }}" target="_blank">Slides</a>]</b>{% endif %}


  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% if publi.award == 1 %}<h4 style="color:Tomato;"><strong>Distinguished Paper Award</strong></h4>{% endif %}
  {% if publi.nomination == 1 %}<h4 style="color:Tomato;"><strong>Best Paper Award nomination </strong></h4>{% endif %}
{% endfor %}


### Thesis

{% for publi in site.data.publist_thesis %}

  <b>{{ publi.year }}:</b> {{ publi.title }}
  <!-- Check if file links exist -->
  {% if publi.link.pdf %}<b>[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.pdf }}" target="_blank">PDF</a>]</b>{% endif %}
  {% if publi.link.slides %}<b>[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.slides }}" target="_blank">Slides</a>]</b>{% endif %}


  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% if publi.award == 1 %}<h4 style="color:Tomato;"><strong>Distinguished Paper Award</strong></h4>{% endif %}
  {% if publi.nomination == 1 %}<h4 style="color:Tomato;"><strong>Best Paper Award nomination </strong></h4>{% endif %}
{% endfor %}


### Industrial Conference

{% for publi in site.data.publist_industry %}

  <b>{{ publi.year }}:</b> {{ publi.title }}
  <!-- Check if file links exist -->
  {% if publi.link.pdf %}<b>[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.pdf }}" target="_blank">PDF</a>]</b>{% endif %}
  {% if publi.link.slides %}<b>[<a href="{{ site.url }}{{ site.baseurl }}/docs/{{ publi.link.slides }}" target="_blank">Slides</a>]</b>{% endif %}


  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
  {% if publi.award == 1 %}<h4 style="color:Tomato;"><strong>Distinguished Paper Award</strong></h4>{% endif %}
  {% if publi.nomination == 1 %}<h4 style="color:Tomato;"><strong>Best Paper Award nomination </strong></h4>{% endif %}
{% endfor %}

