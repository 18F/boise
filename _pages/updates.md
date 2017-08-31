---
---

We will try to post a project update here weekly. If you'd like to get notified via email, send a message to [{{ site.contact_email }}](mailto:{{ site.contact_email }}).

{% for post in site.posts %}
## [{{ post.date | date: "%b %w, %Y" }}]({{ post.url }})

{{ post.excerpt }} [...]({{ post.url }})
{% endfor %}
