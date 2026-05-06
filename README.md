# Steph Ran | Personal Portfolio

A modern, responsive portfolio website built with **Astro** and **Tailwind CSS v4**, showcasing software engineering projects and UX design work.

## 🚀 Tech Stack

- **Framework:** [Astro](https://astro.build) - Fast, modern static site generator
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com) - Utility-first CSS with CSS-based theming
- **Typography:** Plus Jakarta Sans, Inter (Google Fonts)
- **Icons:** Material Symbols Outlined

## 📁 Project Structure

```
/
├── public/
│   ├── favicon.svg
│   └── favicon.ico
├── src/
│   ├── assets/           # Images and static assets
│   ├── components/       # Reusable Astro components
│   │   ├── Contact.astro
│   │   ├── Design.astro
│   │   ├── DesignCard.astro
│   │   ├── Footer.astro
│   │   ├── Hero.astro
│   │   ├── Landing.astro
│   │   ├── Navbar.astro
│   │   ├── ProjectCard.astro
│   │   ├── Projects.astro
│   │   ├── SkillChip.astro
│   │   └── Skills.astro
│   ├── layouts/
│   │   └── Layout.astro  # Main page layout with Navbar and Footer
│   ├── pages/
│   │   └── index.astro   # Main entry point
│   └── styles/
│       └── global.css    # Tailwind directives and theme configuration
├── astro.config.mjs
└── package.json
```

## 🧩 Components

| Component | Description |
|-----------|-------------|
| `Layout` | Main layout wrapper with Navbar, Footer, and slot for page content |
| `Navbar` | Sticky navigation header with responsive mobile menu |
| `Hero` | Landing section with profile image, introduction, and social links |
| `Projects` | Software engineering projects showcase with project cards |
| `ProjectCard` | Reusable card component for individual project display |
| `Design` | UX design section with design showcase cards |
| `DesignCard` | Reusable card component for design projects |
| `Skills` | Toolkit section displaying technical skills as chips |
| `SkillChip` | Reusable skill badge with icon and label |
| `Contact` | Contact form section with name, email, and message fields |
| `Footer` | Site footer with copyright and navigation links |
| `Landing` | Composite component composing all main sections |

## 🎨 Design System

The project uses a custom Material Design-inspired color palette defined in `src/styles/global.css` using Tailwind v4's `@theme` directive:

- **Primary:** `#486553` (Forest Green)
- **Secondary:** `#496551`
- **Tertiary:** `#5b5f5e`
- **Surface variants** for layered backgrounds
- Custom font sizing for headings (`h1`, `h2`, `h3`, `display`) and body text (`body-md`, `body-lg`, `label-caps`)

## 🧞 Commands

All commands are run from the root of the project:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `pnpm install`            | Installs dependencies                            |
| `pnpm dev`                | Starts local dev server at `localhost:4321`      |
| `pnpm build`              | Build your production site to `./dist/`          |
| `pnpm preview`            | Preview your build locally, before deploying     |
| `pnpm astro ...`          | Run CLI commands like `astro add`, `astro check` |
| `pnpm astro -- --help`    | Get help using the Astro CLI                     |

## 📝 Notes

- The project uses **Tailwind CSS v4** with CSS-based configuration (`@theme` in `global.css`) instead of the traditional `tailwind.config.js`
- All components follow Astro's component model with declarative props passing
- Images are currently hosted externally (Google public links) - consider migrating to local `src/assets/` for production
- The contact form uses a `#` action - wire up to your preferred form handling service (Formspree, Netlify Forms, etc.)

## 👀 Learn More

- [Astro Documentation](https://docs.astro.build)
- [Tailwind CSS v4 Docs](https://tailwindcss.com/docs)
- [Astro Discord](https://astro.build/chat)
