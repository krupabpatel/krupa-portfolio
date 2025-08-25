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
- [x] Refined color system with lavender as accent-only (not mixed in gradients)
- [x] Added sophisticated animations and visual effects
- [x] Changed navbar to "Krupa Patel" and greeting to "Hi, I'm Krupa"
- [x] Fixed hero section spacing and alignment issues
- [x] ~~Temporarily removed profile picture section (to be redesigned later)~~ Re-added profile picture
- [x] Updated hero subtitle to reflect PM aspirations and consulting background
- [x] Made subtitle italic for elegance
- [x] Fixed hero text left alignment and width matching
- [x] Made lavender bar automatically match title width (inline-block)
- [x] Added responsive scaling with clamp() for all hero elements
- [x] Changed CTA button to "Connect" with LinkedIn icon
- [x] Linked button to LinkedIn profile (krupa-b-patel)
- [x] Made LinkedIn icon scale with button text
- [x] Added gradient fade to lavender accent bar
- [x] Re-implemented profile picture with two-column hero layout
- [x] Added mobile hamburger menu with slide-in navigation
- [x] Fixed mobile responsive issues with hero section
- [x] Addressed navbar overlapping hero text on mobile (partial fix)
- [x] Fixed mobile profile image cutoff issue
- [x] Set overflow: visible on hero section for mobile
- [x] Adjusted mobile image container spacing with percentage-based padding
- [x] Converted all CSS units to rem/em for better responsiveness
- [x] **Enhanced Hero Section Interactivity**
  - Added Contact button with mail icon alongside LinkedIn Connect button
  - Implemented smooth profile picture hover scaling with enhanced shadow
  - Created layered 3D hover effect for profile decoration with independent timing
  - Added subtle opacity breathing animation to profile decoration background
  - Improved button text positioning with slight vertical adjustment
- [x] **Mobile UX Improvements** 
  - Fixed hero title spacing on mobile to match proportional bottom spacing
  - Centered Connect/Contact buttons on mobile screens for better alignment
- [x] **Background Animation Refinements**
  - Replaced problematic rotating gradient that caused harsh edges
  - Implemented smooth static gradient background with radial overlays
  - Maintained elegant visual depth without distracting movement
- [x] **GitHub Pages Deployment & Asset Loading Fixes**
  - Fixed Jekyll compatibility by switching to github-pages gem
  - Corrected baseurl configuration for GitHub Pages subdirectory deployment
  - Updated all asset paths to use Jekyll's relative_url filter
  - Resolved font loading issues by removing spaces from font filenames
  - Added font and image preloading to prevent flash of unstyled content
  - Optimized font-display strategy to reduce layout shifts

## Next Steps
1. ~~Create basic Jekyll structure~~ ✅ Complete
2. ~~Build simple HTML layout~~ ✅ Complete  
3. ~~Add clean CSS styling~~ ✅ Complete
4. **Profile Image Section** ✅ Complete
   - Implemented two-column hero layout with profile image
   - Added responsive mobile layout with proper scaling
5. Configure Decap CMS for content management
6. Add real project content and descriptions
7. Create individual project pages
8. Add About section with more details
9. Implement contact form functionality
10. Test content editing workflow
11. Optimize for GitHub Pages deployment
12. Add SEO meta tags and Open Graph data

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

### CSS Unit Guidelines (IMPORTANT)
- **Use rem units for most measurements** - Relative to root, more predictable
- **Use em units for media queries** - Better browser support
- **Keep 1-2px borders as px** - These are meant to be hairline borders
- **Base font size**: 1rem = 16px (browser default)
- **Conversion reference**: Divide px by 16 to get rem value
- **Media queries**: Use em units (e.g., 48em for 768px breakpoint)
- **All clamp() functions converted to rem** for consistency
- This ensures proper scaling and accessibility across all devices

### Color Palette (Earthy Tones)
- **Primary (Sand/Yellow-Tan)**: #E4D5B7 - Main brand color, warm and inviting
- **Secondary (Sage/Leaf Green)**: #8B956D - Natural, grounding color for key elements  
- **Accent (Lavender)**: #A594B8 - Used SPARINGLY for contrast and highlights only
- **Background**: Cream (#FBF9F4) - Warm, natural background
- **Text**: Charcoal (#2B2922) - Rich dark text color
- **Supporting Colors**: 
  - Warm Gray (#6B645C) - Subtle text
  - Sage Dark (#6B7752) - Darker green variant
  - Sand Dark (#D4C4A0) - Deeper sand tone

### Color Usage Rules (IMPORTANT)
- **Lavender is strictly for accents** - Never mixed in gradients with sand/sage
- **Sand and sage can be paired together** in gradients and combinations
- **Lavender usage limited to**:
  - Navigation hover underlines
  - Hero heading accent bar  
  - Project card top accent on hover
  - CTA button (Book Consultation)
  - Contact section secondary button hover state
- **Primary buttons**: Sand background → Sage on hover (no lavender)
- **Secondary buttons**: Sage background → Lavender on hover (accent contrast)

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

### Visual Design Elements & Animations
- **Hero Section**:
  - Animated rotating conic gradients in background
  - Floating geometric shapes (sand and sage only)
  - Lavender accent bar under main heading (fades to transparent)
  - Two-column layout with text on left, profile image on right
  - Italic subtitle for professional elegance
  - LinkedIn Connect button with scaling icon
- **Buttons**:
  - Pill-shaped with smooth cubic-bezier transitions
  - Expanding overlay effects on hover
  - Dynamic shadows and scale transforms
- **Project Cards**:
  - Shimmer effect with sliding gradient on hover
  - Lavender accent strip that scales in on hover
  - Staggered fade-in animations on load
  - Enhanced depth with multiple shadow layers
- **Typography Effects**:
  - Shadow effects on section titles for depth
  - Decorative elements using data-text attributes
- **Background Patterns**:
  - Subtle diagonal stripe overlays
  - Multiple layered radial gradients
  - Floating orbs with single-color gradients (no color mixing)

### Current Development Command
- `/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll serve --force_polling`
- Site accessible at http://127.0.0.1:4000/

## Notes
- Keep design clean and minimal like the demo site
- Focus on usability for content updates
- Ensure mobile responsiveness