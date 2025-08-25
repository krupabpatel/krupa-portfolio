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
- [x] **Navbar & Mobile UX Enhancements**
  - Increased "Krupa Patel" navbar size from 1.25rem to 1.5rem for better visibility
  - Maintained semibold (600) font weight for professional appearance
  - Updated all mobile breakpoint sizes proportionally for consistency
  - Fixed mobile horizontal overflow issue caused by rotating background elements
  - Added overflow-x: hidden to both html and body to prevent unwanted scrolling
- [x] **Dynamic Navbar Height Solution (Ultra-robust)**
  - Implemented JavaScript solution to dynamically measure actual navbar height
  - Created CSS custom property --header-height with 5rem fallback
  - Updated hero positioning to use calc(var(--header-height) + responsive-padding)
  - Added resize and load event listeners for real-time updates
  - Ensures hero text never gets cut off across all viewports, zoom levels, and content changes
  - Works with desktop (margin-top) and mobile (padding-top) layouts
  - Maintains responsive spacing ratios while preventing navbar overlap
- [x] **Desktop Spacing Optimization**
  - Fixed excessive gap between navbar and hero section on desktop view
  - Simplified desktop hero positioning to use only var(--header-height)
  - Removed extra clamp(1rem, 3vh, 2rem) spacing that was creating unwanted gap
  - Maintained mobile responsive spacing which was already working correctly
  - Ensures clean, professional appearance with proper navbar-to-content flow
- [x] **Mobile Scroll-Triggered Animations**
  - Implemented Intersection Observer API for scroll-based project card animations
  - Mobile-only detection using CSS media queries `@media (hover: none) and (pointer: coarse)`
  - Bidirectional animations that trigger when scrolling cards into/out of viewport
  - Full hover effects applied on scroll: shimmer, lavender accent bar, shadows, scaling
  - Staggered animation delays maintain elegant timing from desktop version
  - Seamless transition between desktop hover and mobile scroll interactions
- [x] **Content and Typography Updates**
  - Changed "Selected Work" to "Projects" in section title and navbar
  - Updated Projects section subtitle to focus on PM side projects and user research
  - Made section subtitle font size match hero subtitle for consistency across viewports
  - Optimized section subtitle width for better line wrapping (3-line layout)
  - Enhanced section title background text effect with better positioning and opacity
  - Increased mobile title sizes for both hero and Projects sections for better readability
- [x] **Project Cards Redesign**
  - Updated project cards with placeholder content (Project 1, 2, 3)
  - Enhanced title line-height to support multi-line titles
  - Experimented with lavender divider animations (removed due to mobile touch conflicts)
  - Maintained mobile touch animations for project card interactions
  - Preserved hover effects and shimmer animations on desktop
- [x] **Enhanced Mobile Touch Animations (Bidirectional)**
  - Fixed mobile touch animations to properly revert when finger is lifted
  - Converted project card animations from delayed (300ms) to immediate bidirectional response
  - Added comprehensive touch animations to all hero section interactive elements:
    - Connect button (LinkedIn) with color change, scaling, shadows, background overlay
    - Contact button (Email) with same hover-equivalent effects
    - Profile picture with image scaling and enhanced shadow effects
  - Disabled desktop hover states on mobile to prevent interference
  - Enhanced CSS transitions with proper timing and easing for mobile performance
  - Added development-only console logging for debugging touch interactions
  - All mobile touch interactions now provide immediate visual feedback with instant revert
- [x] **Project Template System Implementation**
  - Created comprehensive Jekyll project layout (_layouts/project.html)
  - Built project template page (project-template.html) as Decap CMS baseline
  - Implemented Project 1 individual page with realistic PM content
  - Updated project cards with proper linking structure
  - Established complete front matter schema for future CMS integration
- [x] **Project Page Complete Redesign (MAJOR UPDATE)**
  - **Removed body content section entirely** - No more markdown content area
  - **Added document links section** for PRD documents and resources
  - **Implemented responsive role/tools scaling** with proportional vw-based sizing
  - **Fixed spacing between role and tools** to scale down on mobile (8px → 4px)
  - **Created custom document icon** with proper paper proportions (20:16 aspect ratio)
  - **Optimized icon thickness** to match text weight across all viewports
  - **Added sophisticated hover effects** for document links with sage green theming
  - **Established new front matter structure** for links array with title, description, url, external flag
- [x] **Document Links System Architecture**
  - **Document-focused design**: Only for documents, not general links
  - **SVG icon system**: Custom paper icon with 3 horizontal lines, optimized thickness
  - **Responsive scaling**: Icon size clamp(1.5rem, 3vw, 2rem) scales perfectly with text
  - **Professional styling**: Sage green hover effects, smooth animations, proper visual hierarchy
  - **Flexible template**: Supports unlimited documents via Decap CMS array structure
- [x] **Universal Page Slide Transitions (MAJOR UX ENHANCEMENT)**
  - **Intelligent Navigation Detection**: Distinguishes between same-page (hash) and page-to-page navigation
  - **Horizontal Slide Animations**: Smooth slide transitions for page-to-page navigation only
  - **Directional Logic**: Homepage to project (slide right), project to homepage (slide left)
  - **Same-page Navigation Preserved**: Hash links maintain natural browser scrolling behavior
  - **Referrer-based Entry Animation**: Detects navigation source and applies appropriate slide direction
  - **Performance Optimized**: Animations only trigger for actual page changes, not refreshes
  - **Development Logging**: Console debugging for navigation flow understanding
  - **CSS Architecture**: Universal page container with slide classes for consistent transitions
  - **Enhanced UX**: Professional transitions that enhance navigation without interfering with anchors
- [x] **Critical Bug Fixes (Page Transitions & GitHub Pages)**
  - **Fixed Double Animation Twitching**: Resolved screen twitching when clicking "Krupa Patel" from project pages
  - **Improved Animation Cleanup**: Added proper clearAllAnimationClasses() function to prevent conflicts
  - **Enhanced Animation Timing**: Replaced setTimeout with requestAnimationFrame for smoother transitions
  - **Automatic Class Cleanup**: Animation classes automatically removed after 450ms to prevent state conflicts
  - **Fixed GitHub Pages 404 Error**: Corrected "Back to Projects" link using Jekyll relative_url filter
  - **Comprehensive Link Audit**: Verified all navigation links properly use Jekyll filters for GitHub Pages compatibility
  - **Cross-Environment Testing**: Confirmed fixes work in both local development and GitHub Pages deployment
- [x] **Dynamic Media Carousel System (MAJOR FEATURE)**
  - **Multi-Media Support**: Images, videos, and Figma embeds with proper responsive handling
  - **Absolute Positioning Architecture**: Fixed content cropping issues with overlay-based slide system
  - **Mobile-Optimized Design**: Proper viewport constraints (50vh desktop, 40vh mobile) with object-fit: contain
  - **Professional Navigation**: Arrow buttons and dot indicators positioned outside carousel frame
  - **Responsive Typography**: Proportionally scaling captions using clamp() functions
  - **Clean Visual Design**: Removed shadows from media, maintained frame shadows, proper spacing hierarchy
  - **Template Integration**: Complete front matter schema for Decap CMS with comprehensive examples
  - **Consistent Spacing**: Uniform margins between summary, carousel, and document links sections
  - **Vertical Alignment**: Media and captions properly centered within carousel container
  - **Performance Optimized**: Lazy loading, preload metadata, smooth transitions with GPU acceleration

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
- `/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll serve --config _config.yml,_config_dev.yml --force_polling` - Run with direct Jekyll for local development
- `/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll build` - Build for production (GitHub Pages builds automatically)
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
- `/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll serve --config _config.yml,_config_dev.yml --force_polling`
- Site accessible at http://127.0.0.1:4000/ (local development)
- GitHub Pages: https://krupabpatel.github.io/krupa-portfolio/ (production)

### Dynamic Configuration System
- **_config.yml**: Default GitHub Pages configuration (baseurl: "/krupa-portfolio", url: "https://krupabpatel.github.io")
- **_config_dev.yml**: Local development overrides (baseurl: "", url: "http://127.0.0.1:4000")  
- **Build commands**:
  - Local: `--config _config.yml,_config_dev.yml` (overrides for clean URLs)
  - Production: Automatic GitHub Pages build uses `_config.yml` directly

## Notes
- Keep design clean and minimal like the demo site
- Focus on usability for content updates
- Ensure mobile responsiveness

## Project Template System (For Decap CMS Integration)

### Overview
A comprehensive template system has been implemented to prepare for Decap CMS integration. This system provides a structured approach for creating individual project pages while maintaining design consistency and enabling content management.

### File Structure
```
/
├── _layouts/
│   └── project.html          # Jekyll layout template for all project pages
├── project-template.html     # Reference template for Decap CMS (visible page)
├── project-1.html           # Example project using the template
└── index.html               # Updated with project card links
```

### 1. Project Layout Template (_layouts/project.html)

**Purpose**: Jekyll layout that provides consistent structure and styling for all project pages

**Key Features**:
- Follows complete design system (colors, typography, spacing)
- Responsive design with mobile-first approach
- Sophisticated front matter integration
- Professional navigation and back-linking
- Comprehensive CSS styling integrated directly in layout

**Design Elements**:
- Hero section with project title, role, tools, and summary
- Dynamic media carousel supporting images, videos, and embeds
- Rich content area with proper typography hierarchy
- Project navigation (next/previous) for future use
- Back-to-projects navigation with smooth animations
- Full-width layout with lavender accent bar extending halfway across title

### 2. Project Template Page (project-template.html)

**Purpose**: Complete reference template that Decap CMS will use as baseline for new project creation

**Critical Role**: 
- **NOT meant for regular site navigation** - serves as Decap CMS template
- Shows complete front matter schema with all available fields
- Demonstrates content structure and formatting examples
- Includes comprehensive example content across all sections

**Front Matter Schema** (Simplified for side projects):
```yaml
---
layout: project                    # Always "project"
title: "Project Title"            # Required: Main project title
summary: "Brief description"      # Required: Subtitle/elevator pitch
role: "Your Role"                 # Optional: Your role in project
tools:                           # Optional: Array of tools/technologies
  - "Tool 1"
  - "Tool 2"
media:                           # Optional: Array of media items
  - type: "image"                # image, video, or embed
    src: "/path/to/media"
    alt: "Alt text"              # For images
    caption: "Caption text"      # Optional caption
  - type: "video"
    src: "/path/to/video.mp4"
    caption: "Video description"
  - type: "embed"
    embed: '<iframe src="..."></iframe>'
    caption: "Embed description"
next_project:                    # Optional: Navigation to next project
  title: "Next Project Title"
  url: "/project-next.html"
prev_project:                    # Optional: Navigation to previous project
  title: "Previous Project Title"
  url: "/project-previous.html"
---
```

**Content Structure Guidelines** (Simplified for side projects):
- **What I Built**: Brief overview and context
- **The Problem**: What specific issue you wanted to solve
- **My Approach**: How you tackled the challenge
- **Key Features**: Main functionality you implemented
- **What I Learned**: Personal and technical growth
- **Future Ideas**: Where you might take this next

### 3. Content Creation Guidelines for Decap CMS

**When Decap CMS is implemented**:

1. **New Project Creation**:
   - Decap CMS will use `project-template.html` as the baseline
   - All front matter fields will be available as form fields
   - Content structure will be pre-populated for easy editing

2. **Required Fields**:
   - `title`: Project name/title
   - `summary`: Brief description for project cards
   - Content body with proper markdown structure

3. **Optional but Recommended Fields**:
   - `role`: Your role in the project
   - `tools`: Technologies/tools used
   - `media`: Screenshots, videos, prototypes, or embeds

4. **Content Best Practices**:
   - Use markdown headers (##, ###) for proper hierarchy
   - Include quantifiable results where possible
   - Follow the established content structure
   - Keep summaries concise for project card display
   - Use professional tone aligned with PM/consulting background

### 4. Current Implementation Status

**Live Examples**:
- **Project 1**: `/project-1.html` - Complete example with realistic PM content
- **Template Reference**: `/project-template.html` - Comprehensive template showcase
- **Project Cards**: Updated with proper linking structure

**Project Card Linking**:
- Project 1 → Links to individual project page (`/project-1.html`)
- Project 2 → Links to template reference (`/project-template.html`) for testing
- Project 3 → Placeholder for future content

**Testing URLs** (Local Development):
- Template reference: `http://127.0.0.1:4000/project-template.html`
- Project 1 example: `http://127.0.0.1:4000/project-1.html`

### 5. Decap CMS Integration Instructions

**When ready to implement Decap CMS**:

1. **Configuration Setup**:
   - Create `admin/config.yml` with project collection configuration
   - Set `project-template.html` as the template file
   - Configure all front matter fields as form fields

2. **Collection Configuration Example**:
   ```yaml
   collections:
     - name: "projects"
       label: "Projects"
       folder: "/"
       create: true
       template: "project-template"
       fields:
         - {label: "Title", name: "title", widget: "string"}
         - {label: "Summary", name: "summary", widget: "text"}
         - {label: "Duration", name: "duration", widget: "string", required: false}
         - {label: "Role", name: "role", widget: "string", required: false}
         - {label: "Tools", name: "tools", widget: "list", required: false}
         - {label: "Featured Image", name: "featured_image", widget: "image", required: false}
         - {label: "Content", name: "body", widget: "markdown"}
   ```

3. **Workflow**:
   - Content creators use Decap CMS interface
   - New projects automatically follow template structure
   - All pages use consistent design and layout
   - Project cards automatically populate with new content

### 6. Maintenance Guidelines

**File Management**:
- Keep `project-template.html` updated as the definitive reference
- All new projects should follow the established front matter schema
- Update project card links when adding new projects
- Maintain design system consistency across all project pages

**Content Standards**:
- Focus on PM/consulting relevant projects
- Include quantifiable outcomes where possible
- Maintain professional tone and structure
- Use the template content structure as a guide

This template system ensures that when Decap CMS is integrated, content creation will be streamlined, consistent, and aligned with the overall design system while providing maximum flexibility for showcasing diverse project types.

## Document Links System (MAJOR FEATURE)

### Overview
A sophisticated document management system has been implemented to replace the previous markdown content area. This system focuses exclusively on linking to important project documents like PRDs, research findings, and prototypes.

### Core Architecture

**Front Matter Structure**:
```yaml
links:
  - title: "Document Title"
    description: "Brief description of document contents"
    url: "/path/to/document.pdf"
    external: false  # or true for external links
```

**Design Principles**:
- **Document-only focus**: Specifically designed for PDFs, prototypes, and research documents
- **Professional presentation**: Clean, business-appropriate styling with sage green theming
- **Responsive scaling**: All elements scale proportionally across viewport sizes
- **Accessibility**: Proper alt text, ARIA labels, and keyboard navigation support

### Visual Design System

**Custom Document Icon**:
- **SVG-based**: Custom paper icon with proper document proportions (20:16 aspect ratio)
- **Three horizontal lines**: Represents text content within the document
- **Optimized thickness**: Lines scaled to match text weight at all viewport sizes
- **Sage green color**: Matches design system (#8B956D)
- **Responsive sizing**: `clamp(1.5rem, 3vw, 2rem)` ensures perfect scaling

**Layout & Styling**:
- **Left-aligned icon**: Document icon on left, content on right
- **Vertical centering**: Icon perfectly centered with text content
- **Hover effects**: Smooth lift animation, enhanced shadows, color transitions
- **Typography**: Funnel Display font with responsive clamp() sizing
- **Spacing**: All gaps and margins use vw-based responsive units

### Implementation Details

**Responsive Role/Tools Scaling** (Fixed Issue):
- **Problem**: Role and tools elements weren't scaling proportionally
- **Solution**: Implemented vw-based clamp() functions for all dimensions
- **Result**: Perfect scaling from mobile (18px) to desktop (22px) maintaining visual harmony

**Spacing Optimization** (Fixed Issue):
- **Problem**: Gap between role and tools was larger on mobile (24px) than desktop (8px)
- **Solution**: Removed conflicting media query overrides, implemented proportional spacing
- **Result**: Consistent 50% scaling ratio (8px desktop → 4px mobile)

**Icon Design Evolution**:
1. **Started with**: Generic file icon with fold
2. **Improved to**: Document with text lines but square proportions
3. **Optimized to**: Proper paper proportions with refined line thickness
4. **Final result**: Perfect document icon with 20:16 aspect ratio and optimal visual weight

### Decap CMS Integration Ready

**Template Configuration**:
- `project-template.html` serves as baseline for Decap CMS
- Front matter structure supports unlimited document links
- Each project can have 0-many document links
- External vs internal link support built-in

**Content Management Workflow**:
1. Content creator uses Decap CMS interface
2. Adds document links via form fields (title, description, URL, external flag)
3. System automatically generates styled document cards with icons
4. Consistent presentation across all projects maintained

### Technical Specifications

**CSS Implementation**:
```css
.link-icon {
  width: clamp(1.5rem, 3vw, 2rem);
  height: clamp(1.5rem, 3vw, 2rem);
  fill: #8B956D;
}

.project-link:hover {
  transform: translateY(-0.125rem);
  box-shadow: 0 0.25rem 1rem rgba(139, 149, 109, 0.15);
}
```

**HTML Structure**:
```html
<a href="{{ link.url }}" class="project-link">
  <svg class="link-icon"><!-- Custom document SVG --></svg>
  <div class="link-content">
    <span class="link-title">{{ link.title }}</span>
    <span class="link-description">{{ link.description }}</span>
  </div>
</a>
```

### Performance & UX Benefits

**Simplified Content Model**:
- Removed complex markdown content area (performance improvement)
- Focused on essential document linking (better UX)
- Reduced cognitive load for content creators
- Cleaner, more professional presentation

**Enhanced User Experience**:
- Clear visual hierarchy with document icons
- Immediate understanding of content type (documents)
- Professional presentation suitable for PM/consulting portfolio
- Mobile-optimized touch interactions

This Document Links System represents a major architectural shift from traditional blog-style content to a professional document-centric approach, perfectly suited for showcasing PM work, research findings, and project documentation.

## Universal Page Slide Transitions System (MAJOR UX ENHANCEMENT)

### Overview
A sophisticated page transition system has been implemented that provides smooth, professional navigation between pages while preserving natural browser behavior for same-page navigation. This system enhances the user experience without interfering with anchor links or normal page functionality.

### Core Architecture

**Navigation Intelligence**:
- **Same-page Detection**: Recognizes hash links (`#projects`, `/#contact`) and preserves natural scrolling
- **Page-to-page Detection**: Identifies navigation between different pages and applies slide animations
- **Referrer Analysis**: Uses `document.referrer` to determine navigation direction and source
- **Refresh Protection**: Prevents animations on page refreshes or direct navigation

**Slide Direction Logic**:
```javascript
// Homepage to project page = slide from right (content slides left)
// Project page to homepage = slide from left (content slides right)
```

### Technical Implementation

**HTML Structure**:
```html
<div class="page-container">
    <div class="page-content">
        {{ content }}
    </div>
</div>
```

**CSS Animation Classes**:
```css
/* Entry animations */
.page-slide-enter-from-right { transform: translateX(100%); opacity: 0; }
.page-slide-enter-from-left  { transform: translateX(-100%); opacity: 0; }
.page-slide-enter-active     { transform: translateX(0); opacity: 1; transition: 0.4s; }

/* Exit animations (for future enhancements) */
.page-slide-exit-to-left     { transform: translateX(-100%); opacity: 0; }
.page-slide-exit-to-right    { transform: translateX(100%); opacity: 0; }
```

**JavaScript Navigation Handler**:
- **Intelligent Link Detection**: Analyzes href attributes to categorize navigation type
- **Performance Optimization**: Only processes relevant navigation events
- **Development Logging**: Comprehensive console output for debugging navigation flow
- **Browser Compatibility**: Works with modern Navigation API and fallback methods

### Navigation Flow Examples

**Same-page Navigation** (No animation):
- `#projects` from homepage → Natural scroll to Projects section
- `/#contact` from homepage → Natural scroll to Contact section
- `Connect` button → Natural scroll to Contact section

**Page-to-page Navigation** (With slide animation):
- Homepage → Project 1 page → Slide from right (content slides left)
- Project 1 page → Homepage → Slide from left (content slides right)
- Project page → Back to Projects → Slide from left (content slides right)

### User Experience Benefits

**Professional Polish**:
- Smooth, modern transitions that feel native to high-end portfolios
- Directional consistency that provides spatial navigation context
- Enhanced perceived performance through smooth visual continuity

**Preserved Functionality**:
- Anchor links work exactly as expected (no JavaScript interference)
- Back/forward browser buttons maintain natural behavior
- Page refreshes don't trigger unwanted animations
- External links and same-page navigation remain unaffected

**Performance Optimized**:
- Animations only trigger when actually needed (page changes)
- Lightweight CSS-based animations with GPU acceleration
- No interference with existing touch animations or hover effects
- Minimal JavaScript overhead with intelligent event handling

### Technical Specifications

**Animation Timing**:
- **Duration**: 0.4 seconds for professional feel
- **Easing**: `cubic-bezier(0.25, 0.46, 0.45, 0.94)` for smooth, natural motion
- **Opacity**: Coordinated with transform for seamless transitions

**Browser Support**:
- **Modern Navigation API**: Primary detection method for page type
- **Performance API Fallback**: Legacy browser support for refresh detection
- **Referrer Analysis**: Universal browser support for navigation source detection

**Development Features**:
- **Console Logging**: Detailed navigation flow debugging (development only)
- **Error Handling**: Graceful fallbacks for parsing errors or edge cases
- **Extensibility**: Clean architecture for adding more transition types

### Future Enhancement Possibilities

**Exit Animations**: 
- Currently implements entry animations only
- Exit animation classes prepared for potential click-to-transition upgrades
- Could add coordinated exit/entry for seamless page-to-page flow

**Additional Transition Types**:
- Fade transitions for certain navigation patterns
- Vertical slides for different content relationships
- Custom animations based on specific page combinations

**Performance Monitoring**:
- Animation performance metrics
- User interaction analytics for transition effectiveness
- A/B testing framework for different transition styles

### Integration with Existing Systems

**Mobile Compatibility**:
- Works seamlessly with existing mobile hamburger menu
- Maintains touch animation performance
- Respects mobile-specific navigation patterns

**Project Template System**:
- All project pages benefit from consistent transition behavior
- Back-to-projects navigation provides intuitive spatial context
- Template inheritance ensures all pages participate in transition system

**Design System Alignment**:
- Animation timing matches existing hover and touch animations
- Transition easing complements overall design language
- No interference with established visual hierarchy or spacing

This Universal Page Slide Transitions System represents a major enhancement to the portfolio's user experience, providing the polish and sophistication expected in professional PM/consulting portfolios while maintaining all browser functionality and performance standards.

## Complete Page Transition System Overhaul (MAJOR REFACTOR - December 2024)

### Overview
After experiencing issues with the slide animation system (twitching, inconsistent behavior, browser back button problems), the entire page transition system was completely rebuilt with a simpler, more reliable approach using fade animations instead of slides.

### Changes Made

**1. Removed Complex Slide Animation System**
- Eliminated all horizontal slide transitions (translateX)
- Removed directional logic (left/right calculations)
- Cleaned up animation class management issues
- Fixed twitching and bouncing problems

**2. Implemented Cinematic Fade Transitions**
- **Simple opacity-based animations** (0 to 1 fade)
- **Consistent 0.3s duration** across all transitions
- **Universal application** to all internal navigation
- **Smooth ease-in-out timing** for professional feel

**3. Project Card Updates**
- Changed from `onclick` handlers to `data-href` attributes
- Ensures fade animations trigger properly
- Maintains clickable behavior and hover effects

**4. Browser Back/Forward Button Support**
- **Pageshow event handler** for back/forward navigation
- **Fade-in animation** when returning via back button
- **Prevents blank screen** during cache restoration
- **Consistent timing** with regular navigation

**5. Technical Implementation**
```javascript
// Fade-out on click
pageContent.style.opacity = '0';
setTimeout(() => window.location.href = href, 200);

// Fade-in on page load
pageContent.style.transition = 'none';
pageContent.style.opacity = '0';
pageContent.offsetHeight; // Force reflow
pageContent.style.transition = 'opacity 0.3s ease-in-out';
setTimeout(() => pageContent.style.opacity = '1', 10);
```

**6. Universal Navigation Support**
- Works with `<a>` links
- Works with `data-href` attributes
- Works with browser navigation
- Skips external links and anchor links

### Benefits of New System
- **Simpler**: No complex direction calculations
- **Reliable**: Consistent behavior across all browsers
- **Smoother**: No twitching or jumping
- **Universal**: Works with any navigation method
- **Maintainable**: Less code, easier to debug

### Final Animation Specifications
- **Duration**: 0.3s for all transitions
- **Fade-out delay**: 200ms before navigation
- **Fade-in delay**: 10ms for consistency
- **Cleanup**: 400ms to remove inline styles
- **Easing**: ease-in-out for natural motion