---
title: Documenting native library APIs overview
permalink: /nativelibraryapis.html
sidebar: docapis
---

{% assign doclist = site.docs | sort: 'weight'  %}
{% for page in doclist %}
{% if page.section == "nativelibraryapis" %}
<h1 id="{{page.permalink | remove: ".html" | remove: "/"}}">{{page.title}}</h1>
{{page.content}}
{% endif %}
{% endfor %}
