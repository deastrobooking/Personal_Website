---
layout: default
title: Blog Posts
permalink: /blog/
---

# Blog Posts

Here you'll find my latest thoughts on software development, coding tutorials, and technical insights.

<div class="post-list">
  {% for post in site.posts %}
    <article class="post-preview">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p class="post-meta">
        {{ post.date | date: "%B %d, %Y" }}
        {% if post.tags.size > 0 %}
          • 
          {% for tag in post.tags %}
            <span class="tag">{{ tag }}</span>
            {% unless forloop.last %}, {% endunless %}
          {% endfor %}
        {% endif %}
      </p>
      {% if post.excerpt %}
        <div class="post-excerpt">
          {{ post.excerpt }}
        </div>
      {% endif %}
    </article>
  {% endfor %}
</div>

{% if site.posts.size == 0 %}
  <p>No blog posts yet. Check back soon!</p>
{% endif %}