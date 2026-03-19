<div align="center">

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a0030,50:3b0764,100:6b21a8&height=200&section=header&text=Happy+Birthday+Animation&fontSize=46&fontColor=ffffff&fontAlignY=38&desc=A+beautiful+animated+birthday+wish+built+with+HTML%2C+CSS+and+JavaScript&descAlignY=60&descSize=14&descColor=d8b4fe" width="100%"/>

<br/>

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![MIT License](https://img.shields.io/badge/License-MIT-22c55e?style=flat-square)](LICENSE)
[![Deployed](https://img.shields.io/badge/Deployed-GitHub%20Pages-0ea5e9?style=flat-square&logo=github)](https://safin313-stack.github.io/Happy-Birthday-Animation/)
[![Made with Love](https://img.shields.io/badge/Made%20with-Love-6b21a8?style=flat-square)]()

<br/>

<a href="https://safin313-stack.github.io/Happy-Birthday-Animation/">
  <img src="https://img.shields.io/badge/-%F0%9F%8E%82%20%20LIVE%20DEMO%20%20%E2%86%92-3b0764?style=for-the-badge&logoColor=white" alt="Live Demo" height="42"/>
</a>

<br/>
<sub>✦ No login &nbsp;·&nbsp; No install &nbsp;·&nbsp; Opens instantly in your browser ✦</sub>

<br/><br/>

</div>

---

<div align="center">

### 🎂 Features

| 🎉 Birthday Animation | ✨ Particle Effects | 🎈 Balloons | 🎆 Fireworks | 🎵 Celebration Vibe | 📱 Responsive |
|:---:|:---:|:---:|:---:|:---:|:---:|
| Animated birthday wish sequence | Dynamic particle and sparkle effects | Floating balloon animations | Colorful firework bursts | Festive colors and smooth transitions | Works beautifully on all screen sizes |

</div>

---

## 🖥️ Animation Preview

```
╔══════════════════════════════════════════════════════════╗
║                                                          ║
║   🎆  *  · ✦  *   🎆  ·  *  ✦   *   🎆                 ║
║                                                          ║
║         🎈      🎈           🎈       🎈                 ║
║            🎈         🎈        🎈                       ║
║                                                          ║
║         ✨  Happy Birthday!  ✨                          ║
║                                                          ║
║     🎂  Wishing you a wonderful day  🎂                  ║
║                                                          ║
║   ✦  *  · 🎆  *   ·  ✦  *  🎆   ·  *  ✦               ║
║                                                          ║
╚══════════════════════════════════════════════════════════╝
       🎉 particles flying · balloons floating 🎉
```

---

## 🎨 How It Works

### JavaScript-Powered Particle Engine

```js
// Particles generated dynamically and animated with JS
function createParticle() {
  const particle = document.createElement('div');
  particle.classList.add('particle');
  particle.style.left  = Math.random() * 100 + 'vw';
  particle.style.top   = Math.random() * 100 + 'vh';
  particle.style.animationDuration = Math.random() * 3 + 2 + 's';
  particle.style.backgroundColor   = randomColor();
  document.body.appendChild(particle);
}
```

### Animated Text Reveal

```css
/* Birthday text animates in with keyframes */
@keyframes textReveal {
  0%   { opacity: 0; transform: scale(0.5) translateY(30px); }
  60%  { transform: scale(1.1); }
  100% { opacity: 1; transform: scale(1) translateY(0); }
}

.birthday-text {
  animation: textReveal 1.5s cubic-bezier(.68, -.55, .27, 1.55) forwards;
}
```

### Balloon Float Animation

```css
@keyframes balloonFloat {
  0%   { transform: translateY(100vh) rotate(-5deg); opacity: 0; }
  10%  { opacity: 1; }
  90%  { opacity: 1; }
  100% { transform: translateY(-20vh) rotate(5deg); opacity: 0; }
}

.balloon {
  animation: balloonFloat linear infinite;
  animation-duration: calc(3s + var(--delay));
}
```

### Firework Burst

```js
// Firework explosion at random positions
function launchFirework(x, y) {
  for (let i = 0; i < 30; i++) {
    const spark = document.createElement('div');
    spark.classList.add('spark');
    const angle  = (i / 30) * 360;
    const radius = Math.random() * 80 + 40;
    spark.style.setProperty('--angle',  angle  + 'deg');
    spark.style.setProperty('--radius', radius + 'px');
    spark.style.left = x + 'px';
    spark.style.top  = y + 'px';
    document.body.appendChild(spark);
  }
}
```

---

## 📁 Project Structure

```
Happy-Birthday-Animation/
│
├── 📄 index.html    ← Page structure and birthday message
├── 🎨 style.css     ← Animations, colors, layout, responsive
├── ⚙️  app.js       ← Particle engine, fireworks, balloon logic
└── 📄 README.md     ← Project documentation
```

---

## 🚀 Run It Yourself

**Option 1 — Live (instant, no setup)**

> 🔗 **[https://safin313-stack.github.io/Happy-Birthday-Animation/](https://safin313-stack.github.io/Happy-Birthday-Animation/)**

**Option 2 — Clone and open locally**

```bash
git clone https://github.com/Safin313-stack/Happy-Birthday-Animation.git
open index.html
```

**Option 3 — VS Code Live Server**

```
1. Install Live Server extension
2. Right-click index.html → Open with Live Server ✅
```

---

## 🛠️ Tech Stack

```
┌──────────────────────────────────────────────────┐
│           Frontend · Zero Dependencies           │
├─────────────────┬────────────────────────────────┤
│  HTML5          │  Page structure                │
│  CSS3           │  Animations · keyframes        │
│  JavaScript     │  Particles · fireworks · logic │
└─────────────────┴────────────────────────────────┘
```

---

## 📚 Key Concepts Used

```
@keyframes          → text reveal · balloon float · spark burst animations
Math.random()       → random positions · colors · timing for particles
createElement()     → dynamically generate particles and sparks
CSS custom props    → --delay · --angle · --radius for varied animations
cubic-bezier()      → bouncy easing on text reveal
requestAnimationFrame → smooth continuous animation loop
```

---

## 💡 Credits & Inspiration

Special thanks to **TCW - AI & coding resources** (Telegram Community)
for ideas, guidance, and coding support throughout this project. 🙏

---

<div align="center">

## 👤 Developer

<br/>

**Saharia Hassan Safin**
Front-end Developer

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-Safin313--stack-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Safin313-stack)
&nbsp;
[![Live Project](https://img.shields.io/badge/Live%20Project-Visit%20Now-3b0764?style=for-the-badge&logo=vercel&logoColor=white)](https://safin313-stack.github.io/Happy-Birthday-Animation/)

<br/>

*"Because every birthday deserves a little magic in code"* 🎂

<br/>

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6b21a8,50:3b0764,100:1a0030&height=120&section=footer" width="100%"/>

<sub>MIT License · © 2025 Saharia Hassan Safin · ⭐ Star this repo if it made you smile!</sub>

</div>
