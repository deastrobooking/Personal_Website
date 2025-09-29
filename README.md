# Professional Portfolio Website

A modern Jekyll-based personal website designed for showcasing coding projects and research articles. Built with GitHub Pages support, featuring markdown rendering with LaTeX mathematical equations.

## 🚀 Features

- **Jekyll Static Site Generator**: Fast, secure, and SEO-friendly
- **GitHub Pages Ready**: Deploy automatically with GitHub Pages
- **LaTeX/Math Support**: Render mathematical equations using MathJax
- **Syntax Highlighting**: Beautiful code highlighting with Rouge
- **Responsive Design**: Mobile-friendly with modern CSS
- **Blog & Articles**: Separate sections for blog posts and research articles
- **Professional Styling**: Clean, academic-style layout

## 📁 Project Structure

```
├── _config.yml              # Site configuration
├── Gemfile                  # Ruby dependencies
├── index.md                 # Homepage
├── about.md                 # About page
├── blog.md                  # Blog listing page
├── articles.md              # Articles listing page
├── _layouts/                # HTML templates
│   ├── default.html
│   ├── home.html
│   ├── post.html
│   └── article.html
├── _includes/               # Reusable components
│   ├── mathjax.html        # MathJax configuration
│   └── head-custom.html     # Custom head elements
├── _posts/                  # Blog posts
├── _articles/               # Research articles
├── _sass/                   # Sass stylesheets
└── assets/css/              # Compiled CSS
```

## 🛠️ Local Development

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler gem

### Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/deastrobooking/Personal_Website.git
   cd Personal_Website
   ```

2. **Install dependencies**:
   ```bash
   bundle install
   ```

3. **Serve locally**:
   ```bash
   bundle exec jekyll serve
   ```

4. **View your site**: Open [http://localhost:4000](http://localhost:4000)

### Development Commands

- `bundle exec jekyll serve` - Start development server
- `bundle exec jekyll serve --livereload` - Auto-refresh on changes
- `bundle exec jekyll build` - Build static site to `_site/`
- `bundle exec jekyll clean` - Clean the build directory

## 📝 Content Creation

### Writing Blog Posts

Create new files in `_posts/` with the naming convention: `YYYY-MM-DD-title.md`

```markdown
---
title: "Your Post Title"
date: 2025-09-29
tags: [tag1, tag2, tag3]
excerpt: "Brief description of your post"
---

# Your Post Title

Your content here with full markdown support...

```python
# Code blocks are fully supported
def hello_world():
    print("Hello, Jekyll!")
```
```

### Writing Research Articles

Create new files in `_articles/` with comprehensive front matter:

```markdown
---
title: "Research Article Title"
date: 2025-09-29
category: "Research Category"
tags: [mathematics, algorithms, research]
abstract: "Brief abstract of your research"
references:
  - "Author, A. (2025). Paper Title. Journal Name."
  - "Author, B. (2024). Another Paper. Conference Proceedings."
---

# Research Article Title

## Abstract
Your abstract here...

## Mathematical Content
LaTeX equations are fully supported:

Inline math: $E = mc^2$

Display math:
$$\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}$$

Your research content here...
```

### LaTeX/Math Support

The site includes MathJax for rendering mathematical equations:

- **Inline math**: Use `$equation$` or `\\(equation\\)`
- **Display math**: Use `$$equation$$` or `\\[equation\\]`
- **Equation numbering**: Supported with AMS extensions
- **Math environments**: `\begin{align}`, `\begin{matrix}`, etc.

Example:
```latex
$$
\begin{align}
\nabla \times \vec{F} &= \left( \frac{\partial F_z}{\partial y} - \frac{\partial F_y}{\partial z} \right) \mathbf{i} \\
&\quad + \left( \frac{\partial F_x}{\partial z} - \frac{\partial F_z}{\partial x} \right) \mathbf{j} \\
&\quad + \left( \frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y} \right) \mathbf{k}
\end{align}
$$
```

## 🚀 GitHub Pages Deployment

### Automatic Deployment

1. **Push to GitHub**: Your site will automatically build and deploy when you push to the `main` branch.

2. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` / (root)
   - Save

3. **Custom Domain** (optional):
   - Add a `CNAME` file with your domain
   - Configure DNS settings with your domain provider

### Manual Configuration

The site is pre-configured for GitHub Pages with:
- `github-pages` gem in Gemfile
- Compatible Jekyll version
- Proper base URL configuration

## 🎨 Customization

### Site Configuration

Edit `_config.yml` to customize:

```yaml
title: "Your Site Title"
email: your-email@example.com
description: "Your site description"
url: "https://yourusername.github.io"
github_username: yourusername
```

### Styling

- Modify `assets/css/style.scss` for custom styles
- Color scheme variables in CSS `:root` section
- Responsive breakpoints and typography settings

### Navigation

Add new pages by creating markdown files and updating the navigation in `_includes/header.html` (if using custom header) or through Jekyll's automatic navigation.

## 📚 Technologies Used

- **Jekyll 4.3+**: Static site generator
- **GitHub Pages**: Free hosting
- **MathJax 2.7**: Mathematical equation rendering
- **Rouge**: Syntax highlighting
- **Sass**: CSS preprocessing
- **Minima Theme**: Base theme (customized)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Support

If you have questions or need help:

1. Check the [Jekyll documentation](https://jekyllrb.com/docs/)
2. Review [GitHub Pages documentation](https://docs.github.com/en/pages)
3. Open an issue in this repository

## 🌟 Acknowledgments

- [Jekyll](https://jekyllrb.com/) for the amazing static site generator
- [MathJax](https://www.mathjax.org/) for beautiful math rendering
- [GitHub Pages](https://pages.github.com/) for free hosting
- [Minima](https://github.com/jekyll/minima) for the base theme

---

**Live Site**: [https://deastrobooking.github.io/Personal_Website](https://deastrobooking.github.io/Personal_Website)
