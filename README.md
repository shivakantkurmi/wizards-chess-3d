# 🏰 Wizard's Chess 3D — Gothic Cathedral Edition

![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=for-the-badge&logo=three.js)
![Chess.js](https://img.shields.io/badge/Chess.js-0.10.3-d4af37?style=for-the-badge)
![Tone.js](https://img.shields.io/badge/Tone.js-14.8.49-9d4edd?style=for-the-badge)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.x-38bdf8?style=for-the-badge&logo=tailwind-css)
![License](https://img.shields.io/badge/License-MIT-emerald?style=for-the-badge)

A playable, zero-dependency **3D Wizard's Chess** web application set inside a minimalist Gothic cathedral sanctuary. Built entirely using procedural 3D geometry, procedural surface textures, and synthesized Web Audio, this project brings **Carrara Ivory Marble** and **Volcanic Slate-Obsidian** armies to life with custom idle, movement, combat wind-up, and 3D stone-shatter physics animations.

---

## ✨ Key Features

### 🏛️ 1. Minimalist 3D Gothic Cathedral Sanctuary
* **Architectural Environment**: Features an octagonal stepped altar dais, eight clustered Gothic piers with colonnettes, ribbed ceiling vaults converging on a gilded central boss stone, and procedural lancet stained-glass windows.
* **Atmospheric Lighting**: Illuminated by flickering corner braziers, a dedicated overhead sanctuary spotlight, warm/cool directional rim lights, and drifting golden dust motes.

### ♟️ 2. High-Contrast 64-Block 3D Chessboard
* **Individual Beveled Stone Blocks**: Every square is an individually raised 3D block (`BoxGeometry`) separated by recessed metallic brass channels (`0.06` unit grooves) and wrapped in crisp metallic edge bevels.
* **Procedural Stone Textures**: Dynamically generated HTML5 Canvas textures for **Warm Carrara Alabaster (`#f5f0e6`)** with gold/grey veins and **Deep Slate-Obsidian (`#2a3042`)** with crystalline violet fractures.
* **Engraved Coordinates**: `A–H` file and `1–8` rank brass engravings along all four borders of the basalt outer frame.

### 👑 3. Custom Sculpted 3D Piece Silhouettes (Staunton + Wizard's Chess)
All 32 pieces are procedurally sculpted in code using `THREE.LatheGeometry` turned-stone pedestals combined with articulated hierarchical armor and weaponry:
* **King**: Tallest stepped royal mantle topped with a high-arched Imperial Crown, a **3D Gothic Cross** at the apex, and a **two-handed broadsword** planted vertically down the front.
* **Queen**: Curved hourglass gown and collar topped with an open **8-pointed spiked royal coronet** (each spike tipped with a pearl sphere) and an ornate **royal orb-scepter**.
* **Bishop**: Turned pedestal with a stole, an authentic **split-cleft mitre** featuring a deep diagonal V-shaped notch, and a golden spiral **crosier staff**.
* **Knight**: Turned Staunton base supporting a multi-segment arched warhorse neck, sculpted equine cranium, tapered muzzle with lower jaw, flared nostrils, alert pointed ears, 8-plate flowing mane, and spiked **chanfron forehead armor**.
* **Rook**: Tapered masonry siege tower with 4 recessed Gothic arrow slits, flared corbel rings, **6 rectangular battlements (merlons and crenels)**, and a levitating arcane brazier core.
* **Pawn**: Turned Staunton pedestal, domed cuirass breastplate, sallet helmet with glowing visor slit, left-hand **medieval heater shield** with raised cross emblem, and right-hand **halberd poleaxe**.

### 💥 4. Custom Idle, Movement, Attack & Shatter Physics
* **Idle Animations**: Subtle asynchronous breathing and levitation of crowns, mitres, and weaponry.
* **Movement**: Smooth stone-on-stone gliding with dust puffs at takeoff and landing, plus high parabolic leaps for Knights.
* **3-Stage Combat & Shatter Engine**:
  1. **Advance**: Capturing pieces glide or leap to striking range facing their target.
  2. **Wind-Up**: The attacker rears back, raising its weapon and head as cathedral choir chords swell.
  3. **Lunge & Shatter**: The attacker strikes, shattering the defending piece into **45 physics-driven 3D stone and gold/amethyst shards** with gravity, floor bounce, angular tumbling, an expanding shockwave ring, and camera shake.

### 🔊 5. Procedural Cathedral Acoustics (Tone.js)
* **Zero External Audio Files**: All sound effects are synthesized in real time using `Tone.js`:
  * Brown-noise bandpass filters for heavy stone-on-stone sliding.
  * Membrane synthesizers for deep stone impact thuds.
  * High-pass white-noise bursts + low sub-bass drops for piece shattering.
  * Polyphonic triangle choir chords for piece selection, wind-ups, check alerts, and checkmate fanfare.

### 🎛️ 6. Single-Level Material Design 3 HUD
* **Top Navigation Bar**: Houses the live Turn & Check status badge, game mode switcher (`Vs AI` / `2P Local`), 4 camera presets (`White`, `Top-Down`, `Cathedral`, `Black`), `Battle Cam` toggle, `Strike Demo`, `Hint`, `Undo`, `Audio`, and `New Game`.
* **Bottom Status Bar**: Tracks shattered pieces for both armies, material point advantage (`+1`, `+5`, etc.), and a horizontally scrollable algebraic move history strip.

---

## 🛠️ Tech Stack

| Technology | Version | Purpose |
| :--- | :--- | :--- |
| **Three.js** | `r128` | 3D WebGL scene, procedural `LatheGeometry` models, lighting, shadows, and particle physics |
| **Chess.js** | `0.10.3` | Complete FIDE chess rules, legal move generation, castling, en passant, promotion, and checkmate detection |
| **Tone.js** | `14.8.49` | Real-time procedural Web Audio synthesis for stone slides, impacts, and shatter acoustics |
| **Tailwind CSS** | `3.x (CDN)` | Material Design 3 dark glassmorphism HUD and responsive layout |
| **Google Fonts** | `Cinzel` & `Inter` | Gothic cathedral display typography paired with clean Material UI text |

---


## 🤖 AI-Assisted Development

This project stands as an example of how far **AI-assisted software development has progressed**. The application was made **entirely with the assistance of AI**, from the initial concept and architectural planning to the implementation of the 3D environment, procedural chess pieces, animations, physics, audio system, user interface, and supporting game logic.

AI was used extensively throughout the development process to generate, refine, and integrate the project's code and systems. This includes the procedural 3D geometry, Gothic cathedral environment, chess mechanics, combat and shatter effects, camera systems, synthesized audio, UI components, and gameplay functionality.

The project demonstrates the increasingly powerful role of modern AI as a development partner capable of assisting with a complex, multi-system interactive application — including **3D graphics, game logic, physics, animation, audio, interface design, and software architecture — within a single project**.

> **This project was made entirely with AI assistance, demonstrating the remarkable capabilities of modern AI in turning a high-level creative concept into a functional, interactive 3D application.**

AI-generated output was reviewed, integrated, tested, and refined during development to produce the final working application.

---

## 🚀 Getting Started

Because the entire application is self-contained with zero build steps required, you can run it immediately in any modern web browser.

### Option 1: Direct Launch
1. Clone the repository:
   ~~~bash
   git clone https://github.com/your-username/wizards-chess-3d.git
   cd wizards-chess-3d
   ~~~
2. Double-click `index.html` to open it directly in Chrome, Firefox, Edge, or Safari.

### Option 2: Run with a Local Development Server (Recommended)
Using a local server ensures optimal WebGL and Web Audio API behavior:

* **Using Python**:
  ~~~bash
  python -m http.server 8000
  ~~~
  Then open `http://localhost:8000` in your browser.

* **Using Node.js (`npx`)**:
  ~~~bash
  npx serve .
  ~~~

* **Using VS Code**:
  Install the **Live Server** extension, right-click `index.html`, and select **"Open with Live Server"**.

---

## 🎮 Controls & Navigation

### 🖱️ Mouse & Touch Camera Controls
| Action | Mouse | Touch (Mobile / Tablet) |
| :--- | :--- | :--- |
| **Select / Move Piece** | `Left-Click` on a piece or highlighted block | `Tap` on a piece or highlighted block |
| **Orbit Camera** | `Left-Click + Drag` | `One-Finger Drag` |
| **Zoom In / Out** | `Scroll Wheel` | `Two-Finger Pinch` |
| **Pan Camera** | `Right-Click + Drag` | `Two-Finger Drag` |

### 🧭 Top Bar Quick Actions
* **Vs AI / 2P Local**: Switch between playing against the tactical Cathedral AI (plays Black Obsidian) or Two-Player local pass-and-play.
* **White / Top-Down / Cathedral / Black**: Smoothly interpolate the camera to predefined tactical or cinematic angles.
* **Battle Cam**: Toggles automatic dramatic camera zoom during piece captures.
* **⚡ Strike Demo**: Immediately executes a legal capture (or stages an instant tactical strike if none is currently available) so you can test the combat and shatter physics at any time.
* **💡 Hint**: Evaluates the current board state and highlights the strongest tactical move in cyan.
* **↩️ Undo**: Reverts the last turn (or full player + AI round) and restores any shattered pieces.

---

## 📂 Project Structure

~~~text
wizards-chess-3d/
├── index.html       # Complete self-contained 3D web application (HTML, CSS, Three.js, Chess.js, Tone.js)
└── README.md        # Project documentation
~~~

---

## 🌐 Deploying to GitHub Pages

1. Push your code to your GitHub repository.
2. Go to **Settings** → **Pages** in your repository.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Choose the `main` (or `master`) branch and `/ (root)` folder, then click **Save**.
5. Your playable 3D Wizard's Chess sanctuary will be live at `https://your-username.github.io/wizards-chess-3d/`.

---

## 📄 License

Distributed under the **MIT License**. Free to use, modify, and distribute for personal or educational projects.