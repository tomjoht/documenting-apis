---
title: Documenting an endpoint overview
permalink: /docendpoints.html
sidebar: docapis
---

{% assign doclist = site.docs | sort: 'weight'  %}
{% for page in doclist %}
{% if page.section == "docendpoints" %}
<h1 id="{{page.permalink | remove: ".html" | remove: "/"}}">{{page.title}}</h1>
{{page.content}}
{% endif %}
{% endfor %}
