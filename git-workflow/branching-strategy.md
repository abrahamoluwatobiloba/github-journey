# Branching Strategy

## Branch Types

- `main`  
  Stable branch. Only merged, reviewed, and tested work goes here.

- `feature/*`  
  Used for new analyses, models, or dashboards.  
  Examples: `feature/eda`, `feature/classification-model`.

- `experiment/*`  
  Used for exploratory or experimental work that may not be merged.  
  Examples: `experiment/hyperparameter-tuning`, `experiment/new-features`.

## Workflow

1. Create a branch from `main`:
   
   ```bash
   git checkout -b feature/eda
   ```
2. Work on the feature or analysis.
3. Commit with clear messages.
4. Open a pull request (if collaborating) or merge after self-review:
   
   ```bash
   git checkout main
   git merge feature/eda
   git push origin main
   ```
5. Delete the feature branch when no longer needed.

This approach keeps `main` clean and makes my project history easier to understand.
