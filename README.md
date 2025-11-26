# AnimeNexus🌸⚔️

### Modern Next.js 16 Server-Side Anime Streaming UI

## 📸 Preview

![image alt](https://github.com/M-tech-cmd/AnimeNexus/blob/597e08619f649db07606e41c9d1b5f1269a94c15/public/images/hero-preview.jpg)
![image alt](https://github.com/M-tech-cmd/AnimeNexus/blob/597e08619f649db07606e41c9d1b5f1269a94c15/public/images/anime-list-1.jpg)
![image alt](https://github.com/M-tech-cmd/AnimeNexus/blob/597e08619f649db07606e41c9d1b5f1269a94c15/public/images/anime-list-2.jpg)

AnimeFlow is a **modern Next.js 16** full-stack anime browsing experience featuring:

* ⚡ **Server Actions** for cleaner, faster, server-powered logic
* 🔄 **Infinite Scroll** for seamless episode & anime list loading
* 🎞 **Framer Motion Animations** for smooth transitions & UI effects
* 📡 **Optimized Server-Side Rendering (SSR)** for performance
* 🎌 A sleek, anime-inspired interface

---

## 🚀 Features

### ⚔️ **1. Server Actions — Simplified Logic & Better Performance**

Next.js **Server Actions** replace messy API routes, reducing client-side code and improving performance.

* Form handling without API endpoints
* Direct server-side DB/data operations
* Automatic caching & revalidation

### 🔄 **2. Infinite Scroll**

Smooth, uninterrupted browsing:

* Loads more anime as the user scrolls
* Built using Intersection Observer + server data calls
* Fast & responsive UI

### 🎞 **3. Framer Motion Animations**

AnimeFlow integrates modern animation effects:

* Page transitions
* Card hover animation
* Fade, slide, and stagger effects

### 🎌 **4. Clean, Modern UI**

Inspired by anime streaming platforms:

* Beautiful dark theme
* Responsive design
* Clean layout with smooth user experience

---

## 🛠 Tech Stack

**Framework:** Next.js 16 (App Router)

**Language:** TypeScript

**Styling:** TailwindCSS

**Animations:** Framer Motion

**Data Handling:** Server Actions + Fetch

**Features:** Infinite Scroll, SSR, Route Groups

---

## 📁 Folder Structure

```
animeflow/
├─ app/
│  ├─ actions/         # Server actions
│  ├─ anime/           # Anime pages
│  ├─ components/      # Reusable UI components
│  └─ layout.tsx
├─ public/
├─ styles/
└─ README.md
```

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/animeflow.git
cd animeflow
npm install
```

### Run Development Server

```bash
npm run dev
```

Navigate to:

```
http://localhost:3000
```

---

## 📡 Example Server Action

```ts
'use server'

export async function getAnimeList(page: number) {
  const res = await fetch(`https://api.example.com/anime?page=${page}`);
  return res.json();
}
```

Used directly in components without API routes.

---

## 🔄 Infinite Scroll Logic

```tsx
const observer = new IntersectionObserver((entries) => {
  if (entries[0].isIntersecting) fetchMore();
});
```

Smoothly loads additional anime data.

---

## 🎞 Animation Example

```tsx
<motion.div
  initial={{ opacity: 0, y: 20 }}
  animate={{ opacity: 1, y: 0 }}
  transition={{ duration: 0.4 }}
>
  <AnimeCard />
</motion.div>
```

---

## 📌 Future Enhancements

* 🔥 Anime streaming player
* ⭐ Favorites & user accounts
* 🔍 Advanced search & filters
* 🗂 Anime genres & categories system

---

## 📝 License

MIT License © M-tect-cmd

---
