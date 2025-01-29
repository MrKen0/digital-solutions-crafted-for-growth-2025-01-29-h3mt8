# Digital Crafters Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Digital Crafters landing page. Whether you're new to web development or need a quick reference, follow these steps to make common updates safely and effectively.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

```html
<!-- Company Name -->
<div class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">
    Digital Crafters  <!-- Edit this text to change company name -->
</div>
```

### Hero Section
Located at the top of the page, contains main headline and description:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">
    Digital Solutions Crafted for Growth  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-300 leading-relaxed mb-12">
    Empowering SMEs, startups, and non-profits...  <!-- Main description -->
</p>
```

### Tailwind CSS Classes Explained
Common classes used throughout:
- `text-{size}`: Controls text size (xl, 2xl, etc.)
- `md:text-{size}`: Applies style at medium screen sizes
- `bg-gray-900`: Dark background color
- `hover:text-white`: Text color on hover
- `transition-colors`: Smooth color transitions

To modify responsive design:
```html
<!-- Example of responsive classes -->
<div class="text-xl      <!-- Mobile size -->
    md:text-2xl         <!-- Medium screens -->
    lg:text-3xl">      <!-- Large screens -->
    Your text here
</div>
```

## Managing Links

### Navigation Menu Links
Located in the header section:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-300 hover:text-white transition-colors duration-300">Features</a>
    <a href="#benefits" class="text-gray-300 hover:text-white transition-colors duration-300">Benefits</a>
    <!-- Add or modify links here -->
</div>
```

To update a link:
1. Locate the `<a>` tag
2. Modify the `href` attribute
3. Update the link text between the tags

### External Links
The "Get Started" button links:
```html
<a href="https://www.onlinewebpresence.xyz/" class="hidden md:block px-6 py-2 bg-gradient-to-r from-purple-600 to-pink-600 rounded-full">
    Get Started
</a>
```

Replace `https://www.onlinewebpresence.xyz/` with your desired URL.

## Adding Privacy and Terms Pages

### Footer Link Updates
Locate the Legal section in the footer:
```html
<div>
    <h4 class="font-semibold mb-4">Legal</h4>
    <ul class="space-y-2 text-gray-400">
        <li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add new policy pages:
1. Create `privacy.html` and `terms.html` in your project directory
2. Update the href attributes to point to these files
3. Ensure consistent styling by copying the classes from existing links

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
   - Check for typos in `href` attributes
   - Verify file names match exactly
   - Ensure files are in the correct directory

2. **Responsive Design Issues**
   - Check media query classes (md:, lg:)
   - Test on different screen sizes
   - Verify Tailwind CSS is properly loaded

3. **Styling Problems**
   - Confirm class names are spelled correctly
   - Check for missing closing tags
   - Verify class order (Tailwind processes classes left to right)

### Best Practices

1. Always backup before making changes
2. Test changes in a development environment first
3. Validate links after updates
4. Check mobile responsiveness after modifications
5. Keep consistent spacing and indentation

For additional help or complex modifications, consult the [Tailwind CSS documentation](https://tailwindcss.com/docs) or reach out to your development team.