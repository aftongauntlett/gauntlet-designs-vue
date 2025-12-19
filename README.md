# Gauntlet Designs

[![Status](https://img.shields.io/badge/Status-Live-brightgreen)](https://gauntletdesigns.com)
[![License](https://img.shields.io/badge/License-MIT-blue)](https://opensource.org/licenses/MIT)

A clean farewell page for a closed business. Built to be fast, accessible, and easy to maintain.

This project includes:

- a custom theme system with light/dark mode
- reusable Vue 3 components with composition API
- accessible UI with semantic HTML and ARIA labels
- SEO optimization with sitemap and robots.txt
- custom deployment workflow syncing dev to production repos

**Live Site**: [gauntletdesigns.com](https://gauntletdesigns.com)

## What It Does

This site acts as a professional goodbye page. It thanks past clients, links to my current work, and keeps the business closure clear and respectful. I wanted something simple that loads fast and looks good on any device.

## Tech Stack

**Frontend**: Vue 3, Vite, Tailwind CSS, CSS Custom Properties  
**Deployment**: Vercel with custom deployment scripts  
**Icons**: Heroicons

## Quick Start

```bash
git clone https://github.com/aftongauntlett/gauntlet-designs-vue.git
cd gauntlet-designs-vue
npm install

npm run dev
```

The site runs on `http://localhost:5173`.

## Deployment

This repo syncs to a production repository that Vercel watches.

```bash
# Deploy to production
npm run deploy
```

The deploy script checks that you're on the main branch and that all changes are committed before pushing to the production repo.

## License

MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

Built by [Afton Gauntlett](https://www.aftongauntlett.com/)
