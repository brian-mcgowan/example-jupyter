# Example - Jupyter
A template repository for jump-starting development of Jupyter notebooks

## Development

### Create a Working Environment
It is best practice to create an isolated Python environment for each project
you work on to avoid dependency conflicts. I will use conda in this project, but
you can use your preferred environment manager.

Create a conda environment from `conda.yml`:
```shell
conda env create --file conda.yml
```

Optionally you can choose your own name for the environment:
```shell
conda env create --file conda.yml -n <custom-name>
```

### Install Dependencies
This project requires third-party dependencies to function. If you used conda to
create an environment in [Create a Working Environment](#create-a-working-environment)
this has already been done for you.

Install dependencies required for development:
```shell
pip install -r requirements-dev.txt
```

### Apply Code Formatting
Having a scripted code formatting tool improves readability and ensures
compliance with PEP. This project uses `black` to apply code style and
formatting.

Apply code formatting to all files in the `notebooks/` directory:
```shell
python -m black --include notebooks/* notebooks/
```

