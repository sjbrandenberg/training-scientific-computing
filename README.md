# Training Template

> Krishna Kumar, UT Austin

- Template for DesignSafe training built using [Jupyter Book](https://jupyterbook.org/en/stable/intro.html).
- Fork this [repo](https://github.com/DesignSafe-CI/training-template)
- To add `Open In DesignSafe` in Jupyter Notebooks copy the jupyter notebook to Community Data and then point the URL to the folder in Community Data `https://jupyter.designsafe-ci.org/hub/user-redirect/lab/tree/CommunityData/`
- The repo will automatically build a website using GitHub pages

## Template edits
- `_config.yml` Edit for title, author and URL
- `_toc.yml` Set-up the table of contents
- You can write markdown and Jupyter Notebooks and add to table of contents `_toc.yml`

## Build locally

```
# Create a virtual env
virtualenv env
source env/bin/activate
# Install required packages
pip3 install -r requirements.txt
# Build your book
jupyter-book build .
```

This will create a `_build/html` directory with all the files. Open the `index.html` file to start

## Jupyter example templates

**Exercise:** 
[![Try on DesignSafe](https://raw.githubusercontent.com/DesignSafe-CI/training-template/main/DesignSafe-Badge.svg)](https://jupyter.designsafe-ci.org/hub/user-redirect/lab/tree/CommunityData/Training/template/01-template-exercise.ipynb)

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DesignSafe-Training/DesignSafe-CI/blob/main/01-template-exercise.ipynb)

**Solution:** 
[![Try on DesignSafe](https://raw.githubusercontent.com/DesignSafe-CI/training-template/main/DesignSafe-Badge.svg)](https://jupyter.designsafe-ci.org/hub/user-redirect/lab/tree/CommunityData/Training/template/01-template-exercise.ipynb)

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DesignSafe-Training/DesignSafe-CI/blob/main/01-template-exercise.ipynb)

