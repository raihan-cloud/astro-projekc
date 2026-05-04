# Raihan Muzhaffar — Portfolio Website

A modern, responsive personal portfolio built with **Astro** + **Tailwind CSS**.

---

## 🚀 Quick Start

### Prerequisites
- Node.js **18+** installed ([download here](https://nodejs.org))
- npm (comes with Node.js)

### Installation & Running

```bash
# 1. Navigate into the project folder
cd raihan-portfolio

# 2. Install dependencies
npm install

# 3. Start the development server
npm run dev
```

Open your browser at **http://localhost:4321** and you'll see the portfolio live.

---

## 📦 Build for Production

```bash
# Build static files
npm run build

# Preview the production build locally
npm run preview
```

The output goes to the `dist/` folder — ready to deploy anywhere.

---

## 🌐 Deployment Options

### Netlify (drag-and-drop)
1. Run `npm run build`
2. Drag the `dist/` folder to [netlify.com/drop](https://app.netlify.com/drop)

### Vercel
```bash
npx vercel
```

### GitHub Pages
Add to `astro.config.mjs`:
```js
export default defineConfig({
  site: 'https://yourusername.github.io',
  base: '/your-repo-name',
  integrations: [tailwind()],
});
```

---

## 📁 Project Structure

```
rizwan-portfolio/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Navbar.astro
│   │   ├── Hero.astro
│   │   ├── About.astro
│   │   ├── Services.astro
│   │   ├── Projects.astro
│   │   ├── Testimonials.astro
│   │   ├── Contact.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── BaseLayout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── tailwind.config.mjs
└── package.json
```

---

## ✏️ Customization

| What to change | Where |
|---|---|
| Your name & title | `src/components/Hero.astro` |
| About me text | `src/components/About.astro` |
| Services offered | `src/components/Services.astro` |
| Project cards | `src/components/Projects.astro` |
| Testimonials | `src/components/Testimonials.astro` |
| Contact info | `src/components/Contact.astro` |
| Colors | `tailwind.config.mjs` → `primary` |
| Fonts | `src/styles/global.css` |

### Adding a real profile photo
Replace the placeholder in `Hero.astro` and `About.astro`:
```astro
<!-- Remove the placeholder div, add: -->
<img src="/images/profile.jpg" alt="Rizwan Ali" class="w-full h-full object-cover" />
```
Then place your photo at `public/images/profile.jpg`.

---

## 🛠 Tech Stack

- [Astro 4](https://astro.build) — Zero-JS-by-default framework
- [Tailwind CSS 3](https://tailwindcss.com) — Utility-first CSS
- [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans) — Display font
- [DM Sans](https://fonts.google.com/specimen/DM+Sans) — Body font
