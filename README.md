# Introduction to GitHub Course

## 1. Introduction to GitHub

### What is GitHub?
- **Definition**: GitHub is a web-based platform that uses Git, a distributed version control system, for tracking changes in source code during software development.
- **Importance**: Essential for collaboration, allowing multiple people to work on a project simultaneously. Widely used in open-source projects and professional development.

### Basic Concepts of Git and GitHub
- **Version Control System (VCS)**: Tracks changes, allows reverting to previous states, and manages modifications by multiple people.
- **Repositories**: 
  - *Local Repository*: On your computer, where changes are made.
  - *Remote Repository*: Stored on GitHub's server for sharing and collaborating.
- **Commits**: Records of changes to the repository, each with a unique ID.
- **Branches**: Different versions of the repository. Main branch is usually `main` or `master`.
- **Merges**: Combining changes from different branches.
- **Pull Requests**: Requests for someone to review and pull in your contribution.
- **Forks and Clones**: 
  - *Fork*: A GitHub copy of a repository for making changes without affecting the original.
  - *Clone*: Copying the repository to your local machine.

## 2. Setting Up

### Installing Git
- **Windows**: Download and install from [Git's website](https://git-scm.com/download/win).
- **Mac**: Use Homebrew (`brew install git`) or [Git's website](https://git-scm.com/download/mac).
- **Linux**: Install via the distribution's package manager (e.g., `sudo apt-get install git` for Ubuntu).

### Setting Up GitHub Account
- Sign up on [GitHub's website](https://github.com/).
- Fill in details and verify the account.

### Installing Visual Studio Code
- Download from [VS Code's website](https://code.visualstudio.com/Download).
- Follow installation instructions for your OS.

### Configuring Git with VS Code
- Open VS Code terminal (Ctrl+`).
- Set username: `git config --global user.name "Your Name"`.
- Set email: `git config --global user.email "your.email@example.com"`.

## 3. Basic Operations

### Creating a New Repository on GitHub
- **On GitHub**: Click 'New repository' > Name your repository > Initialize with a README (optional) > Create repository.
- **Example**: Creating "MyFirstRepo".

### Cloning a Repository in VS Code
- **Command**: `git clone https://github.com/username/MyFirstRepo.git`.
- Clone via VS Code's source control panel.

### Basic Git Commands
- `git add <filename>` or `git add .` (to add all changes).
- `git commit -m "Commit message"`.
- `git push` (to push to remote repository).
- `git pull` (to update local repository).
- `git branch <branchname>` (to create a new branch).
- `git checkout <branchname>` (to switch branches).

### Making Changes and Committing
- **Editing Files**: Edit files in VS Code.
- **Staging Changes**: Use `git add`.
- **Committing Changes**: `git commit -m "Your message"`.
- **Pushing to GitHub**: `git push`.

### Branching and Merging


1. **Create and Switch to the New Branch**
   Use the following command to create and switch to your new branch:
   ```bash
   git branch new-branch-name
   git checkout new-branch-name
   ```
   Replace `new-branch-name` with your desired branch name.

2. **Make Your Changes**
   Edit, add, or delete files in your project as needed.

3. **Stage Your Changes for Commit**
   ```bash
   git add .
   ```
   This command stages all your changes for the next commit.

4. **Commit the Changes**
   ```bash
   git commit -m "Describe your changes"
   ```
   Replace `Describe your changes` with a message describing what changes you've made.

5. **Push the New Branch to the Remote Repository**
   ```bash
   git push -u origin new-branch-name
   ```
   Replace `new-branch-name` with the name of your new branch.

6. **Switch to the Main Branch**
   ```bash
   git checkout main
   ```

7. **Pull the Latest Changes from Main**
   ```bash
   git pull origin main
   ```
   This ensures you have the latest changes from the remote main branch.

8. **Merge the New Branch into Main**
   ```bash
   git merge new-branch-name
   ```
   Replace `new-branch-name` with your branch's name. Resolve any merge conflicts if they arise.

9. **Push the Merged Changes to Remote**
   ```bash
   git push origin main
   ```

Remember to replace `new-branch-name` and `main` with the actual names of your branches. This guide will help you create a new branch, make commits, and merge it back into the main branch.