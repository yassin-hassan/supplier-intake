# 1. Python version and tooling

## Status
Accepted

## Context
The supplier_intake package, in particular its file parsing and validation (Stage 2), will later be reused inside an Odoo module. It must therefore run on a Python version Odoo supports.

## Decision
Python 3.12, uv for environments and dependencies, ruff for formatting and linting, mypy in strict mode, pytest, pre-commit, and GitHub Actions for CI.

## Consequences
One lockfile pins all versions, and the same checks run locally and in CI.