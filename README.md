# Git Workflow Guide

This guide outlines the essential Git commands to initialize a repository, track changes, commit them, and push them to a remote repository on GitHub.

## Initializing a Git Repository

1. Initialize Git in the current directory:
   ```bash
   git init
   ```
   This sets up a new Git repository in the current directory.

2. Check the status of the repository:
   ```bash
   git status
   ```
   This shows the state of the working directory and staging area.

3. Add files to the staging area:
   ```bash
   git add <file-name>
   ```
   - Stages a specific file for commit
   - Use `git add .` to stage all changes

4. Commit the staged changes:
   ```bash
   git commit -m "Initial commit"
   ```
   This saves a snapshot of the staged changes with a descriptive message.

## Linking to a Remote Repository on GitHub

1. Create a repository on GitHub:
   - Go to GitHub and create a new repository
   - Copy the repository URL (e.g., `https://github.com/username/repo.git`)

2. Link the local repository to GitHub:
   ```bash
   git remote add origin https://github.com/username/repo.git
   ```

3. Push the changes to GitHub:
   ```bash
   git push -u origin main
   ```
   The `-u` flag sets the default remote and branch for future pushes.

## Updating the Remote Repository

1. Make changes to files locally
2. Check the status:
   ```bash
   git status
   ```

3. Stage the changes:
   ```bash
   git add <file-name>
   ```

4. Commit the changes:
   ```bash
   git commit -m "Describe your changes"
   ```

5. Push the changes to GitHub:
   ```bash
   git push origin main
   ```

## Additional Tips

* View the commit history:
  ```bash
  git log
  ```

* If the branch `main` does not exist locally, rename the default branch:
  ```bash
  git branch -M main
  ```

* For frequent updates after setting the upstream branch, simply use:
  ```bash
  git push
  ```
