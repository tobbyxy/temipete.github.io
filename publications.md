---
layout: page
permalink: /publications/
title: publications
---

## publications

{% assign thumbnail="left" %}

{% for pub in site.data.publications %}

{% if pub.pdf and pub.software %}
  [**{{pub.title}}**]({{pub.url}})<br/>
  {{pub.authors}} <br/>
  <i>{{pub.journal}}</i> ({{pub.year}})<br/>
  [[PDF]({{pub.pdf}})] [[Software]({{pub.software}})]
{% elsif pub.software %}
  [**{{pub.title}}**]({{pub.url}})<br/>
  {{pub.authors}} <br/>
  <i>{{pub.journal}}</i> ({{pub.year}})<br/>
  [[Software]({{pub.software}})]
{% elsif pub.pdf %}
  [**{{pub.title}}**]({{pub.url}})<br/>
  {{pub.authors}} <br/>
  <i>{{pub.journal}}</i> ({{pub.year}})<br/>
  [[PDF]({{pub.pdf}})] 
{% else %}
  [**{{pub.title}}**]({{pub.url}})<br/>
  {{pub.authors}} <br/>
  <i>{{pub.journal}}</i> ({{pub.year}})<br/>
{% endif %}

{% endfor %}



<!-- 
# publications
1. Shin D, Lee KJ, **Adeluwa T**, Hur J. Machine Learning-Based Predictive Modeling of Postpartum Depression. *J Clin Med.* 2020;9(9):2899. Published 2020 Sep 8. doi:10.3390/jcm9092899

2. Ishola IO, Akinyede AA, **Adeluwa TP**, Micah C. Novel action of vinpocetine in the prevention of paraquat-induced parkinsonism in mice: involvement of oxidative stress and neuroinflammation. *Metab Brain Dis.* 2018;33(5):1493-1500. doi:10.1007/s11011-018-0256-9 -->
