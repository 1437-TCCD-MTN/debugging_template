# 🕵️‍♂️ Debugging Warm-up

Welcome to our daily debugging challenge! The goal of these warm-ups is to sharpen your problem-solving skills by analyzing existing code, identifying bugs, and fixing them. This is one of the most important and common tasks for a professional software developer.

## 🎯 Objective

Your mission is to find and fix all the bugs in this repository. The code provided does not work as intended. It may have syntax errors that prevent it from compiling, or it may have logical errors that cause it to run incorrectly or crash.

## ⚙️ Setup & Workflow

Follow these steps to get the assignment set up correctly within your Codespace environment.

1.  **Clone the Assignment:** In your Codespace terminal, make sure you are in the root directory (`/workspaces/<YourName>`). Clone this assignment repository using the `git clone` command and the URL from GitHub Classroom.

    ```bash
    git clone <your-assignment-repository-url>
    ```

2.  **Add to Workspace:**
    * In the top menu, click **File > Add Folder to Workspace...**
    * Select the folder for this assignment (e.g., `dw01-yourusername`) and click **OK**.
    * You should now see both your `Home` repository and the assignment folder in the file explorer on the left.

## 🕵️ Your Mission: The Debugging Process

Follow this systematic process to hunt down and eliminate the bugs.

1.  **Attempt to Compile:**
    * Open the terminal (ctrl+`).
    * Navigate into this assignment's directory (e.g., `cd dw01-yourusername`).
    * Run the CMake build process:
        ```bash
        cmake -S . -B build
        cmake --build build
        ```
    * **Pay close attention to the compiler errors!** These messages are your first and best clues for finding syntax-related bugs.

2.  **Create a Branch for Your Fix:**
    * **Direct pushes to the `main` branch are disabled.** You must do all work in 3 feature branch.
    * Before you start fixing a bug, create a new branch:
        ```bash
        # Make sure you are on the main branch and have the latest changes
        git checkout main
        git pull

        # Create and switch to a new branch
        git checkout -b fix/program-bugs
        ```

4.  **Investigate and Fix:**
    * Now, on your new branch, make the necessary code changes to fix the bug.
    * Once you have a fix, commit your changes with a clear and descriptive commit message that references the issue number:
        ```bash
        git add <files you changed>
        git commit -m "fix: <what you fixed>"
        ```

## ✅ Submission

Your assignment is complete when all bugs are fixed and all tests are passing. To submit your work, you will create a Pull Request for each branch you created.

1.  **Push Your Branch:** Push your committed changes from your local branch up to GitHub.
    ```bash
    git push -u origin fix/issue-name
    ```

2.  **Open a Pull Request:**
    * Use the GitHub Pull Request extension in VS Code to create a pull request.

3.  **Merge the Pull Request:**
    * Once the Pull Request is open, you can review your changes and then click **"Merge Pull Request"** to merge your fix into the `main` branch. Your work is considered submitted once all fixes are merged into the `main` branch.
