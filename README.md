# Web Projects Tracker

> Personal documentation system for tracking user stories, features, and ideas across multiple web projects.

## Projects Overview

| Project | Status | Features | Last Updated |
|---------|--------|----------|--------------|
| [Example Project](./example-project/) | Active | 3 planned, 1 in progress, 1 done | 2026-03-02 |
| [Den Perfekta Mackan](./den-perfekta-mackan/) | Kritisk fas | 3 planned, 1 in progress, 1 done | 2026-03-02 |

## Quick Start

### Adding a New Project
1. Create a new folder: `mkdir project-name`
2. Copy the templates:
   ```
   cp _templates/project-template.md project-name/README.md
   cp _templates/feature-template.md project-name/features.md
   ```
3. Fill in your project details (replace all `<!-- ... -->` comments)
4. Add the project to the table above

### Adding a New Feature
1. Open the project's `features.md`
2. Add the feature under the appropriate status section
3. Fill in all fields: priority, owner, effort, created date, dependencies, details, acceptance criteria
4. Update the feature counts in the project's `README.md`

### Moving a Feature Between Statuses
1. Cut the feature block from its current section
2. Paste it into the target section
3. Update `Updated:` date (or add `Completed:` / `Cancelled:` date)
4. Update feature counts in the project `README.md` and in the table above

### Using with GitHub Copilot / AI Assistants
- "Add a feature to example-project: OAuth login via Google"
- "Move the User Authentication feature in example-project to Done, completed today"
- "Create a new project called my-portfolio"

## Structure

```
cli-docs/
├── README.md                    # This file — master index
├── .gitignore                   # Ignore logs, secrets, editor files
├── _templates/                  # Templates for new projects
│   ├── project-template.md      # Copy this for a new project README
│   └── feature-template.md      # Copy this for a new project features file
└── [project-folders]/           # One folder per project
    ├── README.md                # Project overview and feature summary
    └── features.md              # Detailed feature tracking
```

## Workflow Guidelines

- **Branching:** Use feature branches (`feat/feature-name`) and merge via PR
- **Commit style:** Imperative present tense — "Add login page", not "Added login page"
- **Updates:** Update `Last Updated` in the table above whenever you touch a project
- **Reviews:** Do a weekly pass to catch stale in-progress items

## Status Legend

| Emoji | Status | Meaning |
|-------|--------|---------|
| 📋 | Planned | Identified, not started |
| 🚧 | In Progress | Currently being worked on |
| ✅ | Done | Completed and deployed |
| ❌ | Cancelled | No longer pursuing |

## Effort Legend

| Size | Meaning |
|------|---------|
| S | Hours |
| M | 1–3 days |
| L | 1–2 weeks |
| XL | Weeks+ |
