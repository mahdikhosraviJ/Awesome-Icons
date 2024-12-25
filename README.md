# Awesome-Icons [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

This repository hosts a collection of icons displayed beautifully on mahdikhosravij.github.io/awesome-icons

## Features
- **Dynamic Icon Loading**: Icons are loaded from YAML files located in the `data/icons/` directory.
- **Responsive Grid**: A grid layout displays the icons with a modern and clean design.
- **Search Functionality**: Quickly filter icons by name using the search box.
- **Download and Copy Buttons**: Each icon has options to download or copy its SVG code.
- **License Information**: Displays creator details for each icon.
- **Automatic Deployment**: Deploys automatically to GitHub Pages using GitHub Actions.

## Project Structure
```plaintext
.
├── archetypes/          # Default archetypes for content creation
├── content/             # Content files (if any)
├── data/
│   └── icons/           # YAML files containing icon data
│       ├── iconpack1.yml
│       ├── iconpack2.yml
├── layouts/             # Hugo templates for the site
│   ├── _default/
│   │   ├── baseof.html  # Base template
│   │   ├── list.html    # Template for listing icons
├── static/              # Static assets (e.g., images, CSS, JS)
├── themes/
│   └── awesome-icons/   # Custom theme for the project
├── .github/
│   └── workflows/
│       └── deploy.yml   # GitHub Actions workflow for deployment
├── config.toml          # Hugo configuration file
└── public/              # Generated static site (ignored by Git)
```

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/mahdikhosraviJ/Awesome-Icons.git
   cd Awesome-Icons
   ```

2. **Install Hugo**
   Follow the instructions at [https://gohugo.io/getting-started/installing/](https://gohugo.io/getting-started/installing/).

3. **Run the Development Server**
   ```bash
   hugo server
   ```
   Open your browser and navigate to `http://localhost:1313/`.

## Adding Icons

1. Add a YAML file in the `data/icons/` directory (e.g., `iconpack1.yml`).

   Example:
   ```yaml
   icons:
     icon1: '<svg>...</svg>'
     icon2: '<svg>...</svg>'
   ```

2. Hugo will automatically load and display these icons on the site.

## Deployment

This project uses GitHub Actions to automate deployment to GitHub Pages.

1. Push your changes to the `main` branch.
2. The `deploy.yml` workflow builds the site and pushes it to the `gh-pages` branch.
3. Enable GitHub Pages in the repository settings and set the source to the `gh-pages` branch.

## Customization

### Modify the Layout
- Templates are located in `themes/awesome-icons/layouts/`.
- Update `baseof.html` or `list.html` to change the design.

### Tailwind CSS
- Modify the Tailwind CSS configuration in `themes/awesome-icons/tailwind.config.js`.
- Rebuild the CSS if you make changes.
  ```bash
  npx tailwindcss -i ./input.css -o ./output.css --minify
  ```

## Contributing

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch and open a pull request.

## License
All icons are subject to their respective licenses. Please ensure proper attribution to the creators as displayed on the site.

---

Enjoy using Awesome Icons!

