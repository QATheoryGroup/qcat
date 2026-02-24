---
layout: page
title: Research
sitemap: false
permalink: /research
---

We aim to bridge the gap between fundamental quantum theory and practical quantum technologies. Our work explores applications in the nascent fault-tolerant quantum regime, such as quantum simulations for molecular interactions in chemistry; preparing resource states for fault-tolerant quantum computing, and quantum machine learning. Mitigating the impact of noise on quantum computers remains a persistent challenge. To this end, we develop application-specific protocols in quantum noise characterization and control and quantum error mitigation, particularly in regimes where only nascent capaibilities in quantum error correction can be assumed.

## Highlights

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="https://raw.githubusercontent.com/QATheoryGroup/qcat/main/{{ publi.image }}" class="img-responsive" width="50%" style="float: left" />
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

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

## Full list of publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
