# Git and GitHub Conventions

This document outlines the conventions I use for Git and GitHub to keep my work consistent, traceable, and professional.

## Repository Structure

For data-related projects, I aim for a structure similar to:

```text
project-name/
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
├── reports/
│   └── figures/
└── docs/
```

This helps separate data, code, notebooks, and outputs, and makes projects easier to navigate and reproduce.

## Commit Messages

I use clear, imperative-style commit messages, for example:

- `Add initial project structure for churn analysis`
- `Refactor data cleaning functions into src/data.py`
- `Update README with problem statement and results`

I avoid vague messages like `update` or `fix`.

A good commit message should:

- Start with a verb in imperative mood.
- Be specific about what changed.
- Be short but informative (one line summary, optional detail below).

## Branching

- `main` – stable, production-ready code and documentation.
- `feature/*` – new features or analyses (e.g. `feature/eda`, `feature/model-training`).
- `experiment/*` – experimental ideas that may or may not be merged.

I merge to `main` only after:

- Code runs without errors.
- Key outputs are verified.
- Documentation is updated.

## Documentation

Each project repository will include:

- A concise README with problem, data, approach, and results.
- Clear instructions to reproduce the analysis.
- Notes on assumptions, limitations, and possible next steps.

These conventions help me maintain a professional, consistent workflow across all my data projects.
