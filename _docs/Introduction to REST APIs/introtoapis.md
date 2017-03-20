---
title: Introduction to REST APIs overview
permalink: /introtoapis.html
sidebar: docapis
---

{% assign doclist = site.docs | sort: 'weight'  %}
{% for page in doclist %}
{% if page.section == "introtoapis" %}
<h1 id="{{page.permalink | remove: ".html" | remove: "/"}}">{{page.title}}</h1>
{{page.content}}
{% endif %}
{% endfor %}
