# Lympany Art - Hugo Serif Theme Site

This is a Hugo site using the Serif theme for displaying art portfolio.

## Features

- **Serif Theme**: Beautiful, clean design perfect for showcasing art
- **Image Zoom**: Click images to open in a lightbox with full zoom capabilities
- **Pinch to Zoom**: On touch devices, pinch images directly on the page to zoom
- **Responsive**: Works beautifully on desktop, tablet, and mobile devices

## Setup

1. Make sure you have Hugo Extended installed (required for SCSS compilation)
2. Clone this repository
3. The serif theme is already included in `themes/hugo-serif-theme`

## Adding Your Artwork

### Method 1: Using the Image Shortcode (Recommended)

Add images with captions using the `image` shortcode:

```markdown
{{< image src="/images/your-artwork.jpg" alt="Artwork Title" >}}
Description of your artwork goes here.
{{< /image >}}
```

### Method 2: Standard Markdown

You can also use standard Markdown image syntax:

```markdown
![Artwork Title](/images/your-artwork.jpg)

Description of your artwork goes here.
```

### Organizing Images

1. Place your JPEG images in the `static/images/` directory
2. Create content files in:
   - `content/portraits/` for portrait paintings
   - `content/still-lifes/` for still life paintings
   - `content/about.md` for your about page

### Example Content File

Create a file like `content/portraits/my-portrait.md`:

```markdown
---
title: "My Portrait"
date: 2025-01-02
draft: false
---

{{< image src="/images/my-portrait.jpg" alt="My Portrait" >}}
This is a beautiful portrait painting created in 2024.
{{< /image >}}
```

## Running Locally

```bash
hugo server
```

Then visit `http://localhost:1313` in your browser.

## Building for Production

```bash
hugo
```

This will generate the site in the `public/` directory.

## Deployment to Netlify

1. Push your code to a Git repository (GitHub, GitLab, etc.)
2. Connect the repository to Netlify
3. Set build command: `hugo`
4. Set publish directory: `public`
5. Make sure to use Hugo Extended version in Netlify build settings

## Menu Structure

The top menu includes:
- **Home**: Main landing page
- **About**: About page
- **Portraits**: Gallery of portrait paintings
- **Still Lifes**: Gallery of still life paintings

Menu items are configured in `hugo.toml`.

## Image Zoom Features

- **Click/Tap**: Click any image to open it in a full-screen lightbox
- **Pinch to Zoom**: On touch devices, pinch images directly on the page to zoom in/out
- **Double Tap**: Double tap to reset zoom level
- **Lightbox Navigation**: When viewing in lightbox, swipe or use arrow keys to navigate between images

## Customization

- Edit `hugo.toml` to change site settings, colors, and fonts
- Custom styles are in `assets/scss/custom.scss`
- Layouts can be customized in the `layouts/` directory
