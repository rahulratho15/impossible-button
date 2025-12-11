# The Impossible Button

![Game Status](https://img.shields.io/badge/Status-Playable-brightgreen)
![Tech Stack](https://img.shields.io/badge/Tech-HTML%20%7C%20CSS%20%7C%20JS-blue)
![License](https://img.shields.io/badge/License-MIT-orange)

> **Can you survive?** A fast-paced, retro-styled reflex game that tests your cognitive processing speed and accuracy.

## 🎮 Play Now

Try the live version directly in your browser:
**[👉 Play The Impossible Button](https://rahulratho15.github.io/impossible-button/)**

---

## 📖 About The Project

**The Impossible Button** is a web-based reaction game inspired by "WarioWare" and classic "Simon Says" mechanics, wrapped in a nostalgic VT323 terminal/CRT aesthetic. Players must follow rapidly changing instructions within a shrinking time limit.

The project is built entirely with **Vanilla JavaScript**, demonstrating how complex game logic, audio synthesis, and visual effects can be achieved without external game engines or heavy frameworks.

### Key Features

*   **10 Progressive Levels:** Difficulty scales with faster timers and complex task combinations.
*   **Dynamic Task System:** Includes logic puzzles, button mashing, holding mechanics, and visual recognition.
*   **Retro Aesthetic:** Custom CSS animations for CRT scanlines, glitch effects, and screen shake.
*   **Synthesized Audio:** Uses the Web Audio API to generate sound effects programmatically (no external audio files required).
*   **Responsive Design:** Fully playable on both desktop and mobile devices with touch support.

---

## 🕹️ How to Play

The game presents a series of commands. You must interact with the central button based on the instruction before the timer ring runs out.

| Command | Action Required |
| :--- | :--- |
| **PRESS** | Click the button exactly **once**. |
| **DO NOT PRESS** | Do nothing until the timer runs out. |
| **MATH (e.g., "2 + 3")** | Calculate the answer and click the button that many times (e.g., click 5 times). |
| **SPAM** | Click the button as fast as possible to fill the quota. |
| **HOLD** | Click and hold the button down until the timer completes. |
| **PRESS IF RAT** | A visual recognition task. Click only if the text describes a rat. |

**Game Over Conditions:**
*   Running out of time.
*   Clicking when you shouldn't.
*   Clicking the wrong amount of times (Math/Spam).
*   Releasing too early (Hold).

---

## 🛠️ Tech Stack

This project is a lightweight, single-file application structure.

*   **HTML5:** Semantic structure and SVG graphics for the timer ring.
*   **CSS3:** Advanced animations (`@keyframes`), flexbox layout, and responsive media queries.
*   **JavaScript (ES6+):**
    *   `AudioContext` for real-time sound generation.
    *   Game loop management and state tracking.
    *   DOM manipulation for UI updates.

---

## 🚀 Getting Started

Since this project uses standard web technologies with no build steps, running it locally is incredibly simple.

### Prerequisites
*   A modern web browser (Chrome, Firefox, Safari, Edge).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/rahulratho15/impossible-button.git
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd impossible-button
    ```

3.  **Run the game:**
    *   Simply double-click `index.html` to open it in your browser.
    *   *Optional:* For a better experience (to avoid CORS issues if you expand the code later), use a simple local server:
        ```bash
        # Python 3
        python -m http.server 8000
        ```
        Then visit `http://localhost:8000` in your browser.

---

## 📂 Project Structure

The project is contained primarily within `index.html` for portability, but logically structured as follows:

```text
impossible-button/
├── README.md           # Project documentation
└── index.html          # Core game file
    ├── <style>         # CSS: Glitch effects, layout, animations
    ├── <body>          # HTML: Game container, UI overlays, SVG elements
    └── <script>        # JS: Game Logic
        ├── AudioSystem # Web Audio API wrapper
        ├── Game        # Main state machine (Level config, Task definitions)
        └── Event Listeners
```

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<div align="center">
  <p>Created by <a href="https://github.com/rahulratho15">rahulratho15</a></p>
</div>