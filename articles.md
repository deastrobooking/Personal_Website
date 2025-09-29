---
layout: default
title: Research Articles
permalink: /articles/
---

# Research Articles

A collection of in-depth technical articles, research papers, and mathematical analysis.

<div class="post-list">
  {% for article in site.articles %}
    <article class="post-preview">
      <h2><a href="{{ article.url | relative_url }}">{{ article.title }}</a></h2>
      <p class="post-meta">
        {{ article.date | date: "%B %d, %Y" }}
        {% if article.category %}
          • <span class="category">{{ article.category }}</span>
        {% endif %}
        {% if article.tags.size > 0 %}
          • 
          {% for tag in article.tags %}
            <span class="tag">{{ tag }}</span>
            {% unless forloop.last %}, {% endunless %}
          {% endfor %}
        {% endif %}
      </p>
      {% if article.abstract %}
        <div class="post-excerpt">
          <strong>Abstract:</strong> {{ article.abstract }}
        </div>
      {% endif %}
    </article>
  {% endfor %}
</div>

{% if site.articles.size == 0 %}
  <p>No research articles yet. Check back soon!</p>
{% endif %}