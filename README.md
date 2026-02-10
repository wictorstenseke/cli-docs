# Web Projects Tracker

> Personal documentation system for tracking user stories, features, and ideas across multiple web projects.

## 📊 Projects Overview

| Project | Status | Features | Last Updated |
|---------|--------|----------|--------------|
| [Example Project](./example-project/) | Active | 3 planned, 1 in progress | 2026-01-23 |

## 🚀 Quick Start

### Adding a New Project
1. Create a new folder: `mkdir project-name`
2. Copy templates: `cp _templates/project-template.md project-name/README.md`
3. Copy templates: `cp _templates/feature-template.md project-name/features.md`
4. Edit the files with your project details
5. Add the project to the table above

### Adding a New Feature
1. Navigate to the project's `features.md` file
2. Add the feature under the appropriate status section (Planned, In Progress, or Done)
3. Fill in the description, details, and notes

### Using with GitHub Copilot CLI
Simply tell Copilot which project and what feature to add:
- "Add a feature to example-project: user authentication"
- "Create a new project called my-portfolio"
- "Move the login feature in example-project to Done"

## 📁 Structure

```
cli-docs/
├── README.md                    # This file - master index
├── _templates/                  # Templates for new projects
│   ├── project-template.md      # Copy this for new projects
│   └── feature-template.md      # Format for feature tracking
└── [project-folders]/           # One folder per project
    ├── README.md                # Project overview
    └── features.md              # Feature tracking
```

## 💡 Tips

- Keep feature descriptions concise but clear
- Update the "Last Updated" column when you make changes
- Use emojis for quick visual scanning (✅ 🚧 📋 ❌)
- Archive old/cancelled features at the bottom of features.md
- Regular reviews help keep the tracker useful

## 🏷️ Status Legend

- 📋 **Planned**: Feature identified but not started
- 🚧 **In Progress**: Currently being worked on
- ✅ **Done**: Completed and deployed/implemented
- ❌ **Cancelled**: No longer pursuing this feature
