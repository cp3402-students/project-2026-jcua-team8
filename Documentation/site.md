# Site Management Guide

This document explains how to maintain and update the WordPress website. It is intended for someone who is already familiar with WordPress and needs to continue managing the site.

---

## Content Structure Overview

The website is structured using standard WordPress pages. There is no custom post type system used for this project.

- All main website content is managed through Pages
- Navigation is controlled through the Menus system
- Forms are managed using a dedicated plugin (WPForms)

This keeps the site simple and easy to maintain.

---

## Adding and Editing Content

### Editing Existing Pages

All content pages can be edited via:
WordPress Dashboard → Pages → All Pages

Steps:
1. Select the page you want to edit
2. Click Edit
3. Update content using the WordPress block editor (Gutenberg)
4. Click Update to save changes

Changes will immediately reflect on the live site (or staging, depending on environment).

---

### Creating New Pages

To add a new page:

1. Go to: Pages → Add New
2. Enter page title and content
3. Publish the page
4. Add it to the navigation menu if required

---

## Pages vs Posts

This website primarily uses Pages only.

### Pages
- Used for all main content (Home, Contact, Services, etc.)
- Static content
- Manually added to navigation menus

### Posts
- Not used in this project
- Blog functionality is not part of the current site structure

---

## Navigation and Menus

All navigation links are managed through WordPress menus.

Location: Appearance → Menus

### How it works:
- Each menu item links to a specific page
- Menu is assigned to the Primary Menu location
- Any updates to page structure must be reflected in the menu manually

### Editing menu items:
1. Open Menus section
2. Add/remove pages or custom links
3. Drag and reorder items as needed
4. Save menu

---

## Forms (WPForms Plugin)

All forms on the website are managed using the WPForms plugin.

### How to edit forms:
1. Select the form you want to edit
2. Modify fields using the drag-and-drop builder
3. Save changes

### Embedding forms:
- Forms are embedded into pages using WPForms blocks or shortcodes
- Do not manually edit form HTML inside pages

---

## Content Organisation

The site is structured in a simple hierarchy:

- Main Pages (top-level navigation items)
- Supporting Pages (linked from main pages if needed)
- Forms (handled separately via WPForms)

There is no complex category system or blog taxonomy used.

---

## Important Notes

- Do not edit theme files unless necessary
- Always make content changes through the WordPress dashboard
- Menu updates are required whenever pages are added or renamed
- WPForms should be used for all form-related functionality
- Test major changes in staging before applying to production

---

## Summary

The website is designed to be simple and easy to maintain using standard WordPress features. All content is managed through Pages, navigation is controlled through Menus, and forms are handled using WPForms. This structure ensures that future updates can be made without technical complexity.
