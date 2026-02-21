# 17.831 Data and Politics — Group Project

## Getting Started with GitHub Codespaces

Click the green **Code** button above, then select **Open with Codespaces** > **New codespace**.

The codespace will:
1. Build the development environment (1-2 minutes)
2. Install required packages
3. **Automatically open Marimo** in a preview tab

If Marimo doesn't open automatically, check the "Ports" tab in VS Code and click on port 2718.

## Creating Your Notebook

Create your project notebook in the `notebooks/` directory:

```bash
uv run marimo edit notebooks/project.py --host 0.0.0.0 --port 2718 --no-token
```

Or use the Marimo file browser that opens automatically to create a new notebook.

## Adding Dependencies

If your project needs additional Python packages, add them to `pyproject.toml` under `dependencies`, then run:

```bash
uv sync
```

## Submitting Your Work

Commit and push your changes:

**Option A: Using the terminal**
```bash
git add -A
git commit -m "Project submission"
git push
```

**Option B: Using VS Code**
1. Click the Source Control icon in the left sidebar
2. Stage your changes (+ button)
3. Enter a commit message
4. Click "Commit" then "Sync Changes"

## Running Locally

If you prefer to run locally instead of using Codespaces:

1. Install [uv](https://docs.astral.sh/uv/getting-started/installation/)
2. Clone this repository
3. Run:
   ```bash
   uv sync
   uv run marimo edit
   ```

## Need Help?

Post on the course discussion board or come to office hours.
