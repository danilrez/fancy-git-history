# Fancy History

Fancy History is a `python` toolkit to jazz up your GitHub contribution graph! 🚀✨

## Features

-   **Daily Commit Generator:** Generates a random number of commits for every day within a specified year. 📆
-   **Inscription Generator:** Creates a custom inscription _(e.g., "GAME OVER")_ on your contribution graph. ✨

---

## Requirements

-   Python 3.x 🐍
-   Git 🗃️

---

## Installation

### Setting Up Python Dependencies

This project uses [python-dotenv](https://pypi.org/project/python-dotenv/) to load configuration from a `.env` file.
If you see an error like:

> ModuleNotFoundError: No module named **`dotenv`**

follow these steps:

1. Create a Virtual Environment _`(recommended)`_:

    ```bash
    python3 -m venv venv
    source venv/bin/activate   # On Windows: venv\Scripts\activate
    ```

2. Install Dependencies:

    ```bash
    python3 -m pip install python-dotenv
    ```

---

## Configuration

Create a file named **`.env`** in your repository root with your settings. For example:

```py
# Repository settings
REPO_URL=https://github.com/YOUR_GITHUB_NICK/YOUR_REPOSITORY
BRANCH_NAME=main

# Commit generation for Daily Commit Generator
TARGET_YEAR=2022
MIN_COMMITS_PER_DAY=1
MAX_COMMITS_PER_DAY=5

# Commit generation for Inscription Generator
COMMITS_PER_X=10
```

All configuration for the scripts is centralized in the `.env` file. Adjust the values as needed. 🛠️

### Script-Specific Settings

-   **Daily Commit Generator:**

    -   Edit `src/fancy-history.py` to adjust any parameters if needed.
    -   The commit log is stored in `src/commit_log.txt`.

-   **Inscription Generator:**
    -   Edit `src/fancy-text.py` to fine-tune the inscription _(e.g., "GAME OVER")_ using letter offsets and patterns.

---

## Usage

### Daily Commit Generator

1. Open a terminal and navigate to your project root:

    ```bash
    cd /path/to/your/project
    ```

2. Ensure your repository is clean _(commit or stash any changes)_.
3. Run the daily commit generator:

    ```bash
    python3 src/fancy-history.py
    ```

4. A color-coded progress bar will display the commit generation process. ⏳
5. Once finished, the commits will be pushed to your remote repository. 📤

### Inscription Generator

1. Open a terminal and navigate to your project root:

    ```bash
    cd /path/to/your/project
    ```

2. Ensure your repository is clean. ✅
3. Run the inscription generator:

    ```bash
    python3 src/fancy-text.py
    ```

This script will generate an inscription _(e.g., "GAME OVER")_ on your contribution graph. Adjust parameters in the script if needed. ✍️

---

## Notes

-   The generated commit log file (`src/commit_log.txt`) is used solely for generating fake commits and can be ignored (or added to your `.gitignore`). 📄
-   If the new commits do not immediately appear in your contribution graph, try a hard refresh in your browser or switch to the appropriate year view in your GitHub profile. 🔄
-   Ensure you have a clean working directory before running the scripts to avoid errors. ⚠️

---

Enjoy your customized GitHub contribution graph! 🎉
