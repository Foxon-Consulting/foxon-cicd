# Github-Actions Foxon-Consulting standards

## Introduction

The main branch of this repository has all the Foxon-Consulting FR standards for CICD.

## Adding a new Foxon CICD workflow:
Workflow are create by technologie/standard. The same discrimination as the ```.gitignore``` file

For example, for python, in .github/workflows:
- create ```python_integration.yml```
- create ```python_delivery.yml```
- create ```python_deploiement.yml```

This workflow will be then be used by all repository that follow the standard.yml pattern and/or have been created through cookie_cutter.

## Adding a new github actions
For "my_action", you have to create the file workflow_type/actions/my_action/action.yml

You can then create a action or even a composite actions. (See integration/actions/simple/action.yml)

## Cookiecutter template
The ```standard.yml``` file is prepared for cookiecutter with {{ cookiecutter.__cicd_type }} in branch "cookiecutter".

This file has been created to be placed as a submodule of cookiecutter foxon repository, for even more standardisation.
