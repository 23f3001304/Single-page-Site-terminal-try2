# HEMANG :: Web3 Dossier

## Summary

This project is an interactive, single-page web application that reimagines the personal resume as a Web3-grade, avant-garde command center. It fuses the discipline of Swiss design—emphasizing grid, hierarchy, and refined typography—with the high-energy artistry of GPU shaders and generative visuals.

The experience is entirely command-driven and full-screen, designed to feel like a living dossier. The interface is built on a foundation of crystalline grid lines, asymmetric layouts, and glassmorphism, all enhanced with holographic textures, volumetric light, and particle systems.

Powered by a stack of **three.js** for the WebGL rendering engine, **GSAP** for complex timeline choreography, and **anime.js** for precise micro-interactions, the application delivers a polished and immersive narrative experience. Key features include an interactive WebGL portrait that reacts to user input, a robust theme engine, and dynamically streamed output that presents resume data as futuristic, neon-accented log cards.

---

## Setup

This is a static web application with no build process required. All dependencies are included or sourced directly.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/23f3001304/Single-page-Site-terminal-try2.git
    ```

2.  **Navigate to the directory:**
    ```bash
    cd Single-page-Site-terminal-try2
    ```

3.  **Open the application:**
    Simply open the `index.html` file in a modern, WebGL-compatible web browser (e.g., Chrome, Firefox, Safari, Edge).

---

## Usage

Interact with the application by typing commands into the terminal. Type `help` to see a list of available commands at any time.

### Core Commands

| Command             | Description                                                                                             |
| ------------------- | ------------------------------------------------------------------------------------------------------- |
| `help`              | Displays a list of all available commands and their functions.                                          |
| `clear`             | Clears all output from the terminal screen.                                                             |
| `whoami`            | Displays a brief biography, education, and professional headline.                                       |
| `mantra`            | Shows the personal mantra or mission statement.                                                         |
| `theme [name]`      | Cycles through visual themes: `neon` (default), `monochrome`, `dusk`, `noir`. Persists for the session.  |
| `art`               | Toggles the background shader-driven art and particle effects.                                          |
| `download`          | Provides a link to download a traditional PDF version of the resume.                                    |

### Resume & Profile Commands

| Command           | Description                                                                                               |
| ----------------- | --------------------------------------------------------------------------------------------------------- |
| `experience`      | Details professional and research experience, including work at DRDO (GANxART).                           |
| `timeline`        | Provides a chronological overview of key career and academic milestones.                                  |
| `skills`          | Lists key technical and research skills (e.g., Research Skills, GaN, MERN Stack, Python).                   |
| `projects`        | Showcases selected projects with descriptions, rendered as interactive holographic cards.                   |
| `certifications`  | Displays a list of earned certifications (e.g., AWS, SQL, Java, Full Stack).                              |
| `publications`    | Lists published articles and works, such as "Crushader Issue 1".                                          |
| `achievements`    | Highlights significant accomplishments and awards.                                                        |
| `languages`       | Lists spoken languages and proficiency levels (Hindi: Native/Bilingual, English: Professional Working).   |
| `socials`         | Provides links to social and professional profiles, including LinkedIn.                                   |
| `contact`         | Displays contact information, including the email `coehemang@gmail.com`.                                    |
| `references`      | Information on how to request professional references.                                                    |
| `availability`    | Shows current professional availability status.                                                           |

---

## Code Explanation

The architecture is designed to be a cohesive system where visual artistry, interaction, and data presentation are tightly integrated.

### Rendering Engine & Visuals (three.js)

The core of the experience is a `three.js` scene that renders all visual elements.
-   **Interactive Portrait:** The central profile photo is transformed into a live WebGL texture. It is layered with custom shaders to create effects like scanlines, caustics, glitch sweeps, and refractions that react to cursor movement and audio cues. An SVG/CSS fallback is provided for non-WebGL environments.
-   **Reactive Scene:** The background is not static. It features a stack of reactive textures, including refractive glass panels, noise-driven displacement maps, and shader-based overlays that respond to commands and user interaction, creating a sense of a living environment.
-   **Particle Systems:** Subtle particle swarms and data rain effects drift through the scene, enhancing the Web3 aesthetic and responding to system states (e.g., loading, command success).

### Animation & Choreography (GSAP / anime.js)

Motion is a key part of the experience, designed to be expressive yet controlled.
-   **GSAP (GreenSock Animation Platform):** Used for orchestrating major, complex animations. This includes scene transitions, the choreographed streaming of terminal output cards, and camera movements.
-   **anime.js:** Handles high-performance, lightweight micro-interactions. This includes kinetic typography effects on text reveal, liquid transitions for UI elements, and pulse-driven highlights on hover/focus states.
-   **`prefers-reduced-motion`:** All animations respect the user's OS-level accessibility settings. If reduced motion is enabled, non-essential, decorative animations are disabled while crucial UI feedback remains.

### UI & Command System

The user interface is built directly into the WebGL scene and the HTML DOM.
-   **Command Parser:** A simple input parser listens for commands, validates them, and triggers the corresponding data-fetching and rendering sequence.
-   **Futuristic Log Cards:** Command output is not simple text. Each response is rendered as a "log card"—a DOM element styled with glassmorphism, neon gradients, and subtle depth. These cards are animated into view using GSAP, appearing to stream from a data source.
-   **Swiss Design Grid:** Despite the complex visuals, the layout of all UI elements adheres to a strict Swiss grid system, ensuring rhythm, hierarchy, and legibility are maintained.

### Theming & State

-   **Theme Command:** The `theme` command dynamically updates CSS custom properties and swaps materials and uniforms in the `three.js` shaders. This allows for a complete visual overhaul (e.g., `neon` to `monochrome`) without glitches or page reloads. The user's choice is saved in `sessionStorage` to persist across the session.
-   **Stateful Feedback:** The application provides rich, stateful feedback using integrated audio cues for loading pulses, success tones, and error flashes, enhancing the command-center feel.

---

## License

This project is licensed under the MIT License.

Copyright (c) 2024 Hemang

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.