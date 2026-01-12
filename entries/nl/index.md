---
language: nl
title: Dutch Knowledge Base
---

{% assign entries = site.pages
    | where_exp: "p", "p.path contains 'entries/'" + page.language + "/"
    | group_by_exp: "p", "p.path | split: '/' | slice: 2, 1" %}

{% for group in entries %}
{% unless group.name[0] == 'index.md' %}
<h2>{{ group.name[0] | capitalize | replace: '-', ' ' }}</h2>

{% assign entry_pages = group.items | sort: 'path' %}
{% for page in entry_pages %}
- [{{ page.title | capitalize }}](/{{ page.path | replace: '.md', '' }})
{% endfor %}

{% endunless %}
{% endfor %}
