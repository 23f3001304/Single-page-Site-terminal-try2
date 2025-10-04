# Interactive Terminal Resume

This project is a static web application that presents a personal resume and portfolio within a fully interactive, retro-style terminal interface.

The core experience of the original terminal resume is perfectly preserved, including its layout, typography, command registry, and default theme. This update layers new functionality on top without any regressions. Enhancements include an expanded theme system, an ASCII art display command, and two embedded mini-games, all designed to integrate seamlessly into the existing terminal environment.

## Summary

An interactive and gamified personal portfolio website designed to look and feel like a terminal. It is a single-page application built with React, featuring a command-line interface where users can explore a professional profile, view projects, change themes, and play embedded games.

## Setup and Installation

To get a local copy up and running, follow these simple steps.

### Prerequisites

-   Node.js (v14 or later)
-   npm or yarn

### Installation

1.  Clone the repository:
    ```sh
    git clone https://github.com/your-username/terminal-resume.git
    ```
2.  Navigate to the project directory:
    ```sh
    cd terminal-resume
    ```
3.  Install NPM packages:
    ```sh
    npm install
    ```
4.  Run the application in development mode:
    ```sh
    npm start
    ```
    Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

## Usage and Commands

Interact with the application by typing any of the commands below and pressing `Enter`. Use the `help` command at any time to see the list of available commands.

| Command         | Description                                                                                                                                                                                                |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `help`          | Lists all available commands and their descriptions.                                                                                                                                                       |
| `about`         | Displays a brief professional summary.                                                                                                                                                                     |
| `resume`        | Provides a link to the downloadable PDF version of the resume.                                                                                                                                             |
| `projects`      | Shows a list of featured projects with descriptions and links to live demos and source code.                                                                                                               |
| `contact`       | Displays contact information, including email and links to social profiles like LinkedIn and GitHub.                                                                                                       |
| `theme`         | Changes the terminal's color palette. The original `default` theme remains the first-load experience. Usage: `theme set <themename>`.<br>**Themes:** `default`, `aurora-drift`, `mono-noir`.                  |
| `ascii_mood`    | **(New)** Renders a friendly, chill-human portrait in monospaced ASCII art. The art respects the terminal's grid, color theme, and the user's `prefers-reduced-motion` accessibility setting.                 |
| `type-racer`    | **(New)** Starts a lightweight, timed typing challenge. Test your speed using the application's native typography. On-screen instructions are provided. Press `ESC` at any time to quit.                     |
| `asteroid-dodge`| **(New)** Launches a simple, cursor-controlled avoidance mini-game rendered in the command output area. Use your mouse or trackpad to navigate. Press `ESC` at any time to exit.                             |
| `clear`         | Clears all previous output from the terminal screen.                                                                                                                                                       |

## Code Explanation

This application is built with modern web technologies, focusing on a lightweight footprint and a clean, component-based architecture.

### Tech Stack

-   **React.js:** For building the dynamic and responsive user interface.
-   **Styled-Components:** For component-level CSS styling and the dynamic theming system.
-   **TypeScript:** For static typing to improve code quality and maintainability.

### Development Principles

-   **Zero Regression:** All enhancements were layered on top of the existing application without altering, restyling, or removing any original functionality. Core commands, animations, and data behave identically to the baseline version.
-   **Component Reuse:** New features like the mini-games and ASCII art viewer are self-contained components that render within the existing command output area. This approach prevents any disruptive DOM rearrangements and maintains a clean separation of concerns.

## License

This project is distributed under the MIT License. See `LICENSE.txt` for more information.

```text
MIT License

Copyright (c) 2024

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