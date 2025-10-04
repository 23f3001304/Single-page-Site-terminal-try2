```markdown
# Holographic Dossier: A WebGL Terminal Résumé


![Project Banner](https://i.ibb.co/jZxwXR2Y/1759419391197.png)


## Summary

This project is a complete architectural overhaul of a static web application into a web3-grade, holographic résumé. It presents a single-page, command-driven experience that fuses the discipline of Swiss design with high-energy shader artistry. The interface is an avant-garde command center, featuring crystalline grid lines, asymmetric layouts, and refined typography, all bathed in holographic textures, volumetric light, and glassmorphism.

The core interaction model is a full-screen terminal where user commands stream futuristic log cards containing résumé information. These elements are choreographed with sophisticated motion states using GSAP and anime.js, while the immersive environment is rendered with three.js, featuring reactive texture stacks, refractive panels, and particle systems that respond to user input. The experience is designed to be a "living dossier," offering a narrative journey through a professional's identity and skills, while adhering to strict accessibility and performance standards.

## Setup

To run this project locally, ensure you have [Node.js](https://nodejs.org/) and [npm](https://www.npmjs.com/) installed.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    ```

2.  **Install dependencies:**
    The project is self-contained with dependencies managed via npm.
    ```bash
    npm install
    ```

3.  **Run the development server:**
    This command will start a local server and open the application in your default browser.
    ```bash
    npm run dev
    ```

## Usage

The entire experience is navigated through the command-line interface. Type a command and press `Enter` to execute. For a list of all available commands, type `help`.

### Available Commands

| Command         | Description                                                                 |
| --------------- | --------------------------------------------------------------------------- |
| `help`          | Displays a list of all available commands and their descriptions.           |
| `whoami`        | Prints a brief biography and professional headline.                         |
| `mantra`        | Displays a personal or professional mantra.                                 |
| `timeline`      | Shows a chronological overview of education and experience.                 |
| `experience`    | Details professional and research experience, including work at DRDO.       |
| `skills`        | Lists core technical competencies and areas of expertise.                   |
| `projects`      | Showcases featured projects as interactive, holographic cards.              |
| `certifications`| Displays a list of completed certifications and qualifications.             |
| `publications`  | Lists published works and articles.                                         |
| `languages`     | Shows proficiency in spoken and written languages.                          |
| `achievements`  | Highlights key accomplishments and awards.                                  |
| `references`    | Provides information on how to request professional references.             |
| `socials`       | Displays links to social and professional networks like LinkedIn.           |
| `contact`       | Shows contact information, including email.                                 |
| `availability`  | Displays current professional availability for new opportunities.           |
| `download`      | Provides a link to download a traditional PDF version of the résumé.        |
| `theme`         | Cycles through curated visual themes: `neon`, `swiss`, `dusk`, `noir`.      |
| `art`           | Toggles the hero banner ASCII art or other visual flourishes.               |
| `clear`         | Clears all output from the terminal screen.                                 |

## Code Explanation

This project is architected with a modern JavaScript stack, focusing on modularity, performance, and visual fidelity.

*   **Rendering Engine (`three.js`)**: The core of the visual experience. Three.js is used to create the 3D scene, manage the WebGL renderer, and implement all shader-based materials. This includes the reactive background grid, volumetric light effects, glassmorphic panels, and the interactive WebGL portrait with its caustics, scanlines, and particle halos.

*   **Animation & Choreography**:
    *   **GSAP (GreenSock Animation Platform)**: Used for complex, timeline-based choreographies. This includes the sequenced appearance of command outputs ("log cards") and major scene transitions, ensuring a fluid narrative flow.
    *   **anime.js**: Employed for micro-interactions and stateful feedback. This powers kinetic typography, liquid UI transitions, subtle parallax effects on text, and pulse-driven highlights on focus or hover.

*   **State Management & Data**: All résumé content is centralized in a single JavaScript object (`data/resume.js`). This makes updating information straightforward without needing to touch the application's logic. Session state, such as the selected theme, is managed in-memory and persisted for the user's session.

*   **UI & Command Logic (`main.js`)**: The primary application logic resides here. It handles user input from the terminal, parses commands, retrieves the corresponding data, and orchestrates the rendering of the output cards onto the screen. It also integrates with the animation and WebGL modules to trigger visual and audio feedback.

*   **Accessibility**: A high priority. The application respects the `prefers-reduced-motion` media query to disable non-essential animations. The interface is fully keyboard-navigable, and ARIA attributes are used to ensure it is screen-reader compatible. All themes are designed to meet high-contrast standards.

## License

This project is licensed under the MIT License.

```
MIT License

Copyright (c) 2024 [Your Name]

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
```
```