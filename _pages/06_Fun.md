---
layout: gridlay
title: Fun
permalink: /fun/
excerpt: "Fun"
sitemap: false
---

# Fun

{% for event in site.data.fun %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/fun/{{ event.photo }}" class="img-responsive" width="95%" />
  <h4>{{ event.caption }}</h4>
</div>

{% endfor %}
