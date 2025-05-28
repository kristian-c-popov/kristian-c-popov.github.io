---
layout: home
title: "Welcome"
permalink: /
---

## Latest Projects

{% assign recent_projects = site.projects | sort: 'date' | reverse | slice: 0, 3 %}
{% for project in recent_projects %}
### [{{ project.title }}]({{ project.url }})
![Image]({{ project.image }})  
{{ project.excerpt | markdownify }}
{% endfor %}

[See all projects →](/projects)

---

## About Me

Hi, I’m Kristian — an engineer passionate about AI, robotics, and optimization. [Read more →](/aboutme)
