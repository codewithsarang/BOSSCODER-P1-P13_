# BOSSCODER Web Development Laboratory (P1–P13)

**Author:** Sarang Bodhe<br>
**GitHub:** [codewithsarang](https://github.com/codewithsarang)<br>
**Repository:** [BOSSCODER-P1-P13_](https://github.com/codewithsarang/BOSSCODER-P1-P13_)

This repository contains the practical work for the BOSSCODER School of Technology Programming for Web Development laboratory. It covers terminal navigation, Git and GitHub workflows, semantic HTML, reusable CSS tokens, positioning, Flexbox, and CSS Grid.

> Personal education and contact details that were not supplied are explicitly marked for editing. Practical project cards link to pages in this repository; they do not claim outside client or employment work.

## Practical index

| Practical | Demonstration | Files |
|---|---|---|
| P1 | Project folder and terminal navigation | [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md) |
| P2 | Portfolio repository and initial Git commit workflow | [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md), [web-practicals/index.html](./web-practicals/index.html) |
| P3 | Feature branch, commit, push, and merge workflow | [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md), `feature/about-section` branch |
| P4 | README, annotated version tag, and GitHub remote | [README.md](./README.md), [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md) |
| P5 | Semantic biography with education, skills, interests, goals, and contact | [web-practicals/bio.html](./web-practicals/bio.html) |
| P6 | Full semantic portfolio structure | [web-practicals/portfolio.html](./web-practicals/portfolio.html) |
| P7 | Centralized design tokens and typography | [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P8 | Sticky navigation, fixed control, positioning modes, overlay, and stacking | [web-practicals/positioning.html](./web-practicals/positioning.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P9 | Responsive navigation and wrapping Flexbox cards | [web-practicals/flexbox.html](./web-practicals/flexbox.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P10 | Flexible header and footer components | [web-practicals/flexbox.html](./web-practicals/flexbox.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P11 | Newspaper layout with three-column CSS Grid and named areas | [web-practicals/newspaper.html](./web-practicals/newspaper.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P12 | Featured projects, responsive Grid, `auto-fit`, and `auto-fill` | [web-practicals/projects.html](./web-practicals/projects.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P13 | Flexbox and Grid examples with a comparison table | [web-practicals/layout-choice.html](./web-practicals/layout-choice.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |

## Project structure

```text
.
├── .gitignore
├── P1-P4-Git-Workflow.md
├── README.md
├── SUBMISSION.md
└── web-practicals/
    ├── bio.html
    ├── flexbox.html
    ├── index.html
    ├── layout-choice.html
    ├── newspaper.html
    ├── portfolio.html
    ├── positioning.html
    ├── projects.html
    └── css/
        └── styles.css
```

## Technology

- HTML5 with semantic landmarks and accessible navigation
- CSS custom properties, responsive media queries, Flexbox, and Grid
- Git and GitHub
- No JavaScript, framework, or build step is required

## Run locally

1. Clone the repository or open this repository folder in VS Code.
2. Open `web-practicals/index.html` directly in a browser, or use VS Code Live Server if installed.
3. Use the site navigation or practical index to open P5–P13.
4. Resize the browser or use Developer Tools to inspect desktop (1440px), tablet (768px), and mobile (375px) layouts.

For Terminal navigation and Git exercises, follow [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md).

## Git workflow

Useful commands for inspecting this repository:

```bash
git status --short --branch
git log --oneline --decorate --graph --all
git branch -a
git remote -v
git tag --list
```

The feature branch and version tag are maintained without rewriting the existing repository history. See the [P1–P4 workflow guide](./P1-P4-Git-Workflow.md) for safe, reproducible commands.

## Testing

The practical pages are static HTML and CSS and can be tested in a browser without a server or dependencies. Check navigation, stylesheet loading, page layout, and horizontal overflow at the three viewport widths listed above. The final validation results and any remaining manual checks are recorded in [SUBMISSION.md](./SUBMISSION.md).

## Before submitting

- Add your real institution/program/dates and preferred email to [bio.html](./web-practicals/bio.html).
- Review the content and replace any details that do not describe you.
- Capture your own screenshots if required by your instructor.
- Verify the final branch and tag state with the Git commands above.
