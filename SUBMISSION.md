# Submission guide and validation report

## Practical map

| Practical | What it demonstrates | Files |
|---|---|---|
| P1 | Terminal navigation and existing project organization | [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md) |
| P2 | Existing repository inspection and initial-commit commands | [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md) |
| P3 | Feature branch and safe merge workflow | [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md), `feature/about-section` |
| P4 | README, GitHub remote, and version tag workflow | [README.md](./README.md), [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md) |
| P5 | Semantic biography and personal information sections | [web-practicals/bio.html](./web-practicals/bio.html) |
| P6 | Semantic portfolio page with hero, about, skills, projects, education, and contact | [web-practicals/portfolio.html](./web-practicals/portfolio.html) |
| P7 | CSS tokens and type scale | [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P8 | Positioning modes, sticky navigation, fixed link, overlay, and z-index | [web-practicals/positioning.html](./web-practicals/positioning.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P9 | Responsive navigation and flexible card row | [web-practicals/flexbox.html](./web-practicals/flexbox.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P10 | Flex item sizing/alignment and responsive footer | [web-practicals/flexbox.html](./web-practicals/flexbox.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P11 | Three-column newspaper layout with Grid areas | [web-practicals/newspaper.html](./web-practicals/newspaper.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P12 | Featured project cards with `auto-fit` and `auto-fill` | [web-practicals/projects.html](./web-practicals/projects.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |
| P13 | Working Flexbox/Grid examples and comparison table | [web-practicals/layout-choice.html](./web-practicals/layout-choice.html), [web-practicals/css/styles.css](./web-practicals/css/styles.css) |

## How to run

Open `web-practicals/index.html` in a browser, or open the repository in VS Code and use Live Server if installed. No build step or external packages are required. Follow [P1-P4-Git-Workflow.md](./P1-P4-Git-Workflow.md) for command-line practicals.

## Screenshot checklist

Capture your own screenshots if your instructor requires evidence. Suggested views:

1. `web-practicals/index.html` at 1440px, showing the practical index.
2. `web-practicals/bio.html` showing biography sections (after you fill your personal education/contact details).
3. `web-practicals/positioning.html` while scrolled, showing the sticky header and fixed control.
4. `web-practicals/flexbox.html` at desktop and mobile widths.
5. `web-practicals/newspaper.html` at desktop and mobile widths.
6. `web-practicals/projects.html` and `web-practicals/layout-choice.html`.

No screenshots are included or claimed as captured in this repository.

## Git evidence commands

From the repository root, capture the real output of:

```bash
git status --short --branch
git log --oneline --decorate --graph --all
git branch -a
git remote -v
git show --stat --oneline HEAD
git show v1.0.0 --no-patch
git ls-remote --heads origin
git ls-remote --tags origin
```

The configured repository link is [github.com/codewithsarang/BOSSCODER-P1-P13_](https://github.com/codewithsarang/BOSSCODER-P1-P13_). Verify the remote branch and tag state before submission; do not treat local refs alone as proof that they were pushed.

## Validation checklist

- [x] P1–P13 instructions and page content reviewed.
- [x] Opened every P5–P13 HTML page in the browser; the shared stylesheet loaded.
- [x] Checked local navigation links and same-page/cross-page anchors.
- [x] Checked responsive layouts at 1440px, 768px, and 375px.
- [x] Confirmed no horizontal overflow at those widths; the responsive Grid and Flexbox tracks adapt as intended.
- [x] Checked the positioning demo while scrolled: sticky header remained at the viewport top and fixed control stayed in view.
- [x] Browser reported no JavaScript/page errors; the pages use no JavaScript and contain no images.
- [ ] Replace the clearly marked email and education details on the biography page.
- [ ] Capture requested screenshots yourself.
- [ ] Verify `main`, `feature/about-section`, and `v1.0.0` locally and remotely after publishing.

### Executed checks

- Browser-tested all eight practical HTML pages at 1440px, 768px, and 375px. All rendered with the shared stylesheet; `scrollWidth` matched the viewport width on every page and each viewport.
- Checked navigation targets and anchors with a local link checker; all resolved.
- Checked CSS Grid column changes for the newspaper and projects pages and Flexbox wrapping for the card row at all three viewport widths.
- Confirmed sticky-header and fixed-control behavior on P8.
- `git diff --check` passed.
- HTML Tidy is installed, but this machine's binary is a 2006 build that reports HTML5 elements such as `header` and `nav` as unsupported. Its output is therefore not treated as an HTML5 validation result. The browser parser rendered all pages successfully; no external validator result is claimed.

## Remaining personal submission steps

- Add your institution, program, study dates, and preferred email to [web-practicals/bio.html](./web-practicals/bio.html).
- Review and personalize all first-person copy.
- Capture screenshots if required by your instructor.
- Submit the GitHub repository URL and any requested evidence through your course portal.
