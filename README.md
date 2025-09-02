# Krupa Portfolio

A sophisticated portfolio website showcasing an earthy design system with scroll-triggered animations and comprehensive content management.

## 🌐 Live Site
**Production**: https://kroops.me/

## 🛠️ Technical Stack
- **Framework**: Jekyll (GitHub Pages)
- **CMS**: Sveltia CMS for dynamic content management
- **Styling**: Custom CSS with earthy color palette (Sand, Sage, Lavender)
- **Typography**: Local Rinjani Sans + Google Fonts (Funnel Display)
- **Features**: Intersection Observer animations, responsive carousel, touch interactions

## 🚀 Local Development

### Prerequisites
- Ruby (ARM64 Mac setup included)
- Git

### Setup & Run
```bash
# Clone repository
git clone https://github.com/krupabpatel/krupa-portfolio.git
cd krupa-portfolio

# Install Ruby dependencies (ARM64 Mac)
/opt/homebrew/opt/ruby/bin/gem install eventmachine -v '1.2.7' -- --with-cppflags="-I$(brew --prefix)/include -I$(xcrun --show-sdk-path)/usr/include/c++/v1" --with-ldflags="-L$(brew --prefix)/lib"

# Start development server
/opt/homebrew/lib/ruby/gems/3.4.0/bin/jekyll serve --config _config.yml,_config_dev.yml --force_polling
```

**Local URL**: http://127.0.0.1:4000/

## 📁 Project Structure
```
├── _layouts/           # Jekyll templates
├── _projects/          # CMS-managed project content
├── _hero/             # Homepage hero content
├── _sections/         # Section subtitles
├── _education/        # Resume education entries
├── _experience/       # Resume experience entries
├── _skills/           # Skills & certifications
├── assets/            # Images, videos, documents, favicons
├── admin/             # Sveltia CMS configuration
└── index.html         # Homepage
```

## ✨ Key Features
- **Design System**: Earthy color palette with sophisticated animations
- **Mobile-First**: Responsive with hamburger menu and touch interactions
- **Content Management**: Full Sveltia CMS integration for all sections
- **Media Carousel**: Support for images, videos, and Figma embeds
- **Project Links**: Document, GitHub, and hyperlink icon options
- **Resume System**: Timeline layout with dynamic categories
- **Performance**: Optimized assets and scroll-triggered animations
