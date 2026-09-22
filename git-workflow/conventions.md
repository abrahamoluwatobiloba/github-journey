# Git and GitHub Basics

## What is Git?

Git is a version control system that helps track changes in files. It allows me to save versions of my work, review previous changes, and experiment without losing progress.

## What is GitHub?

GitHub is an online platform where Git repositories can be stored, shared, and collaboratively developed.

## Basic Git Workflow

```text
Make changes → Check changes → Stage changes → Commit changes → Push to GitHub
```

## Commands I Am Learning

| Command                   | Purpose                                      |
| ------------------------- | -------------------------------------------- |
| `git clone <url>`         | Copies a remote repository to my computer    |
| `git status`              | Shows the current state of the repository    |
| `git add .`               | Stages all changed files                     |
| `git commit -m "message"` | Saves staged changes with a description      |
| `git push`                | Uploads local commits to GitHub              |
| `git pull`                | Downloads and integrates changes from GitHub |
| `git log`                 | Displays the commit history                  |
| `git branch`              | Lists or manages branches                    |

## My Understanding

A commit is like a saved checkpoint. A good commit message explains what changed and makes the project history easier to understand.

## Example Workflow

```bash
git status
git add .
git commit -m "Add introductory GitHub documentation"
git push origin main
```

## Key Lesson

Git helps me manage the history of my work, while GitHub helps me share and collaborate on that work online.# Git and GitHub Conventions

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
