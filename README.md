# Portfolio Website Maintenance Guide

This guide provides instructions on how to maintain and update your portfolio website, which is hosted on GitHub Pages and built using Jekyll.

## 1. Website Overview

Your portfolio website showcases your learning journey and projects from Breda University of Applied Sciences. It features:

- **Live Site**: [https://ralphwarrand.github.io/portfolio/](https://ralphwarrand.github.io/portfolio/)
- **Repository**: [https://github.com/ralphwarrand/portfolio](https://github.com/ralphwarrand/portfolio)

### Key Features:
- **Modern Design**: Implemented a sleek, professional design with a vibrant color palette and improved typography.
- **Impactful Hero Section**: The homepage now features a dynamic hero section that immediately captures attention.
- **Enhanced Project Cards**: Project cards are visually appealing with subtle animations, clear tags, and improved readability.
- **Smooth Animations**: Added subtle animations for a more engaging user experience.
- **Improved Navigation**: The header and footer are cleaner and more intuitive.
- **Responsive Design**: Optimized for various devices, ensuring a consistent experience on desktops, tablets, and mobile phones.
- **Fixed 404 Errors**: All project links and the "Get In Touch" link now correctly navigate to their respective pages.
- **Cleaned Homepage**: Removed redundant "Home" text, fixed "About Me" text rendering, and eliminated duplicate "My Learning Journey" sections.

## 2. Adding New Content (e.g., Year 3 PowerPoints)

The website is structured to easily integrate new content from your PowerPoint presentations. Follow these steps:

### Step 2.1: Place New PowerPoint Files
Place your new PowerPoint files (e.g., `Y3A.pptx`, `Y3B.pptx`) into the `upload/` directory within your local project environment. If you are working directly in the GitHub repository, you will need to manually extract the content or run the extraction script locally.

### Step 2.2: Run the Extraction Script

I have provided a Python script (`extract_pptx_data.py`) that automates the extraction of text and images from your PowerPoint files and saves them in a structured format. Another script (`create_project_pages.py`) then uses this extracted data to generate new project pages for your Jekyll site.

To run these scripts:

1.  **Ensure Python and `python-pptx` are installed:**
    ```bash
    pip install python-pptx
    ```

2.  **Run the extraction script:**
    ```bash
    python3 extract_pptx_data.py
    ```
    This will create new directories under `extracted_pptx_data/` for each new PowerPoint, containing `_text.txt` files and `slide_*.png` images.

3.  **Run the project page creation script:**
    ```bash
    python3 create_project_pages.py
    ```
    This script will:
    -   Read the extracted text from `extracted_pptx_data/`.
    -   Generate new Markdown files (`.md`) in the `_projects/` directory for each new academic block (e.g., `_projects/y3a.md`).
    -   Copy the extracted images from `extracted_pptx_data/` to `assets/images/`.

    **Important**: The `create_project_pages.py` script is designed to be run whenever you add new PowerPoint files. It will automatically create or update the corresponding project pages and copy the images.

### Step 2.3: Update `_config.yml` (if necessary)

If you introduce new categories or need to adjust the site-wide settings, you might need to modify `_config.yml`. For new project blocks, the `create_project_pages.py` script handles the necessary data for the project cards.

### Step 2.4: Review and Commit Changes

After running the scripts, review the newly generated Markdown files and copied images. Ensure everything looks correct. Then, commit and push your changes to the GitHub repository:

```bash
git add .
git commit -m "Add Year 3 content and update portfolio"
git push origin main
```

GitHub Pages will automatically rebuild and deploy your site with the new content.

## 3. Customizing the Design

All styling is managed in `assets/main.css`. You can modify this file to change the look and feel of your website.

### Key CSS Variables:

Open `assets/main.css` and look for the `:root` selector at the top. Here you can adjust:

-   `--primary-color`, `--secondary-color`, `--accent-color`: For main brand colors.
-   `--text-primary`, `--text-secondary`, `--text-light`: For text colors.
-   `--bg-primary`, `--bg-secondary`, `--bg-dark`: For background colors.
-   `--border-color`, `--shadow-sm`, `--shadow-md`, `--shadow-lg`, `--shadow-xl`: For borders and shadows.
-   `--border-radius`: For rounded corners.
-   `--transition`: For animation smoothness.

### Layouts:

-   `_layouts/default.html`: The base layout for all pages, including header and footer.
-   `_layouts/home.html`: The layout for the homepage, including the hero section and project grid.
-   `_layouts/project.html`: The layout for individual project pages.

### Homepage (`index.md`):

-   The `index.md` file contains the content for your homepage, including the 

