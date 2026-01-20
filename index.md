---
layout: default
title: Home
---

# Welcome to Our Knowledge Base

{% assign category_groups = site.pages | where_exp: "page", "page.path contains '_categories/'" | group_by_exp: "page", "page.path | split: '/' | slice: 1, 1" %}

{% for category_group in category_groups %}
## {{ category_group.name | capitalize | replace: '-', ' ' }}

{% assign category_pages = category_group.items | sort: 'path' %}
{% for page in category_pages %}
- [{{ page.title | default: page.path | split: '/' | last | replace: '.md', '' | capitalize }}](/{{ page.path | remove_first: '_' | replace: '.md', '' }})
{% endfor %}

{% endfor %}
