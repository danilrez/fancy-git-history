# 🚀 Fancy History

It is a fun little `python` toolkit designed to spice up your GitHub contribution graph! 🎨✨

![Preview1](https://raw.githubusercontent.com/danilrez/fancy-git-history/refs/heads/main/images/gameover.png)
![Preview2](https://raw.githubusercontent.com/danilrez/fancy-git-history/refs/heads/main/images/fancyhistory.png)

## 🔥 Features

-   **📆 Daily Commit Generator:** Randomly spreads commits throughout the year, making your graph look awesome.
-   **🎨 Graph Writer:** Lets you write cool phrases _(e.g., "GAME OVER")_ directly onto your contribution graph. Pretty neat, huh? 😎

---

## 🛠 Requirements

-   🐍 Python 3.x
-   🗃️ Git

---

## 🚀 Quick Installation

This project uses [python-dotenv](https://pypi.org/project/python-dotenv/) to load settings from a `.env` file.
If you hit an error like:

> ModuleNotFoundError: No module named **`dotenv`**

Here's how to fix it:

1. **Set Up a Virtual Environment** _(highly recommended)_:

    ```bash
    python3 -m venv venv
    source venv/bin/activate   # Windows: venv\Scripts\activate
    ```

2. **Install Dependencies:**

    ```bash
    python3 -m pip install python-dotenv
    ```

---

## ⚙️ Configuration

Create a file named **`.env`** at the root of your repo and add your settings. Here's an example:

```env
# Repository settings
REPO_URL=https://github.com/YOUR_GITHUB_NICK/YOUR_REPOSITORY
BRANCH_NAME=main

# Daily Commit Generator settings
TARGET_YEAR=2024
MIN_COMMITS_PER_DAY=1
MAX_COMMITS_PER_DAY=3

# Graph Writer settings
COMMITS_PER_X=5
```

All configs live in this `.env` file. Tweak as you like! 🔧

---

## 🚀 How to Use

1. Open your terminal and navigate to the project directory:

    ```bash
    cd /path/to/your/project
    ```

2. Ensure your repo is clean _(commit or stash your changes first)_. ✅
3. Run the scripts:

    **🎨 Generate commits for an entire year:**

    ```bash
    python3 src/fancy-history.py
    ```

    **🕹️ Add cool phrases like "GAME OVER":**

    ```bash
    python3 src/fancy-text.py
    ```

Want to customize more? Dive into the scripts and tweak them as you please. 🛠️

---

## 📝 Notes

-   The commit log file (`src/commit_log.txt`) is just a helper file for tracking fake commits. Add it to `.gitignore` or ignore it entirely. 📄
-   If your commits don’t immediately show, refresh your browser or select the correct year on your GitHub profile. 🔄
-   Always ensure your working directory is clean before running these scripts to avoid headaches. ⚠️

---

🚀 **Enjoy customizing your GitHub contribution graph!** 🎉

⭐️ **If you liked it, don't forget to hit that star button!** ⭐️
