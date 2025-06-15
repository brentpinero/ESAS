# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the website for ESAS (Energy Savings Assessment Services) / Eco Stream Air Solutions, an HVAC services company. The website is built using Microsoft Power Apps Portals (now Power Pages) framework with custom HTML, CSS, and JavaScript components.

## Architecture

- **Platform**: Microsoft Power Apps Portals/Power Pages
- **Structure**: Component-based with reusable HTML templates and custom styling
- **Templating**: Uses Liquid templating syntax for dynamic content and localization
- **Styling**: CSS custom properties with a defined color palette theme system

## Key Files and Components

- `ESAS/web-pages/Home/index.html` - Main homepage content
- `ESAS/Header.html` - Site header with navigation and branding (uses Liquid templating)
- `ESAS/Footer.html` - Site footer component
- `ESAS/theme.css` - Custom theme styles extending Bootstrap
- `ESAS/portalbasictheme.css` - Portal-generated theme with CSS custom properties
- `ESAS/bootstrap.min.css` - Bootstrap 3.3.6 framework

## Styling System

The site uses a CSS custom property system with predefined theme colors:
- Primary green: `--portalThemeColor1: #219653`
- Accent yellow: `--portalThemeColor2: #FFCA4B`
- Background colors: `--portalThemeColor7` (white), `--portalThemeColor12` (light gray)

HTML components use inline styles combined with CSS classes and data attributes for theming (`data-component-theme`).

## Component Structure

- Components are self-contained HTML blocks with inline styles
- Responsive design using flexbox and Bootstrap grid classes
- Image assets stored in root ESAS directory
- Custom JavaScript files are currently empty but structure exists for future enhancements

## External Dependencies

- Bootstrap 3.3.6
- Inter font family (loaded via CDN)
- Cal.com integration for appointment booking
- Power Apps Portals runtime and templating engine

## Development Notes

- HTML components use extensive inline styling for portal compatibility
- Liquid templating syntax is used for dynamic content (`{% %}` blocks)
- Portal theme system automatically generates CSS custom properties
- Mobile responsiveness handled through flexbox and Bootstrap classes