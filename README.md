# Astro Static Website Template

A minimal, modern starter template for building static websites with Astro. This template includes everything you need to get started with a landing page, icons, and content management capabilities.

## Features

- **🚀 Astro** - Lightning-fast static site generation
- **🎨 Tailwind CSS v4** - Utility-first CSS framework for rapid styling
- **🎯 Astro Icons** - Beautiful icon component library with Tabler icon set
- **📝 MDX** - Write JSX in your Markdown documents
- **💅 Sass** - CSS preprocessor with variables, mixins, and nesting
- **📖 Tailwind Typography** - Beautiful typography styles for markdown content

## Tech Stack

### Core Framework

- **Astro** `^5.16.6` - The web framework for content-driven websites

### Integrations

- **@astrojs/react** `^4.4.2` - React integration for Astro
- **@astrojs/mdx** `^4.3.13` - MDX support for writing JSX in Markdown
- **astro-icon** `^1.1.5` - Icon component library

### Styling

- **tailwindcss** `^4.1.18` - Utility-first CSS framework
- **@tailwindcss/vite** `^4.1.18` - Tailwind CSS Vite plugin
- **@tailwindcss/typography** `^0.5.19` - Typography plugin for beautiful markdown styling
- **sass** `^1.97.2` - CSS preprocessor

### Icons

- **@iconify-json/tabler** `^1.2.26` - Tabler icon set for astro-icon

## 📁 Project Structure

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── assets/          # Static assets (images, SVGs)
│   ├── components/      # Reusable Astro components
│   │   ├── CTA.astro           # Call-to-action section
│   │   ├── Features.astro      # Features showcase
│   │   ├── Footer.astro        # Site footer
│   │   ├── Header.astro        # Site header/navigation
│   │   ├── Hero.astro          # Hero section
│   │   ├── ScrollReveal.tsx    # Scroll animation component
│   │   └── SassExample.astro   # Sass usage example
│   ├── layouts/
│   │   └── Layout.astro        # Base page layout
│   ├── pages/          # Routes (file-based routing)
│   │   ├── index.astro         # Homepage
│   │   ├── about.astro         # About page
│   │   ├── contact.astro      # Contact page
│   │   ├── features.astro      # Features page
│   │   └── example.mdx         # MDX example page
│   └── styles/
│       ├── global.css          # Global styles & Tailwind imports
│       └── example.scss        # Sass example file
├── astro.config.mjs    # Astro configuration
├── tailwind.config.mjs # Tailwind configuration
└── package.json
```

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- npm, pnpm, or yarn

### Installation

1. **Clone the repository**

   ```bash
   https://github.com/teknikoyazilimcozumleri/astro-website-template.git
   cd astro-website-template
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the development server**

   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:4321`

## Available Scripts

| Command           | Action                                           |
| :---------------- | :----------------------------------------------- |
| `npm install`     | Installs dependencies                            |
| `npm run dev`     | Starts local dev server at `localhost:4321`      |
| `npm run build`   | Build your production site to `./dist/`          |
| `npm run preview` | Preview your build locally                       |
| `npm run astro`   | Run CLI commands like `astro add`, `astro check` |

## Styling

### Tailwind CSS

This project uses Tailwind CSS v4 for styling. All components use Tailwind utility classes.

**Global Styles:**

- Located in `src/styles/global.css`
- Imports Tailwind CSS
- Includes Tailwind Typography plugin for markdown styling

**Configuration:**

- `tailwind.config.mjs` - Tailwind configuration with Typography plugin

### Sass

Sass is installed and ready to use. You can use Sass in component `<style>` blocks:

```astro
<style lang="scss">
  $primary-color: #000;

  .my-component {
    color: $primary-color;
  }
</style>
```

See `src/components/SassExample.astro` for a complete example.

## Components

### Icons

Use Tabler icons with astro-icon:

```astro
---
import { Icon } from "astro-icon/components";
---

<Icon name="tabler:heart" class="w-6 h-6" />
```

Browse available icons at [Tabler Icons](https://tabler.io/icons).

## 📝 MDX Support

Write JSX in your Markdown documents. Create `.mdx` files in the `src/pages` directory:

```mdx
---
import Layout from "../layouts/Layout.astro";
---

<Layout>
  # My MDX Page This is **markdown** with <Component /> support!
</Layout>
```

See `src/pages/example.mdx` for a complete example.

## Pages

- **/** - Homepage with hero, features, and CTA sections
- **/features** - Features showcase page
- **/about** - About page
- **/contact** - Contact form page
- **/example** - MDX example page demonstrating markdown features

## Configuration

### Astro Config (`astro.config.mjs`)

```javascript
export default defineConfig({
  output: "static",
  vite: {
    plugins: [tailwindcss()],
  },
});
```

### Tailwind Config (`tailwind.config.mjs`)

```javascript
import typography from "@tailwindcss/typography";

export default {
  plugins: [typography],
};
```

## Key Dependencies

### Core

- **Astro** - Web framework
- **React** - UI library for interactive components
- **Tailwind CSS** - Utility-first CSS framework

### Integrations

- **@astrojs/react** - React integration
- **@astrojs/mdx** - MDX support
- **astro-icon** - Icon component library

### Styling

- **@tailwindcss/typography** - Typography plugin
- **sass** - CSS preprocessor

### Icons

- **@iconify-json/tabler** - Tabler icon set

## Design Features

- **Black & White Color Scheme** - Minimal, clean design
- **Responsive Layout** - Mobile-first approach
- **Smooth Animations** - Scroll reveal effects with spring physics
- **Modern Typography** - Beautiful text styling with Tailwind Typography
- **Component-Based** - Reusable, modular components

## Learn

- [Astro Documentation](https://docs.astro.build)
- [Tailwind CSS Documentation](https://tailwindcss.com)
- [Astro Icons Documentation](https://www.astroicon.dev)
- [MDX Documentation](https://mdxjs.com)
---
