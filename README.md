# just a chill human :: terminal

A sleek, interactive terminal-style website designed for a chill, human experience. This project provides a classic command-line interface on a static web page, now enhanced with multiple themes, ASCII art generation, and simple terminal-based games.


![Project Screenshot](https://user-images.githubusercontent.com/83253033/154887309-844a4b2a-0a0e-4735-a681-37f075b058c4.png)

*(Image is a placeholder and should be updated with a current screenshot)*

## Summary

This is a single-page, static web application that simulates a terminal interface. It's built with vanilla HTML, CSS, and JavaScript, making it lightweight and easy to customize. The latest update focuses on expanding user interaction and aesthetic appeal.

**New Features:**
*   **Multiple Themes:** Switch between various color schemes to suit your mood.
*   **ASCII Art Generator:** Create fun ASCII art from any text using the `ascii` command.
*   **Terminal Games:** Kill some time with simple, built-in text-based games.

## Setup

No complex build process is required. Since this is a static site, you can run it locally or deploy it to any static web host.

To run locally:
1.  Clone the repository:
    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd your-repository-name
    ```
3.  Open the `index.html` file in your favorite web browser.

## Usage

Interact with the website by typing commands into the terminal prompt. Type `help` to see a list of all available commands.

### Available Commands

| Command         | Description                                                                 | Usage Example                |
| --------------- | --------------------------------------------------------------------------- | ---------------------------- |
| `help`          | Displays a list of all available commands.                                  | `help`                       |
| `about`         | Shows a brief summary about me.                                             | `about`                      |
| `projects`      | Lists my recent projects with links.                                        | `projects`                   |
| `social`        | Provides links to my social media profiles.                                 | `social`                     |
| `theme`         | Lists available themes or sets a new one.                                   | `theme` or `theme matrix`    |
| `ascii`         | Generates ASCII art from the provided text.                                 | `ascii hello world`          |
| `game`          | Starts a mini-game. Use `game list` to see options.                         | `game snake`                 |
| `clear`         | Clears all output from the terminal screen.                                 | `clear`                      |
| `welcome`       | Displays the welcome banner again.                                          | `welcome`                    |

## Code Explanation

The project is structured for simplicity and easy customization. All core logic resides in three main files:

*   **`index.html`**: The main HTML file that provides the structure for the terminal. The core element is the `<div id="terminal">`.
*   **`style.css`**: Contains all styling, including the layout, animations, and color schemes for themes. New themes can be added by creating a new CSS class (e.g., `.theme-solarized`) and defining the color variables.
*   **`script.js`**: The heart of the application. This file handles:
    *   Command parsing and execution.
    *   DOM manipulation to display output.
    *   Theme switching logic.
    *   The implementation for the ASCII generator and games.

To customize the content (like adding new projects or social links), simply modify the corresponding data structures within `script.js`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Copyright (c) 2025 [Your Name]