# Data Science Cookbook
This website hosts my commonly referenced notes on data science, machine learning, Python, and more.

There is an environment file to create a mamba/conda environment with all the necessary libraries:
> conda env create --file environment.yml

## Cookbook Creation Details
The data science cookbook is created using [Jupyter Book](https://jupyterbook.org/en/stable/intro.html).

Pages are build with this command:
> jupyter-book build project/ --path-output docs

Use the `--all` modifier when creating a new page so that the other pages reference it in the TOC.
> jupyter-book build --all project/ --path-output docs

Then move the files up a couple levels so `/_build/html/` isn't in the url link. 
> mv docs/_build/html/* docs/