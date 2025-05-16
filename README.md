# Unicornia Wiki

[![build](https://github.com/kirin-3/unicornia-wiki/actions/workflows/build.yml/badge.svg)](https://github.com/kirin-3/unicornia-wiki/actions/workflows/build.yml)

The official documentation portal for the Unicornia community, providing helpful guides for both our Minecraft server and Discord community.

## 🌈 Overview

This wiki contains comprehensive documentation for:
- Minecraft server guides and tutorials
- Discord community guidelines and how-tos
- Community resources and features

Visit the live wiki at: [wiki.unicornia.net](https://wiki.unicornia.net/)

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip (Python package manager)

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/kirin-3/unicornia-wiki.git
   cd unicornia-wiki
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the development server:
   ```bash
   mkdocs serve
   ```

4. Visit `http://127.0.0.1:8000` in your browser to preview the site.

## 📝 Contributing

To add or modify content:

1. Create or edit Markdown files in the `docs/` directory
2. Update the navigation in `mkdocs.yml` if adding new pages
3. Preview your changes with `mkdocs serve`
4. Submit a pull request with your changes

### Content Structure

- `docs/minecraft/` - Minecraft server documentation
- `docs/discord/` - Discord community guides

## 🏗️ Building

To build the site for production:

```bash
mkdocs build
```

The built site will be located in the `site/` directory.

## 🔧 Technology

This wiki is built using:
- [MkDocs](https://www.mkdocs.org/) - Documentation framework
- [Material for MkDocs](https://github.com/squidfunk/mkdocs-material) - Theme and extensions