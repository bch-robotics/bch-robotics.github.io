---
title: "Dupont Lab - Publications"
layout: gridlay
excerpt: "Dupont Lab -- Publications."
sitemap: false
permalink: /publications/
---


### Publications 

<div><b><a href="https://scholar.google.com/citations?user=15g03MoAAAAJ&hl=en">Google Scholar</a></b> - <b><a href="https://pubmed.ncbi.nlm.nih.gov/?term=Pierre+E.+Dupont">PubMed</a></b>

<!---## Group highlights--->

<!---**At the end of this page, you can find the [full list of publications and patents](#full-list-of-publications).**--->

<!---{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

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

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>--->


<!---## Patents
<em>Sample Patent Author</em><br /> Methods of turning water to wine <br /> <a href="https://scholar.google.com/">US314159 (2023)</a>

## Full List of publications--->

{% for publi in site.data.publist %}

 <div>
  <h4> {{publi.year}} </h4>
  {{ publi.title }} <br> 
  <em>{{ publi.authors }} </em><br><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
 <br/>
  {{ publi.editor }}
 </div>

{% endfor %}
