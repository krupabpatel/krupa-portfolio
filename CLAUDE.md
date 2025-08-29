# Krupa Portfolio Project

## Overview
Portfolio website for Krupa hosted on GitHub Pages with Jekyll and Decap CMS for content management.

## Tech Stack
- Jekyll (GitHub Pages)
- HTML/CSS
- Decap CMS
- Local Rinjani Sans fonts + Google Fonts (Funnel Display)

## Current Status
✅ **Complete Portfolio Implementation**
- Full-width earthy design with sophisticated animations
- Mobile-responsive with hamburger menu and touch animations
- Hero section with profile picture, Connect/Contact buttons
- Project cards with hover effects and scroll-triggered animations
- Professional footer with glass morphism styling
- Navbar with social icons and smooth navigation
- Complete Resume section with timeline and skills grid
- Project template system with media carousel and document links
- Universal fade page transitions
- Scroll-triggered animations on both desktop and mobile
- Complete favicon system with multi-platform support

## Key Features Completed
- **Design System**: Earthy color palette (Sand #E4D5B7, Sage #8B956D, Lavender #A594B8)
- **Typography**: Rinjani Sans headlines + Funnel Display body text
- **Animations**: Scroll-triggered reveals, hover effects, touch animations
- **Navigation**: Smooth scrolling, fade transitions, mobile menu
- **Content Management**: Jekyll layouts, front matter schemas, CMS-ready templates
- **Mobile UX**: Touch animations, responsive scaling, hamburger menu
- **Favicon System**: Multi-size support (16px, 32px, 180px, 192px, 512px), ICO format, web manifest

## Project Structure
- `_layouts/project.html` - Jekyll template for project pages
- `project-template.html` - Decap CMS baseline template
- `project-1.html` - Example project implementation
- `assets/images/favicon-*.png` - Multi-size favicon files (16, 32, 180, 192, 512px)
- `favicon.ico`, `site.webmanifest` - Root-level favicon and PWA manifest
- Hero, Projects, Resume, Footer sections on homepage

## Commands
### Development
```bash
/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll serve --config _config.yml,_config_dev.yml --force_polling
```
- Local: http://127.0.0.1:4000/
- Production: https://krupabpatel.github.io/krupa-portfolio/

### Ruby Setup (ARM64 Mac)
```bash
/opt/homebrew/opt/ruby/bin/gem install eventmachine -v '1.2.7' -- --with-cppflags="-I$(brew --prefix)/include -I$(xcrun --show-sdk-path)/usr/include/c++/v1" --with-ldflags="-L$(brew --prefix)/lib"
```

## Design Guidelines
- **CSS Units**: Use rem/em, avoid px except for hairline borders
- **Color Rules**: Lavender only for accents, never mixed in gradients
- **Animation**: Scroll-triggered reveals, fade transitions, touch feedback
- **Responsive**: Mobile-first with clamp() scaling

## Next Steps
1. ✅ Configure Decap CMS - Dynamic project cards and content management
2. Add real project content
3. SEO optimization
4. Content editing workflow testing

## CMS Integration Status
✅ **Dynamic Project System**
- Homepage automatically generates project cards from `_projects` collection
- Project cards display `summary` field, project pages display markdown `content`
- URL slug field for customizable project URLs (e.g., `/projects/e-commerce-test/`)
- Proper separation of card preview vs. page content
- Jekyll config updated to use slug-based permalinks
- Unified `media` array supporting images, videos, and Figma embeds
- File upload support for both media and document links

## Key Technical Features
- **Intersection Observer**: Scroll-triggered animations
- **Jekyll Filters**: GitHub Pages asset path compatibility  
- **CSS Custom Properties**: Dynamic navbar height
- **Touch Events**: Mobile interaction animations
- **Document Links**: Professional project resource system
- **Multi-Platform Favicons**: Cross-browser/device compatibility with PWA support