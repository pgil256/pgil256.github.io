# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static HTML5 portfolio website built on the HTML5 UP Miniport template. Single-page design with sections for intro, skills, portfolio projects, and contact form.

## Portfolio Projects (Sibling Repositories)

These projects are located alongside portfolio_new in the parent `projects/` directory. When adding or updating portfolio entries, reference these for accurate descriptions.

### Web Applications

**Juntas Seguras** (`../juntas-seguras/`)
- Rotating savings pool (tanda/ROSCA) management platform
- Tech: Next.js 14, TypeScript, MongoDB, NextAuth.js, Tailwind CSS, shadcn/ui
- Features: MFA authentication, pool management, payment tracking (Venmo/PayPal/Zelle/Cash App), member messaging, analytics dashboard
- 59 API endpoints, 12 MongoDB models, 21 custom React hooks

**Home Finder** (`../home_finder/`)
- Property data aggregation for Pinellas County, FL real estate
- Tech: Django 5, Python, Selenium, Celery/Redis, PostgreSQL, Tailwind CSS
- Features: Scrapes PCPAO (property appraiser) and tax collector data, search/filter dashboard, Excel/PDF export, market visualizations
- Handles 400k+ parcels with async Celery pipeline

**Map-My-Seat** (`../map-my-seat/`)
- Automated seating chart generator for K-12 teachers
- Tech: React 18, Express, PostgreSQL, Knex.js, Chakra UI, JWT auth
- Features: Classroom layout editor, student management, constraint-based seat assignment
- Monorepo with separate frontend/backend

### Desktop Applications

**DesktopPetPy** (`../DesktopPetPy/`)
- Windows desktop pet ("Lou") with energy-driven AI behavior
- Tech: Python, Pygame, Win32 API (layered window transparency)
- Features: State machine with 4 energy tiers, treat system with physics, animated sprite system
- Builds to single .exe via PyInstaller

**TabVision** (`../tab_vision/`)
- Automatic guitar tab transcription from video
- Tech: Electron + React (frontend), Flask + Basic Pitch + MediaPipe (backend)
- Features: Audio pitch detection + visual finger tracking fusion, confidence scoring, interactive tab editor, PDF export

### Games

**Weasel Entertainment System** (`../rpi-game/`)
- Arcade game launcher with 6 classic remakes (Snake, Pac-Man, Frogger, Centipede, Dig Dug, Boulder Dash)
- Tech: Python, Pygame, designed for Raspberry Pi with NES gamepad support
- Features: Weasel/ferret theming, animated ferret sprite system, unified input manager, modular game engine

**Horror Game** (`../horror_game/`)
- First-person horror game (10-20 min experience)
- Tech: Godot 4.x, GDScript
- Features: Room shuffle mechanic, ghost AI with patrol/hunt/kill states, 5 collectible teeth, permadeath
- Currently in design phase (design doc complete)

## Development Commands

```bash
# Compile SASS to CSS
sass assets/sass/main.scss assets/css/main.css

# Watch for SASS changes during development
sass --watch assets/sass:assets/css

# Local development server (either option)
python3 -m http.server 8000
npx http-server
```

No package manager, build step, or test framework is configured. Open `index.html` directly in a browser for quick preview.

## Architecture

### Tech Stack
- HTML5 with semantic sections (`<article>`, `<section>`)
- SASS/SCSS for styling (compiles to `assets/css/main.css`)
- jQuery for interactivity (scroll effects, panels, mobile handling)
- Font Awesome 5 for icons
- Formspree.io for contact form submission

### Key Files
- `index.html` - Single page containing all content
- `assets/sass/main.scss` - Main SASS source, imports libs from `assets/sass/libs/`
- `assets/js/main.js` - Portfolio initialization (scrolly effects, breakpoints)
- `assets/js/util.js` - jQuery plugins for panels, navList, placeholder polyfills

### SASS Structure
The SASS libs in `assets/sass/libs/` provide:
- `_vars.scss` - Color, size, and font definitions
- `_breakpoints.scss` - Responsive breakpoint mixins
- `_mixins.scss` - Utility mixins (icon, padding, vendor prefixes)
- `_html-grid.scss` - Responsive grid system

## Conventions

### Responsive Breakpoints
Use the mixin syntax in SASS:
```scss
@include breakpoint('<=large') { ... }   // 981px-1280px
@include breakpoint('<=medium') { ... }  // 737px-980px
@include breakpoint('<=small') { ... }   // up to 736px
```

### Grid Classes
Responsive column classes with breakpoint suffixes:
```html
<div class="col-4 col-6-medium col-12-small">
```

### Color Palette
- Primary blue: `#43B3E0` (hover: `#43bff0`)
- Body text: `#888`
- Headers: `#3e3e3e`
- Dark backgrounds: `#282828` (nav), `#303030` (footer)

## External Integrations

- **Contact Form**: Formspree endpoint ID `mnqkvpjk`
- **Fonts**: Open Sans via Google Fonts (weights 300, 600, 700)
- **Icons**: Font Awesome 5 (brands, regular, solid)
