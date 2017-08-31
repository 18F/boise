---
---

{% for post in site.posts %}
## [{{ post.date | date: "%b %w, %Y" }}]({{ post.url }})

{{ post.excerpt }} [...]({{ post.url }})
{% endfor %}
