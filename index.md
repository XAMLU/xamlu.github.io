---
layout: default
---

## Welcome to the XAMLU Site

Oredev attendees - one day intro course materials can be found [here](./one-day-intro/readme.md)

### Current Repositories

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}