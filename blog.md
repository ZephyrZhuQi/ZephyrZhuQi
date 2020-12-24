---
layout: page
# title: Blog
permalink: /_blog/
---


<!-- This is my blog. -->

<h1>Latest Posts</h1>

<ul>
  {% for post in site.posts %}
    {% if post.status == "visible" %}
      <li>
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        {{ post.excerpt }}
      </li>
    {% endif %}
  {% endfor %}
</ul>