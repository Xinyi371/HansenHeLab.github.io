---
layout: gridlay
title: People
permalink: /people/
excerpt: "People"
sitemap: false
---

### Principle Investigator
{% for member in site.data.principle_investigator %}

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  <ul style="overflow: hidden">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br> {{ member.info2 }}<br> {{ member.info3 }}<br> {{ member.email }} </i>
  <h5> {{ member.description }} <br><br> {{ member.description2 }} <br><br> {{ member.description3 }} </h5>
  </ul>
</div>

{% endfor %}

### Staff
{% for member in site.data.staff %}

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  <ul style="overflow: hidden">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br> {{ member.email }}</i>
  <h5> {{ member.description }} </h5>
  </ul>
</div>

{% endfor %}

### Postdoctoral Fellows
{% for member in site.data.postdoctoral_fellows %}

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  <ul style="overflow: hidden">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br> {{ member.email }}</i>
  <h5> {{ member.description }} </h5>
  </ul>
</div>

{% endfor %}

### Visiting Scholars
{% for member in site.data.visiting_scholars %}

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  <ul style="overflow: hidden">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br> {{ member.email }}</i>
  <h5> {{ member.description }} </h5>
  </ul>
</div>

{% endfor %}

### Graduate Students
{% for member in site.data.graduate_students %}

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  <ul style="overflow: hidden">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br> {{ member.email }}</i>
  <h5> {{ member.description }} </h5>
  </ul>
</div>

{% endfor %}

### Alumni
{% assign number_printed = 0 %}
{% for member in site.data.alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>Current Position: {{ member.current }}</i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}
