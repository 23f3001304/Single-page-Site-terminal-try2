# Web Terminal Resume

This project is a single-page, static web application designed to look and feel like a terminal. It serves as an interactive resume, allowing users to explore professional information through a familiar command-line interface.

This version enhances the original experience with new themes, mini-games, and a fun ASCII art feature, all while strictly preserving the original application's layout, commands, and feel. All legacy functionality remains untouched and performs identically.


![Web Terminal Resume Screenshot](https://user-images.githubusercontent.com/99264660/191244795-dd71fccb-c0da-4a8b-9807-742969968417.png)


## Summary of Features

-   **Terminal Interface:** A responsive, terminal-like UI built with React.
-   **Extensible Command System:** A simple, robust command parser for resume sections, themes, and interactive features.
-   **Expanded Theming:** The original theme is preserved as the default, now supplemented by two new optional palettes: "Aurora Drift" and "Mono Noir".
-   **Interactive Elements:** Includes a new ASCII art display and two embedded mini-games (`type-racer` and `asteroid-dodge`).
-   **Static & Fast:** Built as a static site for fast loading times and easy deployment.
-   **Zero Regression:** All original commands, keyboard shortcuts, animations, and data behave identically to the previous version.

## Setup

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/web-terminal-resume.git
    cd web-terminal-resume
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Start the development server:**
    ```bash
    npm start
    ```
    The application will be available at `http://localhost:3000`.

## Usage

Type a command and press `Enter`. The following commands are available.

### Standard Commands

-   `help`: Lists all available commands.
-   `about`: Displays a short bio.
-   `skills`: Shows a list of technical skills.
-   `projects`: Lists key projects with descriptions and links.
-   `contact`: Provides contact information.
-   `clear`: Clears all output from the terminal screen.

### Enhanced Commands

-   **`theme [name]`**
    Changes the terminal's color palette. The original look is the default and can be returned to at any time.
    -   `theme`: Lists available themes: `default`, `aurora-drift`, `mono-noir`.
    -   `theme default`: Applies the original theme.
    -   `theme aurora-drift`: Applies the "Aurora Drift" palette.
    -   `theme mono-noir`: Applies the "Mono Noir" palette.

-   **`ascii_mood`**
    Renders a friendly, chill-human portrait in monospaced ASCII art directly in the terminal. The display respects the current theme's colors, accessibility contrast, and the user's `prefers-reduced-motion` setting.

### Mini-Games

-   **`type-racer`**
    Starts a timed typing challenge using the terminal's existing typography. Type the displayed text and see your speed and accuracy.
    -   **To Exit:** Press `Ctrl+C` or type `exit` and press `Enter`.

-   **`asteroid-dodge`**
    Launches a lightweight, cursor-controlled avoidance mini-game rendered in the command output area.
    -   **Controls:** Use the `Up`, `Down`, `Left`, and `Right` arrow keys to move.
    -   **To Exit:** Press `q` or `Ctrl+C`.

## Code Explanation

This application is built with React and aims for a modular, component-based architecture.

-   **Command Processing:** User input is captured and sent to a central command parser. The parser identifies the command, validates any arguments, and executes the corresponding function. The output is then added to the terminal's history state, triggering a re-render.
-   **Component Structure:** The UI is broken down into logical components like `<Terminal>`, `<History>`, `<Input>`, and `<Output>`. New features like the games and ASCII art are rendered within the standard `<Output>` component to avoid altering the main DOM structure.
-   **State Management:** Core application state (command history, current theme) is managed using React hooks (`useState`, `useContext`) to ensure predictable updates and data flow.
-   **Extensibility:** New commands, themes, and interactive elements are designed to be added with minimal side effects. The `theme` command, for example, was expanded by simply adding new palette objects to the theme registry without modifying the original theme's definition or the command's core logic.

## License

This project is licensed under the MIT License.