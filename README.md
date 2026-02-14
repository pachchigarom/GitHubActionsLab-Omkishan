# GitHub Actions Lab – Automated Workflows

## Overview

This project demonstrates the use of GitHub Actions to create automated workflows.  
Two workflows were implemented to showcase job dependencies and multi-platform parallel execution.

---

# Workflow 1 – Dependent Jobs Workflow

## Purpose
This workflow demonstrates job dependencies using the `needs` keyword.  
It ensures jobs execute in a specific order:

build → test → deploy

## Trigger
- Triggered on `push` to the `main` branch.

## Key Concepts Demonstrated

### 1. `on`
Defines when the workflow runs.
```yaml
on:
  push:
    branches:
      - main
