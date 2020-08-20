---
layout: gridlay
title: Publications
permalink: /publications/
excerpt: "Publications"
sitemap: false
---

# Select Publications

<h4> Visit our <a href='https://scholar.google.ca/citations?user=XQI8DIEAAAAJ&hl=en&oi=ao'> Google Scholar </a> for an updated list. </h4>

{% for publi in site.data.publications %}

  <b>{{ publi.title }}</b> <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
