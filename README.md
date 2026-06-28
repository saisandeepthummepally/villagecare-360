# VillageCare 360 — 3D Animated Website

An immersive, single-page 3D website for **VillageCare 360 – Urban–Rural Healthcare Connectivity System**, built from the Team MEDITECH (ID SKH009) presentation.

It tells the full story — problem, objective, telemedicine, architecture, technology, workflow, features, benefits, future, social impact, conclusion, and team — as one scrolling experience with a live WebGL background.

## ✨ Highlights
- **Live 3D background** (Three.js): a rotating wireframe globe with glowing rural→urban connection arcs, travelling data pulses, and an additive particle starfield. Mouse parallax + scroll-driven camera.
- **Scroll animations** (GSAP + ScrollTrigger): section reveals, staggered cards, animated architecture pipeline, vertical workflow timeline, and count-up impact stats.
- **Futuristic medical theme**: dark navy, glowing teal/cyan accents, glassmorphism cards with 3D hover tilt.
- **100% offline · no API keys**: Three.js and GSAP are vendored locally in `/lib`. Nothing is fetched at runtime — no CDN, no keys, no tracking.
- **Responsive** + honours `prefers-reduced-motion`.

## ▶️ How to run
Because browsers restrict local file scripts, serve the folder with any static server:

```bash
# Python (already on most machines)
python -m http.server 8000
```
Then open <http://localhost:8000>.

Other options: `npx serve`, VS Code "Live Server", or any static host. Opening `index.html` directly may also work in some browsers, but a local server is recommended.

## 📁 Structure
```
112/
├── index.html        # all sections + navigation
├── css/style.css     # theme, glassmorphism, layout, responsive, reduced-motion
├── js/scene.js       # Three.js background scene (globe + arcs + particles)
├── js/main.js        # nav, scroll progress, reveals, counters, card tilt
└── lib/              # vendored Three.js + GSAP + ScrollTrigger (offline)
```

## 👥 Team MEDITECH (SKH009)
Sai Sandeep · Vinay · Vishnu Vardhan · Asifuddin

> Note: numbers in the *Social Impact* section are illustrative/projected figures for presentation purposes.
