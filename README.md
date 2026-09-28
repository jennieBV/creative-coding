# 🏛️ Creative Coding Gallery

> An interactive digital art exhibition showcasing generative mathematics, sacred geometry, and terminal glyph sculptures.

**Live Exhibition**: [https://jennieBV.github.io/creative-coding/](https://jennieBV.github.io/creative-coding/)

---

## 🎨 Exhibition Rooms

### [Room 01 // The Geometric Eye](01-geometric-eye/index.html)
* **Medium**: Pure HTML5 Canvas 2D & Trigonometric Vector Harmonics
* **Concept**: A generative *Vesica Piscis* sacred geometry eye. Radiating harmonic rays intersect concentric polar circles with an interactive iris and pupil.
* **Interactions**:
  * Real-time cursor gaze tracking with smooth `lerp` inertia.
  * Interactive control drawer with real-time sliders (ray count, pupil dilation, speed, oscillation harmonics).
  * One-click aesthetic presets (*Sacred Gold*, *Cyberpunk*, *Solar Flare*, *Ethereal*).

---

### [Room 02 // Cyber Heritage](02-terminal-heritage/index.html)
* **Medium**: Terminal ASCII Glyph Sculpture & 24-Bit RGB
* **Concept**: Algorithmic translation of traditional Bulgarian folklore attire into an interactive terminal CLI logo. Reconstructs the male figure (*tall black kalpak cap and crimson elek vest*) and female figure (*golden floral headdress, coins, and royal blue sukman*) from photographic archetypes.
* **Interactions**:
  * **Intro Scanline Reveal**: A CRT electron beam scans down and dynamically decrypts characters into place on launch.
  * **Ambient Phosphor Breathe**: A slow, meditative luminance breathing cycle.
  * **Magnetic Fluid Shimmer**: Hovering your cursor over the figures gently shifts glyphs like magnetic liquid mercury with temporary digital runic scramble.
  * **Clipboard Export**: Click "Copy ASCII" to copy the full ASCII sculpture to paste into any terminal.

---

## 📐 Mathematical & Algorithmic Concepts

1. **Vesica Piscis**: The archetypal geometry formed by the lens created when two circles of radius $R$ intersect at each other's centers.
2. **Polar Coordinates**: Calculating ray tips and mandala nodes using:
   $$x = r \cos(\theta), \quad y = r \sin(\theta)$$
3. **Smooth Damping (Lerp)**:
   $$\vec{P}_{t+1} = \vec{P}_t + (\vec{P}_{\text{target}} - \vec{P}_t) \times \alpha$$
4. **Luminance Mapping & Aspect Correction**: Converting 24-bit RGB pixel channels to terminal character density ramps with aspect-ratio compensation.

---

## ⌨️ Gallery Navigation & Keyboard Shortcuts

* **`1` / `2`**: Jump directly into Piece 01 or Piece 02 from anywhere.
* **`←` / `→` (Arrow Keys)**: Seamlessly glide to the previous or next exhibition room.
* **`ESC` or `G`**: Return to the main Gallery Exhibition Hall.

---

## 🚀 How to Host on GitHub Pages

1. Go to your repository on GitHub: [https://github.com/jennieBV/creative-coding](https://github.com/jennieBV/creative-coding)
2. Click on **Settings** (tab at the top).
3. In the left sidebar, click **Pages**.
4. Under **Build and deployment**:
   * **Source**: `Deploy from a branch`
   * **Branch**: `main`
   * **Folder**: `/ (root)`
5. Click **Save**.
6. Within ~1 minute, your digital art gallery will be live at:
   ```
   https://jennieBV.github.io/creative-coding/
   ```

---

## 💻 Local Preview

Double-click `index.html` to open directly in any web browser, or launch a local web server:

```bash
python3 -m http.server 8000
```
Then visit [http://localhost:8000](http://localhost:8000).

---

## 📂 Project Architecture

```text
creative-coding/
├── index.html                   # 🏛️ Digital Art Gallery Exhibition Hall
├── 01-geometric-eye/
│   └── index.html               # 👁️ Piece 01: Sacred Geometry Eye
├── 02-terminal-heritage/
│   └── index.html               # 🏛️ Piece 02: Terminal ASCII Sculpture
├── img_1_1765648020127.jpg      # Source photographic reference
├── style_1.gif                  # Aesthetic reference study
└── README.md                    # Documentation & exhibition notes
```

&copy; 2026 Jennie BV. All creative coding sketches created with vanilla JavaScript and HTML5 Canvas. Zero dependencies.
