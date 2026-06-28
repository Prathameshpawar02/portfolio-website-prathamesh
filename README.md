# Portfolio Website

A personal portfolio website showcasing projects, skills, and experience.

## Project Structure

```
portfolio-website/
├── index.html      # Main HTML file
├── style.css       # Stylesheet
├── script.js       # JavaScript functionality
├── requirements.txt # Python dependencies
└── README.md       # This file
```

## Files Overview

- **index.html** - Main HTML structure and content
- **style.css** - Styling and layout for the website
- **script.js** - Interactive features and functionality

## Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Python 3.7+ (optional, for local development server)

### Running Locally

#### Option 1: Direct Browser
Simply open `index.html` in your web browser.

#### Option 2: Local Server (Recommended)
Use Python's built-in HTTP server:

```bash
# Python 3.x
python -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## Development

Install development dependencies:

```bash
pip install -r requirements.txt
```

## Features

- Responsive design
- Clean and modern UI
- Interactive elements with JavaScript

## Deployment
This project is a static website and can be deployed in multiple ways. Deployment files are now included in this repository.

### GitHub Pages (recommended)

1. Push this repository to GitHub on the `main` branch.
2. The included workflow at `.github/workflows/deploy_github_pages.yml` will publish the site automatically.
3. In your repository Settings → Pages, make sure the source is set to `GitHub Actions`.

### Netlify

1. Connect your GitHub repository to Netlify or drag and drop the repository folder.
2. The included `netlify.toml` configures the publish directory to the project root.

### Docker

Build and run the container locally:

```bash
docker build -t portfolio-site:latest .
docker run --rm -p 8080:80 portfolio-site:latest
```

Then open http://localhost:8080.

### Local testing

Serve the site locally with Python's simple HTTP server:

```bash
python -m http.server 8000
# Open http://localhost:8000
```

## License

© 2026 Your Name. All rights reserved.
