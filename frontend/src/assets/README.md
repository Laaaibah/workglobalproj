# Assets Folder

Place your images and other static assets here.

## Background Images

To use a background image in the Hero component, add it to this folder and reference it by URL path.

### Example usage in index.astro:

```astro
<Hero 
  backgroundImage="url('/src/assets/images/hero-bg.jpg')"
  title="Your Title"
  subtitle="Your subtitle"
  buttonText="Button Text"
  buttonLink="/page"
/>
```

## Supported Image Formats
- JPG/JPEG
- PNG
- WebP
- SVG
- GIF

## How to Add Images

1. Place image files in the `src/assets/images/` folder
2. Reference them using the path: `/src/assets/images/filename.ext`

## Current Components Using Images

- **Hero Component**: Accepts `backgroundImage` prop for custom backgrounds
- **Navbar**: Logo icon (SVG inline, can be replaced)
- **Footer**: Logo text (can add image logo)
