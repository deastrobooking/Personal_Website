---
title: "Getting Started with Jekyll and GitHub Pages"
date: 2025-09-29
tags: [jekyll, github-pages, web-development]
excerpt: "Learn how to create a professional blog using Jekyll and deploy it for free with GitHub Pages."
---

# Getting Started with Jekyll and GitHub Pages

Jekyll is a fantastic static site generator that powers GitHub Pages, making it perfect for developers who want to create a professional blog or portfolio site. In this guide, I'll walk you through the essentials of building and deploying a Jekyll site.

## What is Jekyll?

Jekyll is a static site generator written in Ruby. It takes your content written in Markdown, applies layouts and templates, and generates a complete static website that can be served from any web server.

## Setting Up Your Environment

First, you'll need to install Ruby and Jekyll on your system:

```bash
# Install Ruby (if not already installed)
# On macOS with Homebrew:
brew install ruby

# Install Jekyll and Bundler
gem install jekyll bundler

# Create a new Jekyll site
jekyll new my-awesome-site
cd my-awesome-site

# Install dependencies
bundle install

# Serve the site locally
bundle exec jekyll serve
```

## Project Structure

A typical Jekyll site has this structure:

```
├── _config.yml          # Site configuration
├── _posts/              # Blog posts
├── _layouts/            # HTML templates
├── _includes/           # Reusable components  
├── _sass/               # Sass stylesheets
├── assets/              # CSS, JS, images
├── index.md             # Homepage
└── Gemfile              # Ruby dependencies
```

## Writing Your First Post

Create a new file in the `_posts` directory with the naming convention `YYYY-MM-DD-title.md`:

```markdown
---
title: "My First Post"
date: 2025-09-29
categories: [blog, tutorial]
tags: [jekyll, markdown]
---

# Welcome to my blog!

This is my first post using Jekyll. Here's some **bold text** 
and some `inline code`.

## Code Example

```python
def hello_world():
    print("Hello, Jekyll!")
    
hello_world()
```

That's it! Jekyll makes blogging with Markdown incredibly simple.
```

## GitHub Pages Deployment

The beauty of Jekyll is that GitHub Pages supports it natively:

1. Create a new repository named `username.github.io`
2. Push your Jekyll site to the `main` branch
3. Enable GitHub Pages in repository settings
4. Your site will be available at `https://username.github.io`

## Advanced Features

Jekyll offers many powerful features:

- **Collections**: Organize content beyond blog posts
- **Data Files**: Store data in YAML, JSON, or CSV files
- **Plugins**: Extend functionality with gems
- **Themes**: Use pre-built designs or create your own

## Conclusion

Jekyll and GitHub Pages provide an excellent platform for technical blogging. The combination of Markdown writing, version control, and free hosting makes it ideal for developers and researchers.

Happy blogging! 🚀