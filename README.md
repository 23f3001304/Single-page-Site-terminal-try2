# Web3 Dossier: Hemang

## Summary

This project is a web3-grade, single-page resume designed as an avant-garde, command-driven terminal. It fuses the discipline of Swiss design with high-energy shader artistry to create an interactive and futuristic experience. The interface uses crystalline grid lines, asymmetric layouts, and refined typography, all enhanced with holographic textures, volumetric light, and glassmorphism.

The application is built with vanilla HTML, CSS, and JavaScript, leveraging powerful libraries for advanced visuals and animations:
-   **three.js**: For sculpting reactive and interactive WebGL texture stacks, including refractive panels and shader-based overlays.
-   **GSAP (GreenSock Animation Platform)**: For timeline choreography and sophisticated motion design.
-   **anime.js**: For fluid micro-interactions and kinetic typography.

The experience is designed to be fully accessible, respecting `prefers-reduced-motion` settings and ensuring keyboard navigability and high-contrast visuals.

## Setup

This is a static web application with all dependencies inlined or sourced directly. No build process is required.

1.  **Clone the repository:**
    
```bash
    git clone https://github.com/your-username/web3-dossier.git
    ```

2.  **Navigate to the project directory:**
    
```bash
    cd web3-dossier
    ```

3.  **Open the application:**
    Open the `index.html` file in your preferred web browser.

## Usage

The interface is entirely command-driven. Type a command into the terminal and press Enter to execute it.

### Available Commands

| Command | Description |
| --- | --- |
| `help` | Displays a list of all available commands. |
| `clear` | Clears the terminal screen. |
| `whoami` | Displays a brief biography and professional headline. |
| `experience` | Details professional and research experience, including work at DRDO. |
| `skills` | Lists top technical and research skills (e.g., Research Skills, GaN). |
| `projects` | Showcases a gallery of projects as interactive holographic cards. |
| `contact` | Provides contact information, including email (`coehemang@gmail.com`). |
| `download` | Provides a link to download the resume data bundle. |
| `theme` | Toggles between neon and monochrome Swiss color palettes. |
| `art` | Toggles artistic shader effects and visualizers. |
| `timeline` | Displays a chronological overview of education and career milestones. |
| `certifications` | Lists all professional certifications. |
| `publications` | Shows published works, such as "Crushader Issue 1". |
| `languages` | Lists spoken languages (Hindi, English). |
| `achievements` | Highlights key achievements and recognitions. |
| `references` | Provides information on how to request references. |
| `availability` | Shows current professional availability status. |
| `socials` | Displays links to social profiles, including LinkedIn. |
| `mantra` | Displays the core identity mantra or mission statement. |

## Code Explanation

The application is architected as a single-page experience driven by a central JavaScript module that handles command parsing, state management, and DOM manipulation.

-   **`index.html`**: The main entry point containing the basic structure, terminal interface, and the WebGL canvas. It also includes links to Google Fonts and script tags for all dependencies.
-   **`style.css`**: Defines the application's visual language. It implements the Swiss grid system for layout, typography, and spacing while incorporating Web3 aesthetics like neon glows, glassmorphism, and emissive grids. It also includes fallback styles for when WebGL is unavailable and accessibility features like high-contrast themes.
-   **`main.js`**: The core application logic. It initializes the terminal, registers command handlers, and manages the output stream. It integrates the following libraries to create the dynamic experience:
    -   **three.js**: Manages the WebGL scene, including the interactive portrait, shader-driven backgrounds, and particle effects that respond to user input and audio cues.
    -   **GSAP**: Used for complex, timeline-based animations, such as the choreographed sequences for command outputs and cinematic transitions.
    -   **anime.js**: Handles smaller, stateful micro-interactions like button pulses, loading indicators, and kinetic typography highlights.
-   **`/assets`**: This directory contains all media, including the interactive profile photo, terminal sound effects, and fonts.

The codebase is documented and designed to be clean, with a focus on respecting accessibility standards like `prefers-reduced-motion`.

## License

This project is licensed under the MIT License.


```
MIT License

Copyright (c) 2025 Hemang

MIT
 License

Copyright (c) 2025 Hemang

<
p>Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:</p>

<p>The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.</p>

<p>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.</p>

```

```