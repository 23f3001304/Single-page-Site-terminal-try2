```markdown
# Hemang :: Web3 Dossier

[
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
](https://opensource.org/licenses/MIT)

An avant-garde, command-driven resume experience that fuses the discipline of Swiss design with the high-energy artistry of WebGL shaders. This single-page application functions as a living dossier, presenting a professional profile within an interactive, full-screen terminal.

The interface is built on a foundation of crystalline grid lines, asymmetric layouts, and refined typography, drenched in holographic textures, volumetric light, and glassmorphism. It's a meticulously crafted world that feels both mathematically precise and artistically outrageous.

[View Live Demo](https://coehemang.github.io/)


![Live Demo Screenshot](https://i.ibb.co/L5QG2F3/image.png)


## Summary

This project is an architectural push to sculpt a resume that transcends traditional formats. It leverages `three.js` for a reactive WebGL environment, `GSAP` for sophisticated timeline choreography, and `anime.js` for precise micro-interactions. The goal is a seamless narrative arc—from an identity mantra to deep-dives into skills and projects—all navigated through a futuristic command-line interface.

Every element, from the kinetic typography to the shader-driven WebGL portrait, is designed to be responsive, accessible, and respectful of user preferences like `prefers-reduced-motion`.

## Setup

This is a static web application with no server-side dependencies. To run it locally:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd your-repository-name
    ```

3.  **Open the application:**
    Simply open the `index.html` file in a modern web browser. For the best experience and to avoid potential CORS issues with asset loading, it's recommended to use a local development server.

    *   **Using VS Code's Live Server:** Right-click `index.html` and select "Open with Live Server".
    *   **Using Python:**
        ```bash
        # For Python 3
        python -m http.server

        # For Python 2
        python -m SimpleHTTPServer
        ```

## Usage

Interact with the application by typing commands into the terminal prompt. All commands stream their output as futuristic log cards that animate onto the screen. Type `help` to see a list of available commands at any time.

### Available Commands

| Command         | Description                                                               | Arguments                  |
| --------------- | ------------------------------------------------------------------------- | -------------------------- |
| **CORE**        |                                                                           |                            |
| `help`          | Displays this list of all available commands.                             | -                          |
| `clear`         | Clears all output from the terminal screen.                               | -                          |
| `mantra`        | Displays the core philosophy and approach.                                | -                          |
| `whoami`        | Prints a detailed biography and professional headline.                    | -                          |
| `socials`       | Lists all social and professional network links.                          | -                          |
| **PROFESSIONAL**|                                                                           |                            |
| `experience`    | Details professional work and research experience.                        | -                          |
| `timeline`      | Shows a chronological overview of education and career milestones.        | -                          |
| `skills`        | Lists key technical and research skills.                                  | -                          |
| `projects`      | Displays a showcase of selected projects as holographic cards.            | -                          |
| `certifications`| Lists all professional certifications.                                    | -                          |
| `publications`  | Shows a list of published works.                                          | -                          |
| `achievements`  | Highlights significant accomplishments.                                   | -                          |
| **UTILITY**     |                                                                           |                            |
| `languages`     | Lists spoken and written languages and proficiency levels.                | -                          |
| `contact`       | Displays contact information.                                             | -                          |
| `availability`  | Shows current professional availability.                                  | -                          |
| `references`    | Information on how to request professional references.                    | -                          |
| `download`      | Provides a link to download the resume in PDF format.                     | -                          |
| `theme`         | Cycles through visual themes or sets a specific one.                      | `neon`, `mono`, `dusk`, `noir` |
| `art`           | Toggles post-processing effects and decorative shaders.                   | -                          |

**Example:**
To change the visual style to the monochrome Swiss palette, type:
`theme mono`

## Code Explanation

The application's architecture is designed to be modular and performant, centered around three core pillars: rendering, animation, and interactivity.

### Rendering Engine (Three.js)

The immersive background and interactive elements are powered by a `three.js` WebGL scene. This is not a static video or image; it's a live, generative environment.
*   **Reactive Textures:** The scene uses a stack of textures and shaders to create effects like refractive glass panels, noise-driven displacement, and iridescent overlays that respond to cursor movement and command context.
*   **WebGL Portrait:** The profile photo is transformed into an interactive WebGL object. It features layered scanlines, caustics, glitch sweeps, and a reactive particle halo that breathes with the application's state. A fallback CSS/SVG version ensures compatibility.
*   **Theming:** The `theme` command directly updates shader uniforms, material properties, and scene lighting in real-time to transition between palettes like `neon` and `monochrome Swiss` without visual glitches.

### Motion System (GSAP & anime.js)

Motion is central to the experience, designed to be both expressive and controlled.
*   **GSAP (GreenSock Animation Platform):** Used for complex, timeline-based choreographies. This includes the sequenced reveal of command output cards, full-screen transitions, and major state changes that require precise synchronization.
*   **anime.js:** Powers the micro-interactions. This library is used for its lightweight and performant handling of kinetic typography, liquid-like hover effects, pulse-driven UI highlights, and other subtle movements that enhance user feedback.
*   **Accessibility:** All motion respects the `prefers-reduced-motion` media query. When enabled, dramatic animations are disabled or replaced with simple, elegant cross-fades.

### Command & State Management

A central JavaScript module handles all user input and application state.
*   **Command Parser:** A simple but effective parser reads user input, identifies valid commands and arguments, and triggers the corresponding function.
*   **Output Stream:** Command outputs are dynamically generated as HTML elements and appended to the DOM. GSAP orchestrates their animated entry to create the "streaming log" effect.
*   **Stateful Feedback:** The system integrates audio cues for loading states, success confirmations, and error notifications, enhancing the command-center feel. The user's selected theme is persisted for the duration of the session using `sessionStorage`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for full details.

```