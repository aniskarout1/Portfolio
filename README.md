# Portfolio OS 🖥️

An interactive macOS-style developer portfolio built with **React + Vite**.

## Features

- 🖥️ macOS-style desktop environment
- 🪟 Draggable windows — About Me, Projects, Career, Resume, Contact
- 🚢 Animated dock with hover magnification & active-app indicators
- 🖼️ Wallpaper picker with 5 built-in backgrounds
- 🔒 Lock screen with PIN pad (enter any 4 digits to unlock)
- ⏻ Logout / power-on screen
- ⚙️ System settings dropdown menu

## Getting Started

### Prerequisites
- Node.js 18+
- npm or yarn

### Install & Run

```bash
# Install dependencies
npm install

# Start dev server (opens at http://localhost:5173)
npm run dev
```

### Build for Production

```bash
npm run build
```

Output is in the `/dist` folder — deploy anywhere.

### Preview Production Build

```bash
npm run preview
```

## Project Structure

```
portfolio-os/
├── index.html            ← Vite HTML entry (root level)
├── vite.config.js        ← Vite + React plugin config
├── package.json
├── src/
│   ├── main.jsx          ← React root mount
│   ├── App.jsx           ← All components & logic
│   └── index.css         ← Global reset & scrollbar styles
└── public/               ← Static assets (favicon etc.)
```

## Customization

Edit `src/App.jsx` and find:

| What to change | Search for |
|---|---|
| Your name & bio | `Alex Mercer` |
| Projects | `const projects = [` inside `ProjectsWindow` |
| Career history | `const jobs = [` inside `CareerWindow` |
| Skills | skill grid inside `AboutWindow` |
| Contact links | socials array inside `ContactWindow` |
| Default wallpaper | `useState(WALLPAPERS[3].src)` |

## Deployment

```bash
# Netlify
netlify deploy --prod --dir=dist

# Vercel
vercel --prod

# GitHub Pages (with vite.config base set)
npm run build && gh-pages -d dist
```
"# Portfolio" 
