# 🦏 NRCC Berlin Website
**Nepali Rhinos Cricket Club Berlin** — [nrccberlin.thegermanguy.org](https://nrccberlin.thegermanguy.org)

Est'd 2020 · President & Captain: Awanish

---

## 📁 Project Structure

```
nrccberlin/
├── index.html          ← Home · About NRCC · Berlin Weather · Join Us
├── gallery.html        ← Club Gallery (carousel + photo upload)
├── squad.html          ← Our Squad (search · filter · sort · player photos)
├── schedule.html       ← Fixtures & Match Schedule
├── css/
│   └── style.css       ← Shared styles (nav, footer, utilities)
├── js/
│   └── shared.js       ← Shared JS (nav, modals, scroll reveal)
├── lib/
│   ├── nrcc-logo.png   ← Club logo
│   ├── gallery/        ← Match & event photos (add here)
│   └── players/        ← Player photos (see naming rules below)
│       └── README.md
└── vercel.json         ← Vercel routing config
```

---

## 🚀 Deploy to Vercel

### Step 1 — Push to GitHub
```bash
git init
git add .
git commit -m "Initial NRCC Berlin website"
git remote add origin https://github.com/YOUR_USERNAME/nrccberlin.git
git push -u origin main
```

### Step 2 — Connect Vercel
1. Go to [vercel.com](https://vercel.com) → **New Project**
2. Import your GitHub repo
3. **Root Directory:** set to `nrccberlin` (or leave as-is if this folder is the repo root)
4. **Framework Preset:** Other (Static)
5. Click **Deploy**

### Step 3 — Add Custom Domain
1. In Vercel project → **Settings → Domains**
2. Add `nrccberlin.thegermanguy.org`
3. In your DNS provider, add a **CNAME** record:
   - Name: `nrccberlin`
   - Value: `cname.vercel-dns.com`

---

## 📸 Player Photos

Add player photos to `lib/players/`. Name rules:
- Lowercase, hyphens for spaces: `awanish.jpg`, `rajan-thapa.jpg`
- Supported: `.jpg`, `.jpeg`, `.png`, `.webp`
- Ideal size: **400×400px** square

See `lib/players/README.md` for the full list.

---

## ✏️ Updating Content

| Task | File | Where |
|---|---|---|
| Add/edit players | `squad.html` | `const players = [...]` array |
| Add fixtures | `schedule.html` | `const fixtures = [...]` array |
| Edit about text | `index.html` | `#about` section |
| Change weather location | `index.html` | `fetchWeather()` function |
| Add gallery photos | `lib/gallery/` | Drop image files here |

---

## 🎨 Brand Colors

| Color | Hex | Usage |
|---|---|---|
| Red | `#cc1117` | Primary accent, buttons |
| Cyan | `#00d4c8` | Secondary accent, links |
| Black | `#0a0a0a` | Background |
| Cream | `#f5f0ee` | Body text |

---

*Built by TGG with ❤️ for NRCC Berlin · 🦏 Rhinos Pride*
