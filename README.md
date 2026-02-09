# example-php

[![view-action-graph](https://img.shields.io/github/actions/workflow/status/actionforge/example-php/workflow.yml?label=View%20Action%20Graph)](https://app.actionforge.dev/github/actionforge/example-php/main/.github/workflows/graphs/build.act)

A simple Hello World app in PHP, built using an [Actionforge](https://actionforge.dev) graph as the CI/CD pipeline.

## Run

```bash
php index.php
```

## Graph

The build pipeline is defined as an Actionforge graph in [`.github/workflows/graphs/build.act`](.github/workflows/graphs/build.act):

```
checkout -> run (php index.php)
```

It runs on every push to `main`, on pull requests, and on manual dispatch.
