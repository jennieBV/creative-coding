# Creative Coding: Geometric Eye

An interactive generative artwork exploring sacred geometry, trigonometric patterns, and dynamic gaze tracking implemented with pure HTML5 Canvas and vanilla JavaScript.

![Geometric Eye Preview](https://img.shields.io/badge/Creative%20Coding-Canvas%202D-00f0ff?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow?style=for-the-badge&logo=javascript)

## Features

- **Sacred Geometry**: Mathematical Vesica Piscis contour constructed via symmetric cubic Bézier tension arcs.
- **Dynamic Iris Mandala**: Star polygons, rotating hexagrams, and overlapping Flower-of-Life circular arcs.
- **Organic Mouse Gaze Tracking**: The iris and pupil follow your cursor with smooth linear interpolation (`lerp`).
- **Organic Blink Cycle**: Interactive click-to-blink with sinusoidal eyelid kinematics and spontaneous blinking.
- **Real-Time Interactive Controls**:
  - Radiating solar ray density (8 to 72 rays).
  - Pupil dilation and breathing pulse.
  - Animation speed.
  - Color palette switcher (*Cyber Cyan & Gold*, *Mystic Violet*, *Emerald Matrix*, *Solar Flare*, *Silver Minimal*).
  - Gaze tracking toggle and randomizer.
- **Zero Dependencies**: Pure HTML5 Canvas & vanilla JavaScript—runs directly in any modern browser.

## Running Locally

### Option 1: Open Directly
On macOS:
```bash
open index.html
```
Or simply double-click `index.html` in your file manager.

### Option 2: Local HTTP Server
Using Python:
```bash
python3 -m http.server 8000
```
Then navigate to [http://localhost:8000](http://localhost:8000).

Using Node (`npx`):
```bash
npx serve .
```

## Mathematical Concepts

1. **Vesica Piscis**: The archetypal geometry of the eye formed by the lens created when two circles of radius $R$ intersect at each other's centers.
2. **Polar Coordinates**: Calculating ray tips and mandala nodes using:
   $$x = r \cos(\theta), \quad y = r \sin(\theta)$$
3. **Smooth Damping (Lerp)**:
   $$\vec{P}_{t+1} = \vec{P}_t + (\vec{P}_{\text{target}} - \vec{P}_t) \times \alpha$$
