# Component Usage Guide

## 1. Navbar Component

**File**: `src/components/Navbar.astro`

The navbar is automatically included in every page through the Layout component.

**Features**:
- WorkGlobal logo with tagline
- Navigation icons (home, info, pricing, team)
- Sticky positioning
- Responsive design
- Hover effects on icons

**No props needed** - just use it as is, or customize the icons/links inside the component.

---

## 2. Footer Component

**File**: `src/components/Footer.astro`

The footer is automatically included in every page through the Layout component.

**Features**:
- Logo and branding
- Email subscription input with SEND button
- Navigation links (HOME, ABOUT US, PRICING, SUPPORT CENTER)
- Footer links (Terms, Privacy, Security, Cookies)
- Wavy header design
- Copyright notice
- Responsive layout

**No props needed** - customize links and content directly in the component.

---

## 3. Hero Component

**File**: `src/components/Hero.astro`

Displays a full-screen hero section with customizable content.

**Props**:
```typescript
interface Props {
  backgroundImage?: string;      // CSS background-image value
  title?: string;                // Main heading
  subtitle?: string;             // Subheading/description
  buttonText?: string;           // CTA button text
  buttonLink?: string;           // CTA button link
}
```

**Usage Example**:
```astro
<Hero 
  backgroundImage="url('/src/assets/images/hero-bg.jpg')"
  title="Welcome to WorkGlobal"
  subtitle="Swipe. Match. Work"
  buttonText="Get Started"
  buttonLink="/jobs"
/>
```

**Default Values** (if not provided):
- Background: Purple gradient
- Title: "Welcome to WorkGlobal"
- Subtitle: "Swipe. Match. Work - Find your perfect job match today"
- Button: "Get Started"

---

## 4. Layout Component

**File**: `src/layouts/Layout.astro`

Main layout wrapper for all pages. Automatically includes:
- Navbar at the top
- AOS (Animate On Scroll) library
- Global styles
- Footer at the bottom

**Usage in pages**:
```astro
---
import Layout from '../layouts/Layout.astro';
---

<Layout title="Page Title">
  <!-- Your page content here -->
</Layout>
```

---

## Adding Background Images

1. Place your hero background image in `src/assets/images/`
2. Reference it in the Hero component:

```astro
<Hero 
  backgroundImage="url('/src/assets/images/your-image.jpg')"
  title="Your Title"
  subtitle="Your subtitle"
/>
```

---

## Customization Tips

- **Colors**: Edit the gradient colors in each component's `<style>` section
- **Spacing**: Modify padding/margin values in styles
- **Fonts**: Change font-size and font-weight values
- **Icons**: Update SVG icons in Navbar component
- **Links**: Modify href attributes in Footer navigation

---

## Animations

All components include:
- **Fade-in animations** on load
- **Hover effects** on interactive elements
- **AOS animations** with `data-aos` attributes
- **Smooth transitions** on buttons and links

Use `data-aos="fade-up"`, `data-aos="fade-in"`, etc. on elements to add scroll animations.
