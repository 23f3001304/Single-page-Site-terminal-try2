```markdown
# Terminal Resume

A personal portfolio website that looks and feels like a real terminal. This project is built with vanilla HTML, CSS, and JavaScript, designed to be lightweight, fast, and fully responsive.

## Summary

This interactive terminal serves as a unique resume and portfolio. The core experience of the original terminal—including its layout, typography, animations, and command registry—has been perfectly preserved.

This update introduces several new, non-intrusive features:

-   **Expanded Theming**: Two new color palettes, "Aurora Drift" and "Mono Noir," have been added to the `theme` command, available alongside the original default theme.
-   **ASCII Art**: A new `ascii_mood` command renders a friendly, monospaced ASCII portrait directly in the terminal, respecting the current theme and accessibility settings.
-   **Mini-Games**: Two lightweight, in-terminal games, `type-racer` and `asteroid-dodge`, are now available for a bit of fun. They run entirely within the command output area without altering the site's layout.

All original commands and functionality remain untouched, ensuring zero regression.

## Setup

To get a local copy up and running, follow these simple steps. No complex build tools are required.

1.  Clone the repository:
    ```sh
    git clone https://github.com/your-username/terminal-resume.git
    ```
2.  Navigate to the project directory:
    ```sh
    cd terminal-resume
    ```
3.  Open the `index.html` file in your preferred web browser.

## Usage

Type `help` at any time to see a list of available commands.

### Standard Commands

These are the original commands, which continue to function as before.

-   `about`     - Displays a short bio.
-   `skills`    - Lists technical skills and proficiencies.
-   `projects`  - Shows a curated list of key projects.
-   `contact`   - Provides contact information and social links.
-   `history`   - Shows a log of previously used commands.
-   `clear`     - Clears all output from the terminal screen.
-   `welcome`   - Displays the welcome banner.

### Enhanced Commands

**`theme`**
Changes the terminal's color scheme. The original default theme is preserved and remains the initial experience.

*Usage:*
```bash
# List available themes
theme

# Set a new theme
theme set <theme_name>
```

*Available themes:*
-   `default` (The original theme)
-   `aurora-drift`
-   `mono-noir`

### New Feature Commands

**`ascii_mood`**
Renders a friendly ASCII art portrait inside the terminal. The output respects the terminal's grid, current color theme, and the user's `prefers-reduced-motion` setting.

*Usage:*
```bash
ascii_mood
```

**`type-racer`**
Launches a timed typing challenge. A random text snippet will appear, and your goal is to type it as quickly and accurately as possible.

*Usage:*
```bash
type-racer
```
> Press `Esc` or `Ctrl+C` to exit the game at any time.

**`asteroid-dodge`**
Starts a simple cursor-controlled mini-game. Use your arrow keys to navigate and dodge the incoming asteroids.

*Usage:*
```bash
asteroid-dodge
```
> Press `Esc` or `Ctrl+C` to exit the game at any time.

## Code Explanation

The application is built with vanilla JavaScript, HTML, and CSS, with a focus on simplicity and performance.

-   **Command Bus**: A central command registry (a simple JavaScript object) maps input strings to corresponding functions. New features like `ascii_mood` and the mini-games are added as new entries to this registry without modifying the core command-handling logic.
-   **Theming Engine**: Themes are managed using CSS variables defined on the `:root` element. The `theme set <name>` command dynamically updates these variables to apply the new color palette instantly. The new themes are self-contained sets of these variables.
-   **Component Re-use**: All new features render their output into the existing terminal history component. This approach prevents any layout shifts or DOM rearrangements, as the new content is simply appended to the output log just like the response from any original command.
-   **Self-Contained Games**: The `type-racer` and `asteroid-dodge` games are designed to be entirely self-contained. Their logic, event listeners (for keyboard input), and render loops are initialized on start and completely torn down on exit, ensuring they do not interfere with the terminal's primary functionality.

## License

This project is distributed under the MIT License. See the `LICENSE.txt` file for more information.

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