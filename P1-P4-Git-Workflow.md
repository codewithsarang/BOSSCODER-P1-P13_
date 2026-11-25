# P1–P4: Terminal, Git & GitHub workflow

These are command-line practicals. Run commands from Terminal. Replace `your-github-username` and email with your own details.

## P1: Project folder and terminal navigation

```bash
# Go to your Desktop
cd ~/Desktop

# Create the assignment folder
mkdir bosscoder-web-lab

# Enter the folder
cd bosscoder-web-lab

# Show the current directory
pwd

# List files (including hidden files)
ls -la

# Create folders
mkdir web-practicals screenshots

# Move one directory up
cd ..

# Return to the project
cd ~/Desktop/bosscoder-web-lab
```

Useful commands:
- `pwd` – prints the current directory.
- `ls` – lists files and folders.
- `cd folder-name` – enters a folder.
- `cd ..` – moves to the parent folder.
- `mkdir name` – creates a directory.
- `touch file.txt` – creates an empty file.

## P2: Portfolio repo with an initial commit

```bash
cd ~/Desktop/bosscoder-web-lab
git init
git status
git add .
git status
git commit -m "Initial commit: portfolio lab setup"
git log --oneline
```

What this does:
1. `git init` creates a local Git repository.
2. `git add .` stages project files.
3. `git commit` saves a version of the staged files.
4. `git log --oneline` displays commit history.

## P3: Feature-branch Git workflow

```bash
# Create and switch to a feature branch
git switch -c feature/portfolio-homepage

# Make a change in VS Code, then stage and commit it
git status
git add .
git commit -m "Add portfolio homepage"

# Return to the main branch
git switch main

# Merge the feature branch into main
git merge feature/portfolio-homepage

# View branch history
git log --oneline --graph --all
```

If your default branch is named `master`, use `master` instead of `main`.
Do not delete the feature branch until you have confirmed the merge succeeded.

## P4: GitHub README and version tags

1. Sign in at https://github.com/ and create a new repository named `bosscoder-web-lab`.
2. Do not initialize it with a README if you already have a local README.
3. In Terminal, from your project folder, connect and push:

```bash
git remote add origin https://github.com/your-github-username/bosscoder-web-lab.git
git push -u origin main
```

4. Create a version tag and push it:

```bash
git tag -a v1.0.0 -m "First complete portfolio lab version"
git push origin v1.0.0
git tag
```

If GitHub says the remote already exists, inspect it with `git remote -v`; do not blindly add it again.
If you created the GitHub repository with an initial commit, you may need to pull and reconcile histories before pushing.
