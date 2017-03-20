---
title: Exploring other APIs
permalink: /otherapis.html
sidebar: docapis
---

{% assign doclist = site.docs | sort: 'weight'  %}
{% for page in doclist %}
{% if page.section == "otherapis" %}
<h1 id="{{page.permalink | remove: ".html" | remove: "/"}}">{{page.title}}</h1>
{{page.content}}
{% endif %}
{% endfor %}
