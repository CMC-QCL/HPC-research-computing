---
layout: page
title: Blog
permalink: /blog/
---

News and updates for CMC QCL research computing onboarding.

{% if site.posts and site.posts.size > 0 %}
## Recent Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %-d, %Y" }}
{% endfor %}
{% else %}
No posts yet. Use the template in templates/blog-post-template.md to create your first post.
{% endif %}