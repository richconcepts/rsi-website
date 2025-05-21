# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Website Architecture

This is a static website for Referentia Systems Incorporated (RSI), a cybersecurity company. The website follows a traditional HTML/CSS/JS structure without a modern framework.

### Key Components

- **HTML Structure**: Individual HTML files for each page (index.html, about-us/index.html, etc.)
- **CSS Styling**: Uses Bootstrap 5 with custom styling in style.css
- **JavaScript**: Minimal JavaScript with libraries for animations and parallax effects
- **Images**: Includes both JPG/PNG and WebP formats with proper fallbacks for browser compatibility

### Optimization Features

- **Image Optimization**: Images use WebP with fallbacks to JPG/PNG
- **Lazy Loading**: Uses the lazysizes.js library for optimized image loading
- **Responsive Design**: Bootstrap-based responsive layout with custom breakpoints

## Directory Structure

- `/`: Main site files including index.html and style.css
- `/about-us/`: About page
- `/business-units/`: Business units page
- `/careers/`: Careers page
- `/contact/`: Contact page
- `/css/`: External CSS libraries
- `/js/`: JavaScript files
- `/img/`: Image assets in both WebP and traditional formats

## Common Development Tasks

### Local Testing

Since this is a static HTML site, you can test it locally by opening the HTML files directly in a browser. For more advanced testing with live reload, you could use a simple HTTP server:

```bash
# Using Python's built-in HTTP server
python -m http.server

# Or with Node.js and live-server (if installed)
npx live-server
```

### Editing Pages

1. Each page lives in its own directory with an index.html file
2. Shared components (navigation, footer) should be kept consistent across pages
3. When adding new pages, follow the existing directory structure pattern

### Image Optimization

When adding new images to the site:

1. Create both WebP and traditional (JPG/PNG) versions
2. Use the same naming pattern for both versions
3. Implement using the `<picture>` element with WebP source and fallback as seen in existing code

### SEO Considerations

Each page includes:
- Unique meta title and description specific to the page content
- Proper canonical URL
- Semantic HTML5 structure
- Follow existing patterns when adding meta information to new pages

## Accessibility Guidelines

The site implements several accessibility features that should be maintained:

1. ARIA labels on all interactive elements
2. Proper image alt text
3. Semantic HTML structure
4. Keyboard navigation support
5. Sufficient color contrast
6. Screen reader compatibility

Always preserve and extend these accessibility features when making changes.