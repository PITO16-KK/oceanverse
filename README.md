# 🌊 Oceanverse — Beneath the Waves

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0:071728,30:176b94,70:408fa9,100:a6c6c4&height=220&section=header&text=OCEANVERSE&fontSize=52&fontColor=effaff&fontAlignY=38&desc=An%20immersive,%20interactive%20voyage%20through%20the%20depths%20of%20the%20ocean.&descFontSize=18&descAlignY=62&descColor=effaffc0" alt="Oceanverse Banner" width="100%" />
</p>

<p align="center">
  <a href="#-the-voyage-chapters"><img src="https://img.shields.io/badge/Chapters-I_to_VI-0ea5e9?style=for-the-badge&logo=compass&logoColor=white" alt="Chapters"></a>
  <a href="#-the-ocean-journal"><img src="https://img.shields.io/badge/Journal-16_Treasures-f59e0b?style=for-the-badge&logo=book&logoColor=white" alt="Journal"></a>
  <a href="#-procedural-synthesizer"><img src="https://img.shields.io/badge/Audio-Web_Audio_API-10b981?style=for-the-badge&logo=soundcharts&logoColor=white" alt="Web Audio"></a>
  <a href="#-tech-stack"><img src="https://img.shields.io/badge/Dependencies-Zero_Vanilla-6366f1?style=for-the-badge&logo=javascript&logoColor=white" alt="Zero Dependencies"></a>
  <a href="https://pito16-kk.github.io/oceanverse/"><img src="https://img.shields.io/badge/Live_Demo-GitHub_Pages-22c55e?style=for-the-badge&logo=github&logoColor=white" alt="Live Demo"></a>
</p>

---

## 🧭 About Oceanverse

**Oceanverse** is an atmospheric, scroll-driven interactive web experience that invites you to dive from a sun-drenched tropical shore all the way down into the deepest, darkest ocean trench.

Built with a philosophy of **"Scroll to Explore, Click to Interact"**, each depth level introduces unique visual landscapes, handcrafted watercolor marine life, dynamic physics, procedural soundscapes, and hidden artifacts to collect in your personal **Ocean Journal**.

---

## 🗺️ The Voyage (Chapters)

```
        00 M ─────────────────── [ Chapter I: The Shore ] ────────────── (Sunlight, Ripples & Shells)
         │
        10 M ─────────────────── [ Chapter II: Into the Blue ] ───────── (Bubbles & Silverfin Fish)
         │
        30 M ─────────────────── [ Chapter III: The Coral Garden ] ───── (Watercolor Reef & Feeding)
         │
       200 M ─────────────────── [ Chapter IV: The Jellyfish Kingdom ] ─ (Bioluminescence & Guide)
         │
       500 M ─────────────────── [ Chapter V: The Whale Sanctuary ] ─── (Playful Whales & Deep Call)
         │
     1,000 M ─────────────────── [ Chapter VI: The Lost Treasure ] ──── (Sunken Ruins & Ocean's Heart)
```

### 🏖️ Chapter I · The Shore (00 M)
*Where the sky meets the sea.*
- Swaying clouds and procedural tide ripples along the sandy shore.
- Interactive pastel shells with resonant glass chimes.
- Glowing cursor particle trail and sound toggle.

### 🫧 Chapter II · Into the Blue (10 M)
*Leave the world above behind.*
- Soft underwater sunbeams (god-rays) that tilt with your scroll parallax.
- School of glistening silverfin fish swimming across the blue.
- Poppable bubbles and the first secret **Ocean Pearl**.

### 🪸 Chapter III · The Coral Garden (30 M)
*Life blooms beneath the blue.*
- Handcrafted watercolor corals blooming across multi-layered dunes.
- Gliding sea turtle, gentle coral fish, and a camouflaged seahorse.
- An interactive pearl clam that opens to yield the **Garden Pearl**.
- Fish feeding mechanism: drop food pellets to feed the school!

### 🪼 Chapter IV · The Jellyfish Kingdom (200 M)
*Even in darkness, life finds a way to shine.*
- Twilight ocean realm glowing with bioluminescent species (Moon, Azure, and Rose Jellies).
- **Grab & Guide Mechanic**: Click and hold a jellyfish to guide it through the abyss; its tentacles dynamically react to your movement vector with physics inertia, then release to swim freely.

### 🐋 Chapter V · The Whale Sanctuary (500 M)
*In the silence of the deep, giants dance.*
- A deep-sea sanctuary inhabited by a gentle Blue Whale mother and her playful calf.
- **Playful Whale Escape**: Click the whales to watch them turn and gracefully glide away with dynamic pitch tilt, bubble wakes, and bioluminescent trails.
- Plankton sparkles and a haunting procedural whale call synthesizer.

### 🗝️ Chapter VI · The Lost Treasure (1,000 M)
*The greatest treasures are found by those who dare to explore.*
- Mysterious sunken ruins framed by ancient stone colonnades and glowing sea flora.
- **Mini-Game**: Search for **3 antique gold keys** hidden in the ruins:
  - An alcove key glinting on the left ruin pillar.
  - A shiftable ancient rock on the right that you can slide or drag aside to reveal a hidden key.
  - A floor stone key resting on the ocean bed.
- **The Ancient Chest**: Rattles with a warning if locked; when all 3 keys are collected, click to trigger a triumphant cinematic opening with 36 radiant golden spark particles and procedural arpeggio fanfare, revealing the legendary **Ocean's Heart**.

---

## 📖 The Ocean Journal

Keep track of your discoveries throughout your journey. The **Ocean Journal** persists your progress across browser sessions via `localStorage`:

| # | Artifact / Creature | Depth | Chapter |
|---|---------------------|-------|---------|
| 1 | Rose Scallop | 00 M | The Shore |
| 2 | Azure Scallop | 00 M | The Shore |
| 3 | Little Pearl Shell | 00 M | The Shore |
| 4 | Ocean Pearl | 10 M | Into the Blue |
| 5 | Silverfin Fish | 10 M | Into the Blue |
| 6 | Sea Turtle | 30 M | The Coral Garden |
| 7 | Hidden Seahorse | 30 M | The Coral Garden |
| 8 | Garden Pearl | 30 M | The Coral Garden |
| 9 | Coral Fish | 30 M | The Coral Garden |
| 10 | Moon Jelly | 200 M | The Jellyfish Kingdom |
| 11 | Azure Jelly | 200 M | The Jellyfish Kingdom |
| 12 | Rose Jelly | 200 M | The Jellyfish Kingdom |
| 13 | Blue Whale | 500 M | The Whale Sanctuary |
| 14 | Whale Calf | 500 M | The Whale Sanctuary |
| 15 | Luminous Plankton | 500 M | The Whale Sanctuary |
| 16 | **Ocean's Heart** | 1,000 M | The Lost Treasure |

---

## 🎵 Procedural Synthesizer (Zero Audio Files)

Oceanverse requires **zero audio files** (`.mp3` / `.wav`), keeping load times instantaneous. All soundscapes are synthesized on the fly via the native browser **Web Audio API**:

- 🔔 **Bell & Scallop Chimes**: Sine wave frequency modulation with exponential decays.
- 🫧 **Bubble Pop**: Quick pitch ramp sweep from 440 Hz to 880 Hz.
- ✨ **Pearl & Plankton Shimmer**: Sparkling harmonics (triangle and high-sine oscillators).
- 🪼 **Jellyfish Pulse**: Ethereal bioluminescent chords (E5 to E6).
- 🐋 **Whale Song**: Dual-oscillator harmonic sweep (160 Hz down to 56 Hz) with resonant low-frequency depth.
- 🪨 **Ancient Rock Slide**: Low sawtooth stone rumble.
- 🗝️ **Key Pickup**: Antique metallic high-register chime.
- 🏆 **Treasure Fanfare**: 4-note ascending C-major arpeggio (C5 → E5 → G5 → C6) with golden reverb decay.

---

## 💻 Tech Stack & Architecture

- **Core**: Vanilla HTML5, CSS3, JavaScript (ES2022).
- **Styling**: Modern CSS Grid & Flexbox, CSS Variables, Backdrop Filters (Glassmorphism), SVG Masks.
- **Audio Engine**: Pure Web Audio API (`AudioContext`, `OscillatorNode`, `GainNode`).
- **Physics & Motion**: Pointer Events with `setPointerCapture`, `requestAnimationFrame` render loops, CSS Keyframe hardware acceleration.
- **Storage**: `localStorage` automatic state serialization.
- **Dependencies**: **0 (Zero)** — no external frameworks, libraries, or build tools required.

---

## 🚀 Quick Start & Deployment

### Running Locally
No installation or build step needed. Simply clone and open:

```bash
git clone https://github.com/PITO16-KK/oceanverse.git
cd oceanverse
```

Open `index.html` in any modern web browser, or launch a lightweight local server:

```bash
# Using Python
python -m http.server 8000

# Using Node (npx)
npx serve
```

### GitHub Pages Setup
1. Go to your repository on GitHub: **Settings > Pages**.
2. Under **Build and deployment > Branch**, select `main` and root directory `/`.
3. Click **Save**. Your site will be live at:
   `https://<username>.github.io/oceanverse/`

---

## ♿ Accessibility

- Respects `prefers-reduced-motion` by disabling parallax shifts, cursor trails, and active particle physics for users who prefer reduced movement.
- Semantic HTML tags (`<header>`, `<main>`, `<section>`, `<dialog>`) with descriptive `aria-label` and `aria-live` attributes.
- Minimum **44px touch targets** on all interactive buttons and elements for mobile accessibility.

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

<p align="center">
  Crafted with care for ocean dreamers and explorers by <a href="https://github.com/PITO16-KK"><b>PITO16-KK</b></a>.
</p>
