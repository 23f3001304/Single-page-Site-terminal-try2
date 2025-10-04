# ./portfolio.sh

## Summary

This project is a personal portfolio reimagined as an interactive, command-line interface. The site is a single-page static web application designed to feel like a retro-futuristic terminal. It provides a unique and engaging way to explore my professional background, projects, and skills.

The application is built with a focus on aesthetics and user experience, featuring multiple themes, ASCII art generation, and even small terminal-based games. The interface is clean, responsive, and fully interactive, allowing users to navigate the portfolio using a set of simple commands.

## Setup

This is a static web application and requires no special setup or build process.

1.  **Clone the repository:**
    
```bash
    git clone https://github.com/23f3001304/Single-page-Site-terminal-try2.git
    ```


2.  **Navigate to the project directory:**
    
```bash
    cd Single-page-Site-terminal-try2
    ```


3.  **Open in your browser:**
    Simply open the `index.html` file in your favorite web browser.

## Usage

Interact with the application by typing commands into the terminal. For a list of available commands, type `help`.

### Core Commands

| Command | Description |
| --- | --- |
| `help` | Displays a list of all available commands. |
| `clear` | Clears all output from the terminal screen. |
| `whoami` | Displays a brief biography and professional summary. |
| `socials` | Lists links to my social and professional profiles. |
| `projects`| Showcases a selection of my projects with descriptions. |
| `skills` | Lists my technical skills. |
| `contact` | Shows my contact information. |
| `theme [name]`| Switches the visual theme of the terminal. Available themes include `default`, `light`, `matrix`, and `gruvbox`. |
| `ascii [text]`| Generates ASCII art from the provided text. |
| `play [game]`| Starts a mini-game. Available games: `snake`, `tetris`. |

## Code Explanation

The application is a vanilla HTML, CSS, and JavaScript project, with a focus on simplicity and performance.

*   **HTML (`index.html`):** The main structure of the application is a single HTML file. The terminal interface is built with simple HTML elements, and the output is dynamically generated and appended to the DOM.

*   **CSS (`style.css`):** The styling is done with CSS, using custom properties for theming. This allows for easy switching of color schemes and fonts by updating the CSS variables. The new themes are implemented as additional color palettes that can be applied by changing a class on the `body` element.

*   **JavaScript (`main.js`):** The core logic of the application is in the JavaScript file. It handles user input, command parsing, and generating the corresponding output.
    *   **Command Parser:** A simple `switch` statement or a command map object is used to handle the different commands entered by the user.
    *   **ASCII Art:** The `ascii` command uses a simple JavaScript library or a custom function to convert text into ASCII art, which is then displayed in the terminal.
    *   **Games:** The terminal games are implemented as self-contained JavaScript modules that handle the game logic, rendering, and user input within the terminal interface.

## License

This project is licensed under the MIT License.

Copyright (c) 2024 Hemang

The
 MIT License (MIT)

Copyright
 (c) 2024 Hemang

<
p>Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:</p>

<p>The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.</p>

<p>THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.</p>