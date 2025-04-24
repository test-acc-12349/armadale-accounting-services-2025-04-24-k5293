# Armadale Landing Page Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Armadale Accounting Services landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To modify:

1. **Company Name**
```html
<!-- Located in header section -->
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">
    Armadale  <!-- Change this text -->
</a>
```

2. **Navigation Menu Items**
```html
<div class="hidden md:flex space-x-8">
    <a href="#services">Services</a>  <!-- Change text here -->
    <a href="#benefits">Benefits</a>  <!-- And here -->
    <a href="#contact">Contact</a>    <!-- And here -->
</div>
```

### Hero Section
The main banner section contains:
```html
<h1 class="text-4xl md:text-6xl lg:text-7xl font-bold leading-tight mb-8">
    Building financial clarity in a complex world  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">
    Expert accounting services tailored to your business needs  <!-- Subheading -->
</p>
```

### Tailwind CSS Tips
- `text-4xl` to `text-7xl`: Controls text size
- `md:` prefix: Applies styles on medium screens and up
- `mb-8`: Adds margin bottom (spacing)
- `text-gray-300`: Sets text color
- `hover:scale-105`: Enlarges element on hover

## Managing Links

### Navigation Links
Current placeholder links that need updating:

1. **Main Navigation**
```html
<a href="#services">Services</a>
<a href="#benefits">Benefits</a>
<a href="#contact">Contact</a>
```
To update:
- Replace `#services` with the actual URL (e.g., `/services.html`)
- Keep the `#` prefix for same-page section links

2. **Call-to-Action Buttons**
```html
<a href="https://theaccountants.com" class="...">
    Get Started
</a>
```
To update:
- Replace `https://theaccountants.com` with your actual booking or contact page URL
- Ensure the URL includes `https://` for external links

### Footer Links
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white">Business Valuation</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white">Audit Preparation</a></li>
    <!-- Add more links as needed -->
</ul>
```
Replace `#` with actual page URLs (e.g., `/services/business-valuation.html`)

## Adding Privacy and Terms Pages

### Step 1: Create New Pages
Create two new files in your project:
- `privacy.html`
- `terms.html`

### Step 2: Update Footer Links
Locate this section in the footer:
```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white">Terms of Service</a></li>
    </ul>
</div>
```

Replace the placeholder links:
```html
<li><a href="/privacy.html" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
<li><a href="/terms.html" class="text-gray-400 hover:text-white">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Links**
- Check for typos in URLs
- Ensure file names match exactly
- Verify file locations in your project folder

2. **Styling Problems**
- Make sure Tailwind CSS is properly loaded
- Check for missing class names
- Verify responsive classes (md:, lg:) are correct

3. **Layout Issues**
- Check container classes
- Verify grid column settings
- Ensure proper nesting of elements

### Need Help?
- Double-check your HTML syntax
- Validate your HTML at [W3C Validator](https://validator.w3.org/)
- Inspect elements using browser developer tools (F12)

Remember to always test your changes across different screen sizes and browsers before publishing updates.