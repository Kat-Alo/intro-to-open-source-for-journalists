# GitHub Setup Guide

GitHub is a powerful platform for version control and collaboration on software projects. This guide will help you get started with the basics: creating an account, cloning a repository, searching through GitHub issues, opening an issue, and making a pull request.

## Creating an Account

See [Github's docs](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github) or just follow these steps:

1. **Visit GitHub**: Go to [github.com](https://github.com/).
2. **Sign Up**: Click on "Sign up" in the top-right corner.
3. **Fill in Your Details**: Provide a username, email address, and password.
4. **Choose a Plan**: Start with the free plan.
5. **Verify Your Email**: Check your inbox and click the verification link.

Now, you have a GitHub account!

## Cloning a Repository

A repository (or repo) is where a project’s files are stored. Cloning a repo means downloading a copy of it to your computer.

1. **Find the Repo**: Go to the repository page on GitHub.
2. **Clone the Repo**: Click the green “Code” button, then click the clipboard icon next to the URL to copy it. We'd recommend using HTTPS. It's less secure, but much easier to configure when you're just getting started.
3. Create a new directory where your repo will get cloned (usually just with the same name as the repo). You can do this with your file management application (e.g. Finder), or with your terminal by running `mkdir name-of-directory`
4. **Use Git to Clone**:
   - Open your terminal (or Command Prompt).
   - Type `git clone <repo-url>`, replacing `<repo-url>` with the URL you copied.
   - Press Enter, and the repo will be downloaded to your computer.

## Searching Through GitHub Issues

GitHub Issues is a feature for tracking tasks, bugs, and feature requests.

1. **Go to the Repo**: Navigate to the repository on GitHub.
2. **Click on "Issues"**: This tab lists all the open issues.
3. **Search for Issues**: Use the search bar at the top to type keywords related to the issue you’re interested in. You can also filter issues by labels, assignees, or other criteria.

## Opening a GitHub Issue

If you encounter a bug, have a question, or want to suggest a feature, you can open a new issue.

1. **Navigate to the Issues Tab**: Go to the repository's Issues tab.
2. **Click "New Issue"**: This button is usually found near the top right.
3. **Fill in the Details**: Provide a title and a detailed description. Use Markdown for formatting if needed.
4. **Submit**: Click "Submit new issue."

Your issue will be added to the list, where others can view and comment on it.

## Opening a Pull Request (PR)

A pull request is a way to propose changes to a repository. It lets others review your changes before they are merged into the main project. There are two common approaches to create a pull request: by forking the repository or by creating a new branch.

### Option 1: Forking the Repository

1. **Fork the Repo**: Click "Fork" at the top right of the repo page. This creates a copy of the repo under your account.
2. **Make Your Changes**: Clone your forked repo, make changes on your local machine, and commit them.
3. **Push Changes to GitHub**: Use `git push origin <branch-name>` to push your changes.
4. **Create a PR**: 
   - Go back to the original repo on GitHub.
   - Click "Compare & pull request."
   - Review the changes, add a description, and click "Create pull request."

### Option 2: Creating a New Branch

1. **Create a Branch**: 
   - Open the repository in your GitHub account or the original repository if you have write access.
   - In the terminal, navigate to the repo's directory and create a new branch with `git checkout -b <branch-name>`.
2. **Make Your Changes**: Make changes to your branch locally and commit them.
3. **Push the Branch**: Use `git push origin <branch-name>` to push your branch to GitHub.
4. **Create a PR**:
   - Go to the repository on GitHub.
   - Click "Compare & pull request."
   - Review the changes, add a description, and click "Create pull request."

Now, the repo maintainers can review and merge your changes.