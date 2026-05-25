---
layout: page
title: Projects
permalink: /projects/
---

# Trainee Projects

Browse all submitted Claude Code workshop projects below.

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

**Team:** {{ post.team }}

**Built with:** {{ post.tools }}

**Summary:** {{ post.summary }}

---
{% endfor %}
