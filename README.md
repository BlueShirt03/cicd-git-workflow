# cicd-git-workflow
A repository demonstrating a standardized Feature Branch Git workflow for reliable integration and Continuous Integration practices.

## Project Overview

This repo demonstrates a standardized Git workflow designed to support Continuous Integration (CI) practices.

This project will use the Feature Branch Worflow to ensure that changes are developed separately from the main branch before being reviewed and merged.

## Workflow 

Development changes are made using dedicated branches rather then directly on the 'main' branch. Changes are submitted through Pull Requests and reviewed before being merged into 'main'.

## Repository Structure 

- README.md - Provides an overview of the project.
- GIT_WORFLOW.md - Documents the Git workflow, branching naming conventions, commit standards, and merge approval process. 
- .gitignore - Prevents unnecessary Python-generated files from being tracked by Git.

## Branching Strategy

This repository uses the Feature Branch Workflow.

The 'main' branch represents the stable version of the project. New development work is completed on separate branches and integrated into 'main' through Pull Requests.