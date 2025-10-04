# HEMANG :: A Terminal-Based Interactive Resume

## Summary

This project is an interactive, single-page web application that reimagines a personal resume as a terminal command center. It blends a clean, minimalist design with a touch of retro terminal aesthetics, offering an engaging and unique way to explore professional information.

The experience is entirely command-driven. The interface is designed to be simple and intuitive, focusing on a straightforward command-line experience. It now includes multiple themes, ASCII art, and simple text-based games to enhance user engagement.

Powered by a lightweight stack of HTML, CSS, and vanilla JavaScript, the application is fast, responsive, and easy to modify.

---

## Setup

This is a static web application with no build process required.

1.  **Clone the repository:**
    
```bash
    git clone https://github.com/23f3001304/Single-page-Site-terminal-try2.git
    ```


2.  **Navigate to the directory:**
    
```bash
    cd Single-page-Site-terminal-try2
    ```


3.  **Open the application:**
    Simply open the `index.html` file in any modern web browser.

---

## Usage

Interact with the application by typing commands into the terminal. Type `help` to see a list of available commands.

### Core Commands

| Command             | Description                                                                                             |
| ------------------- | ------------------------------------------------------------------------------------------------------- |
| `help`              | Displays a list of all available commands.                                          |
| `clear`             | Clears all output from the terminal screen.                                                             |
| `whoami`            | Displays a brief biography.                                       |
| `socials`         | Provides links to social and professional profiles.                                   |
| `contact`         | Displays contact information.                                    |
| `theme [name]`      | Cycles through visual themes.                                                                            |
| `art`               | Displays an ASCII art piece with the text "just a chill human".                                         |
| `games`             | Lists available mini-games to play in the terminal.                                                     |
| `download`          | Provides a link to download a PDF version of the resume.                                    |

### Resume Commands

| Command           | Description                                                                                               |
| ----------------- | --------------------------------------------------------------------------------------------------------- |
| `experience`      | Details professional and research experience.                           |
| `skills`          | Lists key technical and research skills.                   |
| `projects`        | Showcases selected projects with descriptions.                   |
| `education`       | Displays educational background.                                                                        |
| `achievements`    | Highlights significant accomplishments and awards.                                                        |

---

## Code Explanation

The application is built with simplicity and extensibility in mind, using only vanilla HTML, CSS, and JavaScript.

*   **`index.html`**: The main entry point of the application. It contains the basic structure of the terminal interface.
*   **`style.css`**: This file contains all the styling for the application, including the different color themes for the terminal.
*   **`script.js`**: This is the core of the application. It handles the command parsing, executes the corresponding functions, and displays the output in the terminal. The new features such as ASCII art and games are implemented here.

### Key Features

*   **Command Parser**: A simple function that takes user input, splits it into a command and arguments, and calls the appropriate function.
*   **Theming**: The `theme` command dynamically updates CSS variables to change the colors of the terminal.
*   **ASCII Art**: The `art` command prints a pre-defined ASCII art string to the terminal.
*   **Terminal Games**: The `games` command introduces a simple game loop, allowing for interactive text-based games within the terminal.

---

## License

This project is licensed under the MIT License.

Copyright (c) 2024 Hemang

This
 project is licensed under the terms of the MIT license. Please see the `LICENSE` file for full details.