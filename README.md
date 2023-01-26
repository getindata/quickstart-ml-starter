# GetInData ML Framework Kedro starter for GCP

## Overview
This is a `cookiecutter` template for Kedro, which features:
  * poetry
  * pre-commit hooks
  * Dockerfile setup
  * VSCode dev-containers for ease of development
  * MLFlow
  * VertexAI

## Usage
```bash
pip install kedro
kedro new --starter=https://gitlab.com/getindata/aa-labs/coe/gid-ml-framework-starter.git --checkout=local-gcp
# or kedro new --starter=git@gitlab.com:getindata/aa-labs/coe/gid-ml-framework-starter.git  --checkout=local-gcp
cd <my-project-name>  # change directory into newly created project directory
code .
```
