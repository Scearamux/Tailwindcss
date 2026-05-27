# 🎨 Tailwind CSS — Starter Project

A minimal starter project to integrate **Tailwind CSS v3** with a modern build pipeline powered by **Parcel**, **PostCSS**, **PurgeCSS**, and **cssnano**.

---

## 🗂️ Project Structure

```
├── src/
│   └── ...              # CSS sources / assets
├── index.html           # HTML entry point
├── tailwind.config.js   # Tailwind CSS configuration
├── postcss.config.js    # PostCSS configuration
├── package.json
└── .gitignore
```

---

## ⚙️ Tech Stack

| Tool | Role |
|---|---|
| [Tailwind CSS v3](https://tailwindcss.com) | Utility-first CSS framework |
| [Parcel v2](https://parceljs.org) | Bundler / dev server |
| [PostCSS](https://postcss.org) | CSS transformation pipeline |
| [Autoprefixer](https://github.com/postcss/autoprefixer) | Automatic CSS vendor prefixes |
| [PurgeCSS](https://purgecss.com) | Removal of unused CSS classes |
| [cssnano](https://cssnano.github.io/cssnano/) | CSS minification for production |

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/Scearamux/Tailwindcss.git
cd Tailwindcss

# Install dependencies
npm install
```

---

## 🧑‍💻 Development

Start the development server with hot reload:

```bash
npm run dev
```

Parcel automatically serves `index.html` and watches for file changes in real time.

---

## 📦 Production Build

Generate optimized files (purged + minified CSS):

```bash
npm run build
```

Compiled files are output to the `dist/` folder.

---

## 🔧 Configuration

### Tailwind (`tailwind.config.js`)

Update the `content` array to tell Tailwind which files to scan for used classes:

```js
module.exports = {
  content: ['./index.html', './src/**/*.{html,js}'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### PostCSS (`postcss.config.js`)

The PostCSS pipeline includes Tailwind, Autoprefixer, PurgeCSS, and cssnano in production.

---

## 👤 Author

**Scearamux** — [GitHub](https://github.com/Scearamux)

---

## 📄 License

ISC
