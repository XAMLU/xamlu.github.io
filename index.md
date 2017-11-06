---
layout: default
---

## Welcome to the XAMLU Site

Welcome Oredev 2017 attendees - navigate to the course materials below:

<a href="./one-day-intro/readme.html" class="btnDark">One Day Intro</a>

## Learn more about the Team

<a href="./about-us.html" class="btnDark">About Us</a>

### Current Repositories

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}