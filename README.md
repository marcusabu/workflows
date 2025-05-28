# Workflows

## Example usage
```
name: Deploy

on:
  push:
    branches:
      - main

jobs:
  Deploy:
    uses: marcusabu/workflows/.github/workflows/deploy.yml@main
    with:
      app_name: [appName]
    secrets:
      ssh_password: ${{ secrets.SSH_PASSWORD }}
```
