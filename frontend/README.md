# Frontend - Astro Project

A modern web frontend built with Astro, React, and Tailwind CSS with animation support.

## Features

- ⚡ **Astro** - Fast static site generation
- ✨ **Animations** - Framer Motion and AOS (Animate On Scroll)
- 🎨 **Tailwind CSS** - Utility-first CSS framework
- ⚛️ **React** - Interactive components
- 📱 **Responsive Design** - Mobile-first approach

## Project Structure

```
frontend/
├── src/
│   ├── components/     # Reusable Astro and React components
│   ├── layouts/        # Layout templates
│   ├── pages/          # Page components (routes)
│   └── styles/         # Global CSS and Tailwind config
├── public/             # Static assets
├── astro.config.mjs    # Astro configuration
├── tailwind.config.mjs # Tailwind configuration
└── package.json        # Dependencies
```

## Getting Started

### Install Dependencies

```bash
npm install
```

### Development Server

```bash
npm run dev
```

Visit `http://localhost:3000` to see your site.

### Build for Production

```bash
npm run build
npm run preview
```

## Animation Libraries

- **Framer Motion** - Powerful React animation library
- **AOS** - Animate elements on scroll
- **Tailwind CSS Animations** - Built-in utility animations

## Customization

- Edit components in `src/components/`
- Add new pages in `src/pages/`
- Modify styles in `src/styles/global.css`
- Configure animations in `tailwind.config.mjs`

## Learn More

- [Astro Documentation](https://docs.astro.build)
- [Tailwind CSS](https://tailwindcss.com)
- [Framer Motion](https://www.framer.com/motion)
- [AOS Library](https://michalsnik.github.io/aos)
