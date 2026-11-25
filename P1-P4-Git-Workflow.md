# P1–P4: Terminal, Git & GitHub workflow

These practicals use the existing repository at `BOSSCODER_P1_P13`. Run commands from the repository root. This project already has a `.git` directory and the `origin` remote; **do not run `git init` or add a second remote**.

## P1: Project folder and terminal navigation

From Terminal, verify and navigate to this project:

```bash
cd ~/Downloads/BOSSCODER_P1_P13
pwd
ls -la
ls web-practicals
```

Useful navigation examples:

```bash
cd web-practicals
pwd
ls
cd ..
```

`pwd` prints the current directory, `ls` lists its contents, and `cd` changes directories. The practical pages are organized in `web-practicals/`, with shared styles in `web-practicals/css/`.

## P2: Portfolio repository and initial commit workflow

The supplied project is already a Git repository with an existing commit history. Inspect it instead of initializing a nested repository or recreating history:

```bash
git status --short --branch
git log --oneline --decorate --all
git remote -v
```

For a new local project, the general initial-commit sequence is:

```bash
git init
git add index.html style.css README.md
git diff --cached
git commit -m "Initial commit: create portfolio project structure"
```

Do **not** run `git init` in this existing assignment folder. Review `git status` and `git diff` before staging or committing changes.

## P3: Feature-branch workflow

The assignment work is developed on `feature/about-section` and merged into `main` after review. To demonstrate the workflow on a future change, use a unique branch name:

```bash
git switch main
git pull --ff-only origin main
git switch -c feature/your-change
# Edit and inspect the intended files.
git status
git diff
git add path/to/changed-file
git diff --cached
git commit -m "feat: describe the change"
git push -u origin feature/your-change
git switch main
git merge --no-ff feature/your-change
git push origin main
git log --oneline --graph --all
```

The commands above are examples; inspect the current remote state first and do not overwrite another contributor's work.

## P4: README and version tag

The repository's configured GitHub remote is:

```text
https://github.com/codewithsarang/BOSSCODER-P1-P13_.git
```

Inspect the configured remote and existing tags before publishing:

```bash
git remote -v
git tag --list
git ls-remote --heads origin
git ls-remote --tags origin
```

After the final assignment commit is on `main`, create and publish the version tag if it does not already exist:

```bash
git switch main
git tag -a v1.0.0 -m "Complete BOSSCODER P1-P13 web development practicals"
git push origin v1.0.0
git show v1.0.0
```

If `v1.0.0` already exists, do not move or overwrite it; inspect it and choose a new version only if appropriate. The README documents the practicals, technologies, structure, and local run instructions.

## Safety notes

- Never put passwords or access tokens in commands, files, or Git history.
- Do not force-push or rewrite the existing project history.
- Confirm the current branch and `git status` before each commit or merge.
- A successful local push command is not proof of remote state; verify with `git ls-remote` or the GitHub repository page.
