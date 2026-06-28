# lessons

A personal daily-learning repository. Each day gets a structured lesson in two tracks — rhetoric and cognitive training — generated and committed automatically.

## What it is

This repo stores daily markdown lesson files organised by topic and date:

- `rhetoric/` — one file per day covering a specific rhetorical device, with definition, examples across three contexts (public speaking, writing, conversation), and a writing exercise.
- `cognitive/` — one file per day covering a specific cognitive skill (e.g. working memory, attention), with an exercise and a reflection prompt.
- `index.html` — a static HTML index page listing all lessons with links, suitable for serving directly via GitHub Pages.

Example lesson structure (`rhetoric/YYYY-MM-DD.md`):

```markdown
# Rhetoric — March 15, 2026

## 1. Device of the Day
Anadiplosis — repetition of the last word of one clause at the start of the next.

## 2. Three Examples
...

## 3. Your Challenge
...
```

Example cognitive lesson structure (`cognitive/YYYY-MM-DD.md`):

```markdown
# Cognitive — March 15, 2026

### 1. Skill: Working Memory
...

### 2. Exercise
...

### 3. Reflection
...
```

## Why it exists

Daily deliberate practice in rhetoric and cognitive skills compounds over time. Storing lessons in a git repo gives a permanent, searchable, version-controlled record of what was practised and when.

## Repository layout

```
lessons/
├── cognitive/
│   ├── 2026-03-15.md
│   └── ...
├── rhetoric/
│   ├── 2026-03-15.md
│   └── ...
└── index.html
```

## Viewing lessons

Open `index.html` in a browser, or browse the `rhetoric/` and `cognitive/` directories directly on GitHub.

If you fork and enable GitHub Pages on the repository, `index.html` serves as the entry point. The index links to `.html` versions of the lesson files, which requires converting `.md` to `.html` as part of a build or deployment step.

## Adding a lesson

Each lesson file follows this naming convention:

```
<category>/YYYY-MM-DD.md
```

To add a day manually:

1. Create `rhetoric/YYYY-MM-DD.md` following the structure in existing files.
2. Create `cognitive/YYYY-MM-DD.md` following the structure in existing files.
3. Add the corresponding links to `index.html`.
4. Commit and push.

## CI

A GitHub Actions workflow at `.github/workflows/ci.yml` runs on push and pull request to `main`/`master`. It detects Node or PHP projects and runs the appropriate install and test steps.

## Contributing

This is a personal learning repository. Corrections to factual errors in lesson content (wrong definition of a rhetorical device, incorrect exercise instructions) are welcome via pull request.

See `CONTRIBUTING.md` for guidelines.

## License

MIT. See `LICENSE`.
