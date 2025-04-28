# Bryan Engel Photography Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Bryan Engel Photography landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<div class="flex-shrink-0">
    <h1 class="text-2xl font-bold">Bryan Engel</h1> <!-- Update business name here -->
</div>
```

#### Hero Section
```html
<h2 class="text-4xl md:text-6xl font-bold leading-tight mb-4">Bryan Engel Photography</h2>
<p class="text-xl md:text-2xl mb-8">Taking your photography to the next level</p>
```

#### Announcement Bar
```html
<div class="bg-gray-900 text-white py-2 text-center text-sm">
    <p>Fast Worldwide Shipping (5 days delivery) | 100% Satisfaction Guarantee</p>
</div>
```

### Tailwind CSS Class Modifications

#### Understanding Responsive Classes
- `md:` prefix = applies styles on medium screens and larger
- `lg:` prefix = applies styles on large screens and larger
- Example: `text-4xl md:text-6xl` means text is 4xl on mobile, 6xl on medium screens

#### Common Class Categories
1. Spacing Classes
   - `p-` (padding): `p-4`, `py-2`, `px-4`
   - `m-` (margin): `m-4`, `my-2`, `mx-4`

2. Text Classes
   - Size: `text-sm`, `text-lg`, `text-2xl`
   - Color: `text-white`, `text-gray-600`
   - Weight: `font-bold`, `font-semibold`

3. Layout Classes
   - Flex: `flex`, `flex-col`, `items-center`
   - Grid: `grid`, `grid-cols-1`, `md:grid-cols-3`

### Troubleshooting Tips
- Always maintain both mobile and desktop classes
- Test responsive design using browser dev tools
- Keep consistent spacing throughout sections

## 2. Fixing Broken Links

### Navigation Menu Links
Current internal links in the navigation:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#pricing">Pricing</a>
<a href="#testimonials">Testimonials</a>
```

To update:
1. Identify the section ID you want to link to
2. Add or modify the `href` attribute with `#section-id`
3. Ensure the target section has matching `id` attribute

### External Links
For email links:
```html
<a href="mailto:bryanengel@icloud.com">Contact Now</a>
```

To update:
1. Replace `bryanengel@icloud.com` with new email
2. Maintain the `mailto:` prefix

### Social Media Links (Adding New)
```html
<!-- Add to footer section -->
<div class="space-x-4">
    <a href="https://instagram.com/yourhandle" class="text-gray-400 hover:text-white">
        Instagram
    </a>
    <a href="https://facebook.com/yourpage" class="text-gray-400 hover:text-white">
        Facebook
    </a>
</div>
```

## 3. Linking Privacy and Terms Pages

### Footer Link Updates
Current placeholder links:
```html
<div>
    <h4 class="font-bold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To update:
1. Create privacy.html and terms.html files
2. Update href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

### Creating Policy Pages
Basic structure for privacy.html/terms.html:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Privacy Policy - Bryan Engel Photography</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
</head>
<body class="font-sans antialiased">
    <!-- Copy header from index.html -->
    
    <main class="container mx-auto px-4 py-12">
        <h1 class="text-3xl font-bold mb-8">Privacy Policy</h1>
        <!-- Add policy content here -->
    </main>

    <!-- Copy footer from index.html -->
</body>
</html>
```

### Troubleshooting Tips
- Verify all file names match exactly (case-sensitive)
- Test all links after updating
- Maintain consistent styling across pages
- Ensure navigation back to home page works

Remember to:
- Keep backups before making changes
- Test on multiple devices and browsers
- Update any references to old links
- Maintain consistent branding across all pages

Need more help? Contact your web developer or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).