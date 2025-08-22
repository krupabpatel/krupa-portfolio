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
- [x] Successfully installed Jekyll and dependencies on ARM64 Mac
- [x] Resolved eventmachine compilation issues using C++ compiler flags
- [x] Jekyll server running at http://127.0.0.1:4000/
- [x] Built complete portfolio design from scratch with earthy color palette
- [x] Integrated local Rinjani Sans fonts (Regular, Semibold, Bold)
- [x] Implemented sophisticated typography system
- [x] Created wide, full-width layout design
- [x] Added Funnel Display as body font paired with Rinjani Sans

## Next Steps
1. ~~Create basic Jekyll structure~~ ✅ Complete
2. ~~Build simple HTML layout~~ ✅ Complete  
3. ~~Add clean CSS styling~~ ✅ Complete
4. Add Krupa's profile image to `/assets/images/profile.jpg`
5. Configure Decap CMS for content management
6. Test content editing workflow
7. Add real project content and descriptions
8. Optimize for GitHub Pages deployment

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

### ARM64 Mac (M1/M2) Installation Issues & Fixes
**Problem**: EventMachine gem fails to compile with "iostream not found" error on ARM64 Macs

**Root Cause**: EventMachine's native extensions have C++ compilation issues on ARM64 architecture due to missing C++ standard library headers

**Solution**: Install eventmachine with specific C++ compiler flags:
```bash
/opt/homebrew/opt/ruby/bin/gem install eventmachine -v '1.2.7' -- --with-cppflags="-I$(brew --prefix)/include -I$(xcrun --show-sdk-path)/usr/include/c++/v1" --with-ldflags="-L$(brew --prefix)/lib"
```

**Additional Required Gems** (installed individually):
- `gem install jekyll` - Main Jekyll gem
- `gem install minima` - Default Jekyll theme
- `gem install jekyll-feed` - RSS feed plugin (installed with minima)
- `gem install jekyll-sitemap` - Sitemap plugin

**Working Jekyll Command**:
- `/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll serve --force_polling`

**Note**: Bundle install still fails even after configuring build flags, so gems must be installed individually and Jekyll run directly

## Design System Implemented

### Color Palette (Earthy Tones)
- **Main**: Sand (#E4D5B7) - warm, sophisticated primary color
- **Secondary**: Sage (#8B956D) - deep, natural green for headings
- **Accent**: Lavender (#A594B8) - refined purple for buttons
- **Background**: Cream (#FBF9F4) - warm, natural background
- **Text**: Charcoal (#2B2922) - rich dark text color

### Typography System
- **Headlines & Titles**: Rinjani Sans (local fonts)
  - Regular (400), Semibold (600), Bold (700) weights
  - Art Deco character, wide letterforms
  - Used for main headings and section titles
- **Body Text & UI**: Funnel Display (Google Fonts)
  - Modern, condensed, variable weight (300-800)
  - Excellent readability and contemporary feel
  - Perfect contrast with Rinjani Sans

### Font Integration
- **Local Rinjani Sans fonts** stored in `/assets/fonts/`
  - Rinjani.otf, Rinjani Semibold.otf, Rinjani Bold.otf
  - RinjaniRegular.ttf, RinjaniSemibold.ttf, RinjaniBold.ttf
  - Proper @font-face declarations with fallbacks
- **Google Fonts**: Funnel Display with full weight range

### Layout System
- **Wide, full-width design** (not centered containers)
- **Dramatic spacing** and generous padding
- **Sophisticated grid systems** for projects and content
- **Mobile-responsive** with maintained visual impact

### Current Development Command
- `/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll serve --force_polling`
- Site accessible at http://127.0.0.1:4000/

## Notes
- Keep design clean and minimal like the demo site
- Focus on usability for content updates
- Ensure mobile responsiveness