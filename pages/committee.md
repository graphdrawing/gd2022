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

* Patrizio Angelini (co-chair), John Cabot University, Italy
* Therese Biedl, University of Waterloo, Canada
* Sabine Cornelsen, Universität Konstanz, Germany
* Giordano Da Lozzo, Roma Tre University, Italy
* Stephan Diehl, Universität Trier, Germany
* Henry Förster, Universität Tübingen, Germany
* Martin Gronemann, TU Wien, Austria
* Yasuhiro Hashimoto, The University of Aizu, Japan
* Michael Hoffmann, ETH Zürich, Switzerland
* Hiroshi Hosobe, Hosei University, Japan
* Yifan Hu, Yahoo! Research, USA
* Takayuki Itoh, Ochanomizu University, Japan
* Philipp Kindermann, Universität Trier, Germany
* Karsten Klein, Universität Konstanz, Germany
* Stephen Kobourov, University of Arizona, USA
* Jan Kratochvíl, Charles University of Prague, Czech Republic
* Kim Marriott, Monash University, Australia
* Irene Parada, TU Eindhoven, The Netherlands
* Sergey Pupyrev, Facebook, USA
* Helen Purchase, University of Glasgow, Scotland
* Arnaud Sallaberry, LIRMM, Université Paul-Valéry Montpellier, France
* Ingo Scholtes, University of Zurich, Switzerland
* Falk Schreiber, Universität Konstanz, Germany
* André Schulz, FernUniversität in Hagen, Germany
* Andrew Suk, University of California San Diego, USA
* Antonios Symvonis, National Technical University of Athens, Greece
* Alessandra Tappini, University of Perugia, Italy
* Meirav Zehavi, Ben-Gurion University, Israel
* Reinhard von Hanxleden (co-chair), Christian-Albrechts-Universität zu Kiel, Germany
* Tatiana von Landesberger, Universität Köln, Germany

## Steering Committee

Please refer to [graphdrawing.org](http://graphdrawing.org/sc.html)
