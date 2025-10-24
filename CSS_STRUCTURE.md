# CSS File Structure - SkillShare™ Website

## Overview
The CSS has been separated into multiple files for better organization, maintainability, and performance. Each HTML page now has its own specific CSS file while sharing common styles through a base file.

## File Structure

```
css/
├── base.css              # Common styles shared across all pages
├── index.css             # Homepage-specific styles
├── about.css             # About page-specific styles
├── features.css          # Features page-specific styles
├── how-it-works.css      # How It Works page-specific styles
├── contact.css           # Contact page-specific styles
└── style.css             # Original combined file (kept for reference)
```

## File Descriptions

### `base.css`
**Purpose**: Contains all common styles shared across all pages
**Includes**:
- CSS Reset & Base Styles
- Color Palette (CSS Variables)
- Typography
- Layout Utilities
- Navigation Styles
- Button Styles
- CTA Section Styles
- Footer Styles
- Animations
- Responsive Design
- Accessibility Styles

### `index.css`
**Purpose**: Homepage-specific styles
**Includes**:
- Hero Section
- Features Preview
- Phone Mockup
- App Preview Components

### `about.css`
**Purpose**: About page-specific styles
**Includes**:
- Page Header
- Story Section
- Community Illustration
- Mission & Vision Cards
- Values Grid
- Team CTA

### `features.css`
**Purpose**: Features page-specific styles
**Includes**:
- Page Header
- Main Features Showcase
- Feature Mockups (Profile, Listing, Payment, Reviews)
- Additional Features Grid

### `how-it-works.css`
**Purpose**: How It Works page-specific styles
**Includes**:
- Page Header
- Steps Overview Timeline
- Detailed Steps
- Step Mockups
- Success Stories

### `contact.css`
**Purpose**: Contact page-specific styles
**Includes**:
- Page Header
- Contact Section
- Contact Methods
- Social Links
- Contact Form
- FAQ Section

## HTML File Updates

Each HTML file now includes:
```html
<link rel="stylesheet" href="css/base.css">
<link rel="stylesheet" href="css/[page-name].css">
```

## Benefits of This Structure

1. **Better Organization**: Each page's styles are clearly separated
2. **Improved Maintainability**: Easier to find and modify specific page styles
3. **Better Performance**: Browsers can cache base.css across all pages
4. **Reduced File Size**: Each page only loads the CSS it needs
5. **Easier Debugging**: Page-specific issues are isolated to their respective CSS files
6. **Team Collaboration**: Multiple developers can work on different pages without conflicts
7. **Modularity**: Easy to add new pages with their own CSS files

## Usage Guidelines

- **Always include base.css first** in HTML files
- **Add page-specific CSS after base.css** to allow overrides
- **Keep common styles in base.css** to maintain consistency
- **Use page-specific CSS only for unique elements** not shared across pages
- **Test all pages** after making changes to base.css

## Migration Notes

- The original `style.css` file is kept for reference
- All functionality remains exactly the same
- No visual changes were made during the separation
- All responsive design and animations are preserved
