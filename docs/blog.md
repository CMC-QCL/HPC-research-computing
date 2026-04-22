---
layout: page
title: Blog
permalink: /blog/
---

Stories, updates, and practical guidance from the Claremont McKenna College Quantitative and Computing Lab High-Performance Computing (HPC) for Research program.

{% if site.posts and site.posts.size > 0 %}
## Recent Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %-d, %Y" }}
{% endfor %}
{% else %}
No posts yet. Use the template in templates/blog-post-template.md to create your first post.
{% endif %}