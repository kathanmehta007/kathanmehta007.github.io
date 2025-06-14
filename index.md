---
layout: home
title: "Welcome"
hero:
  title: "Hi, I’m Kathan Nilesh Mehta"
  tagline: "AI Lead @ Satelytics | M.S. ECE from CMU"
  image: "/assets/images/hero-bg.jpg"
  actions:
    - title: "About Me"
      url: "/about/"
      style: "primary"
    - title: "Experience"
      url: "/experience/"
      style: "accent"
# Data sections to show on home page:
experience:
  data: experience
  limit: 3
projects:
  data: projects
  limit: 3
hobbies:
  data: hobbies
  limit: 5
---

Welcome to my corner of the web! I build AI-powered geospatial workflows and love hiking, photography,  
and cooking paneer tikka. Dive in to learn more:

## Recent Blog Posts

<ul class="latest-posts">
  {% for post in site.posts limit:3 %}
    <li>
      <time datetime="{{ post.date | date_to_xmlschema }}">
        {{ post.date | date: "%b %-d, %Y" }}
      </time>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
