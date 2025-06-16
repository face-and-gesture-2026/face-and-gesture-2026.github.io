# FG 2026 - IEEE International Conference on Automatic Face and Gesture Recognition

This repository contains the official website for **The 20th IEEE International Conference on Automatic Face and Gesture Recognition (FG 2026)**, taking place from **May 25-29, 2026, in Kyoto, Japan**.

**Conference Website**: [https://face-and-gesture-2026.github.io](https://face-and-gesture-2026.github.io)

## Project Overview

This website is built using [Hugo](https://gohugo.io/), a fast static site generator, with a custom theme originally designed for conference websites. The site is deployed on GitHub Pages and serves as the primary information hub for conference attendees, speakers, and organizers.

## Prerequisites

Before you can run this project locally, you'll need to install the following dependencies:

### Required Dependencies

1. **Hugo Extended** (v0.120.0 or later)
   - Install [Hugo](https://gohugo.io/installation)
   - Make sure to get the "extended" version for SCSS processing
   - Verify installation: `hugo version`

2. **Git** (for cloning and managing submodules)
   - Download from [git-scm.com](https://git-scm.com/)
   - Verify installation: `git --version`

## Installation & Setup

### 1. Clone the Repository

```bash
git clone --recursive https://github.com/face-and-gesture-2026/face-and-gesture-2026.github.io.git
cd face-and-gesture-2026.github.io
```

### Run the Development Server

Start the Hugo development server:

```bash
hugo server -D
```

The site will be available at `http://localhost:1313`

For development with live reload and draft content:

```bash
hugo server -D --disableFastRender
```

## Building for Production

To build the static site for production:

```bash
hugo --minify
```

The built site will be available in the `public/` directory.

## Project Structure

```text
├── archetypes/          # Content templates
├── assets/              # Site assets (images, styles, etc.)
├── content/             # Markdown content files
├── data/                # Data files (YAML, JSON, TOML)
├── i18n/                # Internationalization files
├── layouts/             # Custom layout templates
├── public/              # Generated static site (ignored by git)
├── resources/           # Hugo resource cache
├── static/              # Static files (served as-is)
├── themes/              # Hugo themes (submodule)
│└── hugo-theme-event/  # Custom conference theme
├── hugo.yaml            # Main Hugo configuration
└── README.md            # This file
```


## Configuration

The main configuration is located in `hugo.yaml`. Key sections include:

- **Conference Details**: Title, dates, location
- **Theme Settings**: Colors, logos, sponsors
- **Menu Configuration**: Navigation structure
- **Language Settings**: Multi-language support

### Content Updates

1. Content is written in Markdown
2. Data such as speakers and sessions are stored in the file `assets/sessionize-view-all.json`
3. Images and assets go in the `assets/` directory

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the main branch. The deployment process:

1. GitHub Actions builds the site using Hugo
2. Generated files are deployed to the `gh-pages` branch
3. GitHub Pages serves the site from the `gh-pages` branch

## Support

For technical issues with the website, please:

1. Check the [Hugo documentation](https://gohugo.io/documentation/)
2. Review the theme documentation
3. Open an issue in this repository

For conference-related inquiries, please contact the organizing committee.
