# Krupa Portfolio Project

## Overview
Portfolio website for Krupa hosted on GitHub Pages with Jekyll and Sveltia CMS for content management.

## Tech Stack
- Jekyll (GitHub Pages), HTML/CSS, Sveltia CMS
- Local Rinjani Sans fonts + Google Fonts (Funnel Display)

## Status: Complete Portfolio Implementation ✅
- **Design**: Full-width earthy palette (Sand #E4D5B7, Sage #8B956D, Lavender #A594B8), sophisticated animations
- **Mobile**: Responsive with hamburger menu, touch animations, clamp() scaling
- **Homepage**: Hero section, project cards with hover effects, resume timeline, skills grid, glass morphism footer
- **Navigation**: Smooth scrolling, fade transitions, social icons
- **Projects**: Template system with media carousel, multiple icon types for links
- **Favicon**: Multi-platform support (16-512px, ICO, web manifest)

## Development Commands
```bash
# Local development
/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll serve --config _config.yml,_config_dev.yml --force_polling

# Ruby setup (ARM64 Mac)
/opt/homebrew/opt/ruby/bin/gem install eventmachine -v '1.2.7' -- --with-cppflags="-I$(brew --prefix)/include -I$(xcrun --show-sdk-path)/usr/include/c++/v1" --with-ldflags="-L$(brew --prefix)/lib"
```
- Local: http://127.0.0.1:4000/
- Production: https://krupabpatel.github.io/krupa-portfolio/

## Design Guidelines
- **CSS**: rem/em units, lavender accents only, no gradient mixing
- **Animation**: Scroll-triggered reveals, fade transitions, mobile-first

## Complete CMS Integration ✅
- **Projects**: `_projects` collection with slug URLs, summary/content separation, media carousel (images/videos/Figma), link icons (document/GitHub/hyperlink), reverse order sorting (higher numbers first)
- **Hero**: `_hero` collection with title/subtitle/image/contacts
- **Sections**: `_sections` collection for subtitle management  
- **Education**: `_education` collection with timeline, category/body pairs
- **Experience**: `_experience` collection with responsibilities, bullet rendering
- **Skills**: `_skills` collection with color themes (tan/lavender), tag generation

## Technical Features
- **Animations**: Intersection Observer scroll triggers, touch events, lavender carousel hovers
- **Jekyll**: GitHub Pages asset path filters, custom properties
- **Media**: Responsive carousel with controls, organized uploads
- **Icons**: Document/GitHub/hyperlink SVG system for project links
- **Typography**: Project content headers (Rinjani Sans), proper paragraph spacing, line height optimization
- **Content**: Markdown header support with visual hierarchy