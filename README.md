# Hive Architecture - Product Page

> 🐝 **Production-Ready Multi-Agent Ecosystem**
> A showcase website for Agent Zero's Hive architecture and its capabilities.

This repository contains a standalone, self-hosted static product website for the Hive architecture. It is **completely isolated** from the main Agent Zero project and can be deployed independently.

---

## 🎯 Purpose

This site demonstrates the key features and advantages of the Hive architecture over other agent frameworks. It is designed to be:

- ✅ **Fully self-contained** - Single HTML file with embedded CSS/JS (no external dependencies except fonts)
- ✅ **Dark mode by default** - Warm off-white (`#f0e6d2`) text on dark backgrounds (`#2d2d2d`)
- ✅ **Responsive** - Works on desktop and mobile
- ✅ **Fast** - Pure static HTML, no frameworks
- ✅ **GitHub Pages ready** - Automated deployment via GitHub Actions

---

## 🚀 Quick Start

### Deploy to GitHub Pages

1. **Create a new repository** on GitHub (e.g., `your-username/hive-architecture`)

2. **Push this code** to the repository:

```bash
git init
git add .
git commit -m "Initial commit: Hive architecture product page"
git branch -M main
git remote add origin https://github.com/your-username/hive-architecture.git
git push -u origin main
```

3. **Enable GitHub Pages** in repository settings:
   - Go to **Settings** → **Pages**
   - Source: **GitHub Actions**
   - The included workflow (`deploy.yml`) will automatically deploy on every push to `main`

4. **Access your site** at: `https://your-username.github.io/hive-architecture/`

---

## 📁 File Structure

```
.
├── index.html       # Main HTML page with embedded content
├── styles.css       # Dark mode stylesheet
├── script.js        # Interactive features (scroll effects, animations)
├── README.md        # This file
├── .gitignore       # Files to exclude from git
├── deploy.yml       # GitHub Actions workflow for Pages deployment
└── LICENSE          # MIT License
```

---

## 🎨 Customization

### Colors

CSS variables in `styles.css` define the color scheme:

```css
:root {
    --bg-primary: #2d2d2d;      /* Main background */
    --bg-secondary: #1a1a1a;    /* Alternate background */
    --text-primary: #f0e6d2;    /* Primary text (warm off-white) */
    --text-secondary: #eee8d5;  /* Secondary text */
    --accent: #ff6b6b;          /* Accent color (coral) */
    --accent-hover: #ff5252;    /* Accent on hover */
    --border: #3a3a3a;          /* Border color */
    --success: #4ecdc4;         /* Success messages */
}
```

To change the accent color, modify `--accent` and `--accent-hover` values.

### Content

Edit `index.html` to update:
- Hero section text and statistics
- Feature descriptions
- Skills list
- Integration examples
- Links and call-to-action buttons

### GitHub Repository Links

Replace placeholder URLs in `index.html`:

```
https://github.com/stupendous-software/skynet
```

With your actual repository URLs.

---

## 🔧 Technical Details

- **No build step required** - Just plain HTML/CSS/JS
- **CSS Framework**: Custom CSS with CSS Grid and Flexbox
- **Fonts**: Inter (Google Fonts) + JetBrains Mono for code
- **Responsive**: Mobile-first media queries
- **Animations**: CSS transitions and Intersection Observer API
- **Accessibility**: Proper heading hierarchy, ARIA labels where needed

---

## 📦 Deployment Options

### 1. GitHub Pages (Recommended)

Uses the provided `deploy.yml` GitHub Actions workflow. Automatically deploys on every push to `main`.

### 2. Manual

Simply upload `index.html`, `styles.css`, and `script.js` to any static hosting service:
- Netlify Drop
- Vercel
- Cloudflare Pages
- AWS S3 + CloudFront
- Any web server (nginx, Apache)

### 3. Docker

Create a simple Dockerfile:

```dockerfile
FROM nginx:alpine
COPY index.html /usr/share/nginx/html/
COPY styles.css /usr/share/nginx/html/
COPY script.js /usr/share/nginx/html/
EXPOSE 80
```

---

## 🤝 Contributing

This is a static product showcase. To contribute:

1. Fork the repository
2. Make your changes
3. Submit a Pull Request

Please keep the design consistent and follow the existing dark theme.

---

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

---

## 🔗 Links

- **Agent Zero Documentation**: https://agent-zero.ai
- **Agent Zero GitHub**: https://github.com/agent0ai/agent-zero
- **Skills Standard**: https://agentskills.io

---

Built with ❤️ for the Agent Zero ecosystem.
