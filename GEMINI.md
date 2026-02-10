# Project Context: nase-ucetni.cz

## Project Overview
This project is a static website serving as a landing page and portal ("Rozcestník") for **nase-ucetni.cz**. Its primary purpose is to provide a central location for accessing external presentations and materials (e.g., hosted on OneDrive).

## Technologies & Architecture
*   **Type:** Static Website.
*   **Core:** HTML5.
*   **Styling:** [Tailwind CSS](https://tailwindcss.com/) (loaded via CDN, no build step required).
*   **Typography:** Google Fonts (Inter family).
*   **Hosting:** Configured for static hosting (likely GitHub Pages), indicated by the presence of a `CNAME` file.

## Key Files
*   **`index.html`**: The main entry point. Contains all the structure, content, and embedded scripts for the landing page.
*   **`CNAME`**: Contains the custom domain configuration (`nase-ucetni.cz`).

## Development & Usage

### Running Locally
Since this is a simple static site with no build process:
1.  Open `index.html` directly in any modern web browser.
2.  Alternatively, use a simple HTTP server (e.g., `python3 -m http.server`, `npx serve`, or the VS Code Live Server extension) in the project root to preview.

### Adding Content
To add new presentations or links:
1.  Edit `index.html`.
2.  Locate the `#presentation-list` container.
3.  Duplicate the existing anchor (`<a>`) block representing a presentation card.
4.  Update the `href`, title, description, and icon as needed.

### Deployment
*   The site is designed to be served statically.
*   Ensure `CNAME` is present for custom domain support on platforms like GitHub Pages.
