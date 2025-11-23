---
layout: coding
permalink: /coding
---

{% for post in site.categories.coding %}

## [{{ post.title }}]( {{ post.url | relative_url }})

### [{{ post.categories[0] | upcase }}] {{ post.date | date: "%d %B %Y "}}

{{ post.excerpt | markdownify | strip_html }}

{% endfor %}
