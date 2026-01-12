---
layout: default
title: Home
---

## Available Languages

{% for lang in site.languages %}
- [{{ lang | upcase }}](/entries/{{ lang }})
{% endfor %}
