---
title: Using an API like a developer
permalink: /likeadeveloper.html
sidebar: docapis
---
{% assign doclist = site.docs | sort: 'weight'  %}
{% for page in doclist %}
{% if page.section == "likeadeveloper" %}
<h1 id="{{page.permalink | remove: ".html" | remove: "/"}}">{{page.title}}</h1>
{{page.content}}
{% endif %}
{% endfor %}
