---
layout: page
title: "Projects"
permalink: /projects/
---

## All Projects

{% for project in site.projects %}
### [{{ project.title }}]({{ project.url }})
![Image]({{ project.image }})  
{{ project.excerpt | markdownify }}
{% endfor %}
