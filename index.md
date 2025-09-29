---
layout: home
title: Home
---

# Welcome to My Professional Portfolio

I'm a software developer passionate about creating innovative solutions and conducting meaningful research. This site showcases my coding projects and research articles, featuring:

## 🚀 What You'll Find Here

- **Technical Articles**: In-depth coding tutorials and best practices
- **Research Papers**: Academic and industry research with mathematical formulations
- **Project Showcases**: Detailed breakdowns of my development work
- **Code Examples**: Practical implementations and algorithms

## 🔬 Technical Focus Areas

- Software Development & Architecture
- Data Science & Machine Learning
- Mathematical Modeling & Analysis
- Open Source Contributions

---

## Recent Articles

{% for article in site.articles limit:3 %}
- [{{ article.title }}]({{ article.url | relative_url }}) - {{ article.date | date: "%B %d, %Y" }}
{% endfor %}

## Latest Blog Posts

{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

---

*This site supports full markdown rendering with syntax highlighting and LaTeX mathematical equations using MathJax.*