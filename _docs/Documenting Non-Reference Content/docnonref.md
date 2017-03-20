---
title: Documenting non-reference sections overview
permalink: /docnonref.html
sidebar: docapis
---

{% assign doclist = site.docs | sort: 'weight'  %}
{% for page in doclist %}
{% if page.section == "docnonref" %}
<h1 id="{{page.permalink | remove: ".html" | remove: "/"}}">{{page.title}}</h1>
{{page.content}}
{% endif %}
{% endfor %}
