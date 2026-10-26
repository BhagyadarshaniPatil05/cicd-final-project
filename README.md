# OpenShift CI/CD Final Project

## Project Overview
A Python Flask application demonstrating automated linting and unit testing with GitHub Actions, plus Tekton task definitions for OpenShift Pipelines.

## Technologies
- Python and Flask
- GitHub Actions
- flake8
- nose
- Tekton
- OpenShift

## Application Endpoints
- / - Project welcome message
- /health - JSON health status

## GitHub Actions
Workflow file: .github/workflows/workflow.yml

The workflow installs dependencies, runs flake8, and executes unit tests with nose.

## Tekton Tasks
File: .tekton/tasks.yml

Includes a cleanup task and a nose testing task.

## Run Locally
Install dependencies with python -m pip install -r requirements.txt, then start the application using python app.py.

Open http://127.0.0.1:8080/ in your browser.

## Run Tests
Run python -m flake8 app.py tests --count --show-source --statistics
Run python -m nose -v

## OpenShift
Actual pipeline execution and deployment require a configured OpenShift cluster.
