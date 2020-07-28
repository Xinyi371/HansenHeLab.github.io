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
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <h5> {{ member.description }} </h5>
  </ul>
</div>

{% endfor %}

### Staff
{% for member in site.data.staff %}

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/people/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  <ul style="overflow: hidden">
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
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
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
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
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
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
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <h5> {{ member.description }} </h5>
  </ul>
</div>

{% endfor %}

### Alumni
