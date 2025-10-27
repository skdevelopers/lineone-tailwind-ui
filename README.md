```markdown
# Lineone Tailwind UI Kit 🚀  
Multipurpose Admin & Web-App Starter built with **Tailwind CSS**  
*(Repo maintained by **Muhammad Salman Khalid** – “Salman”)*

---

## ✨ What’s inside?

| Module | Description |
| ------ | ----------- |
| **Dashboards** | Analytics, e-commerce, SaaS overview layouts |
| **Auth Pages** | Sign-in, sign-up, forgot-password, 2-FA |
| **CRUD Screens** | Table + form variants, modal create/edit |
| **Components** | Buttons, cards, alerts, tabs, dropdowns, charts |
| **Dark Mode** | Fully supported via Tailwind’s `dark:` variant |
| **RTL** | Pre-built RTL styles (`*-rtl` folders) |
| **ES6 Bundles** | Vanilla JS modules; Alpine JS ready |
| **Build Scripts** | Vite config with PurgeCSS, PostCSS, autoprefixer |

---

## 📦 Folder structure
```
lineone-tailwind-ui/
├─ Documentation/          # HTML docs & component showcase
├─ lineone-html/           # LTR static version
├─ lineone-html-rtl/       # RTL static version
├─ lineone-html-es6/       # ES6 modules (LTR)
├─ lineone-html-es6-rtl/   # ES6 modules (RTL)
└─ vite.config.js          # Build / hot-reload config
```

---

## 🚀 Quick start

1. **Clone the repo**

```bash
git clone https://github.com/skdevelopers/lineone-tailwind-ui.git
cd lineone-tailwind-ui
```

2. **Install dependencies**

```bash
npm install        # or pnpm / yarn
```

3. **Run in dev mode**

```bash
npm run dev        # Vite + Tailwind JIT
```

Open `http://localhost:5173` and start editing – hot-reload will reflect changes instantly.

4. **Production build**

```bash
npm run build      # outputs to /dist with minified CSS/JS
```

---

## 🛠️ Integrate with Laravel

```bash
# within a Laravel 10/11 project
npm install
npm install tailwindcss postcss autoprefixer vite --save-dev
cp -R path/to/lineone-tailwind-ui/resources/js ./resources/js/ui
cp -R path/to/lineone-tailwind-ui/resources/css ./resources/css/ui
```

Update `vite.config.js` and `tailwind.config.js` to include the new paths:

```js
export default defineConfig({
    plugins: [laravel({
        input: [
            'resources/css/app.css',
            'resources/css/ui/lineone.css',
            'resources/js/app.js',
            'resources/js/ui/index.js',
        ],
        refresh: true,
    })],
})
```

---

## 🖌️ Customisation

| Task | How |
| ---- | --- |
| **Change primary colour** | Update `tailwind.config.js → theme.extend.colors.primary` |
| **Enable dark mode** | Toggle `data-theme="dark"` on `<html>` or use Tailwind’s class strategy |
| **RTL build only** | `npm run build -- --env RTL=true` (see `package.json` script) |

---

## 🗺️ Roadmap

- Convert HTML pages into Blade components
- Vue 3/React component ports
- Figma design kit (in progress)
- Interactive charts examples with ApexCharts + Chart.js

---

## 🤝 Contributing

Pull requests welcome!  
1. Fork the repo  
2. Create a feature branch `git checkout -b feat/awesome`  
3. Commit & push `git commit -m "Add awesome feature"`  
4. Open a PR describing your change

---

## 📄 License

Personal & commercial use allowed under the **MIT License**.  
Please retain attribution in the source comments.

---

## 💬 Need help?

Open an issue or ping me on GitHub.

> Crafted with ❤️ by **Muhammad Salman Khalid** ([@skdevelopers](https://github.com/skdevelopers))
```
