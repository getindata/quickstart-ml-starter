# QuickStart ML Kedro starter

## Overview

This is a set of [Cookiecutter](https://www.cookiecutter.io/) templates in the form of [Kedro starters](https://kedro.readthedocs.io/en/0.18.0/get_started/starters.html). These starters allow to easily create a new project that doesn't implement any nodes or pipelines yet, but contains necessary tooling and follows all [QuickStart ML Blueprints](https://github.com/getindata/quickstart-ml-blueprints) principles.

QuickStart ML Blueprints repository and documentation with detailed description of the way of work can be found [here](https://github.com/getindata/quickstart-ml-blueprints).

Initiating a project using one of the Kedro starters you will get out-of-the box:
* appropriate project structure matching [Kedro](https://kedro.org/) and Cookiecutter standard that features configuration files, code testing framework, layered data-engineering convention and more
* [VSCode Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers) and Docker setup files to create a transferrable working environment automatically
* [MLFlow](https://mlflow.org/) and [Kedro-Viz](https://docs.kedro.org/en/0.17.4/03_tutorial/06_visualise_pipeline.html)
* A set of pre-configures environment management and code quality tools ([Poetry](https://python-poetry.org/), [pre-commit](https://pre-commit.com/) hooks, linters)
* Accordingly to your target full-scale environment - Kedro plugins setup for easy transfer and running your local work on [GCP](https://github.com/getindata/kedro-vertexai), [AWS](https://github.com/getindata/kedro-sagemaker),  [Azure](https://github.com/getindata/kedro-azureml) or [Kubeflow](https://github.com/getindata/kedro-kubeflow)

There are a few branches in the repository that use basically the same template, but have environment-specific additions depending on where are you planning to run your full-scale solution after local prototyping phase:
- `local` - if you plan to stay in local environment
- `local-gcp` - if you plan to transfer your project to Google Cloud (VertexAI)
- (to be added ) `local-aws` - if you plan to transfer your project to AWS (Sagemaker)
- (to be added ) `local-azure` - if you plan to transfer your project to Azure (AzureML)
- (to be added ) `local-kuberflow` - if you plan to transfer your project to Kubeflow

## Usage

To use this Kedro starter you to have some Python 3 environment with Kedro installed. The method of installation is up to you (you can use Pyenv and Poetry, Conda, Virtual Env etc.) - this installation Kedro is only needed to create a project from a starter. After that, the project will use its own encapsulated Pyenv/Poetry environment with its own Kedro.

To create a new project using Kedro starter:

```bash
# For HTTPS cloning:
kedro new --starter=https://github.com/getindata/quickstart-ml-starter.git --checkout=<branch_name>

# For SSH cloning:
kedro new --starter=git@github.com:getindata/quickstart-ml-starter.git  --checkout=<branch_name>

# Follow the prompts to name your project and optionally set cloud project details, then change directory into newly created project directory:
cd <my-project-name>
```

After that, follow the way of work described in [QuickStart ML Blueprints](https://github.com/getindata/quickstart-ml-blueprints) to develop your project.
