# Krupa Portfolio Project

## Project Overview
- Creating a simple, beautiful portfolio website for Krupa
- Will be hosted on GitHub Pages with Jekyll
- Using Decap CMS for no-code content management
- Design inspiration: https://adri-fluid-demo.squarespace.com (clean, modern, grid-based layout)

## Goals
- Simple, elegant design
- Easy for non-technical user to update content
- Mobile responsive
- Professional portfolio showcase

## Tech Stack
- Jekyll (for GitHub Pages compatibility)
- HTML/CSS (keeping it simple)
- Decap CMS for content management
- GitHub Pages for hosting

## Work Completed
- [x] Initial project setup
- [x] Created CLAUDE.md for tracking

## Next Steps
1. Create basic Jekyll structure
2. Build simple HTML layout
3. Add clean CSS styling
4. Configure Decap CMS
5. Test content editing workflow

## Commands to Remember
### Setup (run once)
- `brew install ruby` - Install Ruby via Homebrew (if needed)
- `/opt/homebrew/opt/ruby/bin/gem install bundler` - Install Bundler with Homebrew Ruby
- `BUNDLE_PATH=vendor/bundle /opt/homebrew/opt/ruby/bin/bundle install` - Install Jekyll dependencies locally

### Development (if bundle install works)
- `/opt/homebrew/opt/ruby/bin/bundle exec jekyll serve` - Run local development server
- `/opt/homebrew/opt/ruby/bin/bundle exec jekyll serve --livereload` - Run with auto-refresh

### Alternative (if bundle install fails)
- `/opt/homebrew/opt/ruby/bin/jekyll serve --force_polling` - Run with direct Jekyll (no live reload)
- `python3 -m http.server 4000` - Simple HTTP server for static files

### Ruby Setup Notes
- Project uses Ruby 3.4.5 (specified in .ruby-version)
- Uses Homebrew Ruby to avoid system Ruby permission issues
- Gems installed locally in vendor/bundle to avoid conflicts

## Notes
- Keep design clean and minimal like the demo site
- Focus on usability for content updates
- Ensure mobile responsiveness