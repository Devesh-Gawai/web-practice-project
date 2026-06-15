# ✦ GestureAR Studio v1.0 ✦

<p align="center">
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan.svg?style=for-the-badge" alt="Version" />
  <img src="https://img.shields.io/badge/Environment-Web_Browser-magenta.svg?style=for-the-badge" alt="Environment" />
  <img src="https://img.shields.io/badge/Maintained-Practice_Project-orange.svg?style=for-the-badge" alt="Status" />
  <img src="https://img.shields.io/badge/AI_Assisted-Claude_Sonnet_4.6-purple.svg?style=for-the-badge" alt="AI Assisted" />
</p>

---

## 🚀 Overview

**GestureAR Studio** is an interactive, browser-based 3D workspace designed for real-time spatial computing without requiring dedicated VR hardware. By leveraging your webcam and microphone, the application maps spatial workflows onto a 3D WebGL engine, allowing you to create, manipulate, and simulate physics on 3D primitives completely through **natural hand gestures** and **voice commands**.

> 💡 **Presentation Node:** Open `[gesture-ar-studio.html](https://devesh-gawai.github.io/web-practice-project/gesture-ar-studio/GESTURE_AR_STUDIO.html)` directly in any modern browser, grant webcam access, and instantly interact with a fluid, multi-modal augmented workspace!

---

## 🎨 System Interface Presentation

```text
┌──────────────────────────────────────────────────────────────────────────┐
│                             HEADER BAR                                   │
│  [✦ GESTURE AR STUDIO]       [• TRACKING]     [⚛ PHYSICS]    [🔬 DEBUG] │
├─────────────────────────┬────────────────────────┬───────────────────────┤
│                         │                        │                       │
│       LEFT PANEL        │     CENTER CANVAS      │      RIGHT PANEL      │
│  ┌───────────────────┐  │                        │  ┌─────────────────┐  │
│  │  8x 3D Shapes     │  │     Camera Feed        │  │ Performance     │  │
│  │  8x Materials    │  │          +             │  │ Metrics (FPS)   │  │
│  │  7x Colors        │  │     3D Primitives      │  │ Hand Stats      │  │
│  │  [＋ SPAWN OBJECT]│  │                        │  │ Selected Obj    │  │
│  └───────────────────┘  │                        │  └─────────────────┘  │
│                         │                        │                       │
├─────────────────────────┴────────────────────────┴───────────────────────┤
│  [↖ Mode Toolbar]          [✋ GESTURE HUD]            [🎤 Voice Listening]│
└──────────────────────────────────────────────────────────────────────────┘



✨ Key Features
1. ✋ Real-time Hand Gesture Framework
The system uses automated frames debouncing (4+ frames stabilization) to maximize recognition confidence:

✋ Open Palm: Object Selection & Hovering (triggers a custom cyan screen ring highlight)

🤏 Pinch Motion: Dynamic Grab & Move translation across standard 3D coordinate space with 35% linear interpolation (lerp) blending

🤞 Double Pinch: Object Cloning/Duplication (instantly copies shapes, colors, and materials with a 1.2s safety cooldown)

✊ Closed Fist: Object Deletion/Removal (wipes a target from the canvas, with instant Toast feedback)

☝️ Point Index: Teleportation tracking via camera-to-hand raycasting (15% snappy lerp tracking)

🖐️ Fingers Spread: Uniform Scaling Up transformation continuously at 0.8% change per frame

🤘 Rock Sign: Y-Axis continuous inspection rotation (0.04 rad/frame)

👍 Thumbs Up: Interactive Parameter Lock/Unlock state (protects nodes from accidental moves/deletions)

2. 🎤 Natural Language Processing (Web Speech API)
Control your environment flawlessly using continuous audio processing commands:

Creation Pipeline: "Create Cube", "Spawn Sphere", "Create Torus", or "Create Pyramid"

Modification Matrix: "Delete Selected Object", "Duplicate Object", or "Lock/Unlock"

Material Shifting: "Apply Glass Material", "Make it Metal", "Neon", or "Apply Chrome"

Color Injection: "Change Color to Cyan", "Magenta", "Green", or "Amber"

State Control: "Enable Physics", "Disable Gravity", "Clear Scene", or "Save Scene"

3. 🧪 Advanced Rendering & Physics Engine
Material Presentation Matrix:

✨ Holographic - Translucent edges with a 40% emissive shimmer tint effect.

🪟 Glass - Low roughness, high-performance refraction and transmission optics.

🔩 Metal - Highly reflective, shiny polished element with 95% surface specular gloss.

💡 Neon - Bright self-illuminating shader boasting 120% emissive highlight rendering.

🪵 Wood / 🔵 Plastic / 🪞 Chrome / ⬛ Carbon - Diverse procedural and composite texturing.

Custom Kinematic Physics Sandbox: Toggle an active downward gravity grid field. Objects bounce off an implicit virtual floor layer with a structural 40% restitution value and 12% friction reductions, alongside elastic sphere-to-sphere target bounds collisions.

🛠️ Project Tech Architecture
The architecture utilizes zero-dependency modular loading wrappers to minimize bundle friction:





[ Browser Event Thread ] ──> [ Web Speech API Engine ] ──> UI Notification Toast State
                                      │
[ Webcam Input Frame ]  ──> [ MediaPipe Pipeline ]     ──> Gestures Extraction HUD
                                      │
                                      ▼
[ WebGL Render Canvas ] <── [ Three.js Renderer Core ]  <── [ Custom Physics Matrix ]







🤖 Built with AI Collaboration
This system was ideated, structured, and implemented with extensive algorithmic pair-programming aid:

AI Core Engine: Powered by Claude Sonnet 4.6

Role: Architectural design patterns, MediaPipe multi-dimensional landmark isolation parsing, optimization matrices, and documentation formulation.

📈 Roadmap / Engineering Enhancements
The current architecture is solid, and I am looking to patch several algorithmic areas to improve processing speeds:

🎯 Hand-Object Coordination: Refining structural landmark proximity checks to eliminate minor translation drift during fast grab sequences.

⚡ Gesture Detection Velocity: Shifting standard debouncing frames parameters into adaptive micro-timed intervals to accelerate action recognition.

🗣️ Voice Pipeline Operations: Injecting dynamic phrase matching patterns to reduce ambient background audio interference inside noisy environments.

⚙️ Advanced Physics Libraries: Transitioning from simple geometric sphere-sphere bounding box approximations to a rigid body integration framework.

🤝 Open for Contributions!
Contributions make the developer ecosystem thrive! If you'd like to help improve tracking mechanics, enhance shaders, or rewrite algorithmic logic, your support is incredibly welcome.

Fork the Project Repo

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Refactored changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a well-documented Pull Request



⚠️ Disclaimer
This repository represents a pure educational, foundational research, and personal practice project. * It is not affiliated, allocated to, endorsed by, or associated with any formal corporate entity, professional organization, university, or brand.

All implementations are completed out of personal interest toward spatial engineering and real-time interaction models.

The codebase is presented "as-is" for personal portfolio presentation and review under open-source educational terms. No liabilities are assumed, and no infringement or problematic application is intended.











