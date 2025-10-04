```
markdown
_
output
 = """# HEMANG :: A Terminal-Based Interactive Resume

## Summary

This project is a unique and interactive single-page web application that presents a personal resume in the style of a terminal command center. It combines a minimalist, retro aesthetic with an engaging command-line interface, offering a creative way to explore professional information. The application now includes multiple themes, ASCII art, and simple text-based games to enhance user engagement. Built with a lightweight stack of HTML, CSS, and vanilla JavaScript, the application is fast, responsive, and easily customizable.

## Setup

This is a static web application and requires no build process.

1.  **Clone the repository:**
    
```
bash
    git clone https://github.com/23f3001304/Single-page-Site-terminal-try2.git
    
```

2.  **Navigate to the directory:**
    ```
bash
    cd Single-page-Site-terminal-try2
    
```

3.  **Open the application:**
    Simply open the `index.html` file in any modern web browser.

## Usage

Interact with the application by typing commands into the terminal. For a list of available commands, type `help`.

### Core Commands

| Command | Description |
| --- | --- |
| `help` | Displays a list of all available commands. |
| `clear` | Clears all output from the terminal screen. |
| `whoami` | Displays a brief biography. |
| `socials` | Provides links to social and professional profiles. |
| `contact` | Displays contact information. |
| `theme [name]` | Cycles through available visual themes. |
| `art` | Displays an ASCII art piece with the text "just a chill human". |
| `games` | Lists available mini-games to play in the terminal. |
| `download` | Provides a link to download a PDF version of the resume. |

### Resume Commands

| Command | Description |
| --- | --- |
| `experience` | Details professional and research experience. |
| `skills` | Lists key technical and research skills. |
| `projects` | Showcases selected projects with descriptions. |
| `education` | Displays educational background. |
| `achievements`| Highlights significant accomplishments and awards. |

## Code Explanation

The application is built with simplicity and extensibility in mind, using only vanilla HTML, CSS, and JavaScript.

*   **`index.html`**: The main entry point of the application, containing the structure of the terminal interface.
*   **`style.css`**: This file contains all the styling for the application, including the different color themes for the terminal.
*   **`script.js`**: The core of the application. It handles command parsing, executes the corresponding functions, and displays the output in the terminal. This file implements features such as ASCII art and games.

### Key Features

*   **Command Parser**: A simple function that takes user input, splits it into a command and arguments, and calls the appropriate function.
*   **Theming**: The `theme` command dynamically updates CSS variables to change the colors of the terminal.
*   **ASCII Art**: The `art` command prints a pre-defined ASCII art string to the terminal.
*   **Terminal Games**: The `games` command introduces a simple game loop, allowing for interactive text-based games within the terminal.

## License

This project is licensed under the MIT License. See the `LICENSE` file for full details.
"""
print(markdown_output)
```