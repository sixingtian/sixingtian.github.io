---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
{% include base_path %}

<h2>Journal Articles</h2>
{% assign pubs = site.publications | where: "category", "manuscripts" | sort: "date" | reverse %}
{% for post in pubs %}
  {% include archive-single.html %}
{% endfor %}

<h2>Working Papers</h2>
{% assign wps = site.publications | where: "category", "workingpapers" | sort: "date" | reverse %}
{% for post in wps %}
  {% include archive-single.html %}
{% endfor %}
