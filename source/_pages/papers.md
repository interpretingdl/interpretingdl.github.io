---
title: 'Key papers'
layout: single
classes: wide
permalink: /papers
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/network-bw-1.png
years: [2018, 2017, 2015]
sidebar:
  - nav: pubnav
---
{% for y in page.years %}
  <h3  id="{{y}}" class="pubyear">{{y}}</h3>
  {% bibliography -f interpretingdl -q @*[year={{y}}]* %}
{% endfor %}
