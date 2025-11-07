# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
This is a Jekyll-based academic personal website built on the Academic Pages template. It showcases Dr. Huaijun Qiu's research publications, teaching activities, and industrial experience. The site is hosted on GitHub Pages and uses the Minimal Mistakes theme.

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Serve the site locally with live reload
bundle exec jekyll serve --watch

# Serve on specific host and port
bundle exec jekyll serve --host 0.0.0.0 --port 4000
```

### Docker Development
```bash
# Build and run with Docker
docker build -t jekyll-site .
docker run -p 4000:4000 -v $(pwd):/usr/src/app jekyll-site
```

### Asset Building
```bash
# Install npm dependencies
npm install

# Build JavaScript assets
npm run build:js

# Watch JavaScript files for changes
npm run watch:js
```

## Site Architecture

### Jekyll Structure
- `_config.yml` - Main Jekyll configuration with site settings, author info, and collections
- `_layouts/` - Page templates (default, single, archive, talk)
- `_includes/` - Reusable components (head, footer, navigation, analytics)
- `_sass/` - Sass stylesheets organized by component
- `assets/` - CSS, JavaScript, fonts, and other static assets

### Content Collections
- `_pages/` - Static pages (about, publications, teaching, etc.)
- `_posts/` - Blog posts with date-based URLs
- `_publications/` - Research publications organized by year
- `_teaching/` - Teaching experiences and courses
- `_talks/` - Conference presentations and talks
- `_portfolio/` - Portfolio items (if used)

### Navigation
Main navigation is configured in `_data/navigation.yml` with links to:
- Publications
- Honors
- Teaching
- Students
- Academic
- Industrial
- News (blog archive)

### Key Features
- **Publication Categories**: Organized by type (books, manuscripts, conferences) as defined in `_config.yml`
- **Author Profile**: Comprehensive author information with academic and social links
- **Analytics**: Google Analytics 4 integration
- **Responsive Design**: Mobile-friendly layout using Minimal Mistakes theme
- **Docker Support**: Containerized development environment

### Content Management
- Publications use markdown files with YAML front matter
- Blog posts follow Jekyll's date-based naming convention
- Images stored in `/images/` directory
- PDF files in `/files/` directory

### Styling
- Main styles compiled from `assets/css/main.scss`
- Custom variables in `_sass/_variables.scss`
- Component-specific styles in individual `_sass/` files
- Font Awesome icons and Academicons for academic links

## Development Notes
- The site uses kramdown for markdown processing
- Timezone set to "Asia/Shanghai"
- Supports emoji via jemoji plugin
- Includes sitemap and feed generation
- HTML compression enabled in production