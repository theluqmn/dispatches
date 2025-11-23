---
layout: all
permalink: /
---

{% for post in site.posts %}

## [{{ post.title | upcase }}]( {{ post.url | relative_url }})

### [{{ post.categories[0] | upcase }}] {{ post.date | date: "%d %B %Y "}}

{{ post.excerpt | markdownify | strip_html }}

{% endfor %}
