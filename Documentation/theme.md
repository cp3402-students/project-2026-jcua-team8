# Theme Documentation

This document explains the structure, features, and design decisions of the custom WordPress theme used in this project. It is intended to help another developer quickly understand how the theme works and continue development.

---

## Theme Overview

The website is built using the Picostrap 5 starter theme, which is a lightweight theme based on Bootstrap 5.

Picostrap is designed as a minimal starting point rather than a finished theme. It provides basic layout structure and Bootstrap integration, allowing full control over styling and layout through customisation.

Most of the visual design and layout adjustments in this project are implemented using:
- WordPress Customizer settings
- Custom CSS

---

## Theme Features

Key features of the theme include:

- Bootstrap 5 integration for responsive layout and grid system
- Customisable navigation bar using WordPress menus
- Support for WordPress block editor (Gutenberg)
- Basic header and footer structure provided by Picostrap
- Ability to override styles using Additional CSS

The theme is intentionally kept simple to allow flexibility in design.

---

## Main Edited Files in Picostrap 5 Theme

When working with the Picostrap 5 starter theme, most custom development is kept minimal to maintain upgradability and avoid breaking core functionality. However, some key files and areas are commonly edited or extended during development.

---

### 1. `style.css`
- Base stylesheet for the theme
- Used for minor overrides, but most styling is handled via WordPress Customizer (Additional CSS)
- Contains theme metadata and sometimes global style adjustments

---

### 2. `functions.php`
- Used to enable or modify WordPress features
- Common edits include:
  - Enqueuing custom styles or scripts
  - Adding theme support options
  - Registering menus or widgets

---

### 3. `header.php`
- Controls the top section of the site
- Contains:
  - Navigation bar structure
  - Logo placement
  - Header layout using Bootstrap classes

---

### 4. `footer.php`
- Controls footer layout and content
- Used for:
  - Contact information
  - Opening hours
  - Footer layout structure using Bootstrap grid system

---

### 5. WordPress Customizer (Not a file but important)
Most styling changes are applied here instead of editing theme files:

- Appearance → Customize → Additional CSS
- Used for:
  - Layout adjustments
  - Typography changes
  - Spacing fixes
  - Component styling (buttons, navbar, etc.)

---

### 6. Template Files (Minimal or Optional Edits)
Depending on project needs, these may also be referenced or lightly modified:

- `page.php` – controls page layout
- `single.php` – controls blog post layout (if used)
- `index.php` – fallback template

In this project, most layout changes are handled through CSS rather than modifying these templates directly.

---

## Summary

The Picostrap 5 theme is designed to minimise direct file editing. Most development work is done through:

- `header.php` and `footer.php` for structure
- `functions.php` for functionality
- `style.css` and Customizer for styling

This approach keeps the theme lightweight, flexible, and easier to maintain.
