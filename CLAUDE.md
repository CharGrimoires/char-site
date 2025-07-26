# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll static site using the Minimal Mistakes theme, configured for GitHub Pages deployment. The site follows standard Jekyll conventions with Markdown content and front matter configuration.

## Common Commands

### Development
- `bundle exec jekyll serve` - Start development server with auto-regeneration
- `bundle exec jekyll build` - Build the site to `_site/` directory
- `bundle install` - Install Ruby gem dependencies

### Content Management
- Blog posts go in `_posts/` with naming format: `YEAR-MONTH-DAY-title.markdown`
- Pages can be created as `.markdown` files in the root directory
- Use front matter to set layout, title, permalink, and other metadata

## Site Architecture

### Key Files
- `_config.yml` - Main site configuration with Minimal Mistakes theme settings
- `Gemfile` - Ruby dependencies using github-pages and minimal-mistakes-jekyll
- `_data/navigation.yml` - Site navigation menu configuration
- `index.markdown` - Homepage using `home` layout with author profile
- `about.markdown` - About page using `single` layout

### Directory Structure
- `_posts/` - Blog posts with date-based naming
- `_pages/` - Static pages (posts.md, categories.md, tags.md)
- `_data/` - YAML data files for navigation and configuration
- `_site/` - Generated static site (excluded from version control)

### Theme and Styling
- Uses Minimal Mistakes theme via remote_theme for GitHub Pages compatibility
- Supports multiple skins: "default", "air", "aqua", "contrast", "dark", "dirt", "neon", "mint", "plum", "sunrise"
- Author profile configuration in `_config.yml` with bio, avatar, and social links
- Built-in layouts: `single`, `home`, `posts`, `categories`, `tags`

### GitHub Pages Configuration
- Uses `github-pages` gem for compatibility
- Remote theme: `mmistakes/minimal-mistakes@4.24.0`
- Includes required plugins: jekyll-paginate, jekyll-sitemap, jekyll-gist, jekyll-feed, jekyll-include-cache

### Content Format
- All content uses Markdown with YAML front matter
- Post defaults: `single` layout with author_profile, read_time, comments, share, related enabled
- Page defaults: `single` layout with author_profile enabled
- Pagination configured for 5 posts per page