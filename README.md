# Jupyter Book Training Template

[![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue?logo=github)](https://img.shields.io/badge/GitHub-Pages-blue?logo=github)
[![Jupyter Book](https://img.shields.io/badge/Powered%20by-Jupyter%20Book-orange)](https://jupyterbook.org)

A customizable template for creating training materials on DesignSafe using [Jupyter Book](https://jupyterbook.org/en/stable/intro.html).

> Maintained by Krishna Kumar, University of Texas at Austin

## Features
- Pre-configured Jupyter Book structure
- GitHub Pages integration
- DesignSafe-specific workflows
- Easy content authoring with Markdown/Jupyter Notebooks
- Customizable table of contents
- "Open in DesignSafe" button integration

## Quick Start
1. **Fork the Repository**  
   [Fork original repository](https://github.com/DesignSafe-CI/training-template/fork)

2. **Enable GitHub Pages**  
   Go to Settings → Pages → Set source to `gh-pages` branch

3. **Clone Your Fork**
   ```bash
   git clone https://github.com/DesignSafe-CI/training-template.git

## Configuration
1. Basic Settings (`_config.yml`)

```yaml
title: "Your Training Title"
author: "Your Name"
url: "https://your-username.github.io/training-template"
```

2. Table of Contents (`_toc.yml`)
```yaml
format: jb-book
root: intro
chapters:
  - file: path/to/chapter1
  - file: path/to/chapter2
```

3. DesignSafe Integration

To add "Open in DesignSafe" buttons:

- Upload notebooks to `Community Data >> Training`
- Update notebook URLs to:
[![Try on DesignSafe](https://raw.githubusercontent.com/DesignSafe-CI/training-template/main/DesignSafe-Badge.svg)](https://jupyter.designsafe-ci.org/hub/user-redirect/lab/tree/CommunityData/Training/template/01-template-exercise.ipynb)

## Adding Content

Supported formats:

- 📝 Markdown (.md)

- 📓 Jupyter Notebooks (.ipynb)

- 🔄 MyST Markdown

### Organization tips:

```
├── content/
│   ├── intro.md
│   ├── chapter1/
│   │   ├── notebook.ipynb
│   │   └── images/
├── _toc.yml
└── _config.yml
```

## Building Locally
```bash
# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Linux/macOS
# venv\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt

# Build book
jupyter-book build .
```

## Serve built content (optional)

> python -m http.server --directory _build/html

## Deployment

Commit changes:
```bash
    git add .
    git commit -m "Update content"
    git push origin main
```

GitHub Actions will automatically:

    - Build book

    - Deploy to GitHub Pages

    - View at: https://<your-username>.github.io/training-template


## License

BSD 3-Clause License - See [LICENSE](LICENSE.md)

## Jupyter example templates

**Exercise:** 
[![Try on DesignSafe](https://raw.githubusercontent.com/DesignSafe-CI/training-template/main/DesignSafe-Badge.svg)](https://jupyter.designsafe-ci.org/hub/user-redirect/lab/tree/CommunityData/Training/template/01-template-exercise.ipynb)

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DesignSafe-Training/DesignSafe-CI/blob/main/01-template-exercise.ipynb)

**Solution:** 
[![Try on DesignSafe](https://raw.githubusercontent.com/DesignSafe-CI/training-template/main/DesignSafe-Badge.svg)](https://jupyter.designsafe-ci.org/hub/user-redirect/lab/tree/CommunityData/Training/template/01-template-exercise.ipynb)

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DesignSafe-Training/DesignSafe-CI/blob/main/01-template-exercise.ipynb)

