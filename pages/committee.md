---
# permalink: /about/
layout: single
title: "Committee"
header:
  image: /assets/images/teaser/snow.png
  caption: "Image credit: [**Tokyo Tech**](https://www.titech.ac.jp/english)"
last_modified_at: 2021-10-26
toc: true
---

{% assign data = site.data.publicity %}

## Organization Committee

{% assign role = "" %}
{% for member in data.OC-Members %}
  {% if role != member.Role %}
    {% assign role = member.Role %}
<h3 class="oc-role"><strong>{{ member.Role }}</strong></h3>
  {% endif %}
<div style="display: inline-block; width: 45%; text-align: left;">
  {% if member.Photo == "yes" %}
<img style="border-radius: 50%" src="../../assets/images/oc/{{ member.First }}_{{ member.Given }}.jpg"
     class="circle" width="150" height="150" /><br />
  {% else %}
<img style="border-radius: 50%" src="../../assets/images/oc/nobody.jpg" width="150" height="150" /><br />
  {% endif %}
<strong>{{ member.First }} {{ member.Given }}</strong><br />
{{ member.Affiliation }}<br /><br />
</div>
{% endfor %}


## Program Committee

## Steering Committee

Please refer to [graphdrawing.org](http://graphdrawing.org/sc.html)
