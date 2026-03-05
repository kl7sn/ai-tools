# AI-Tools

A curated collection of rules and skills for AI-assisted development workflows in Cursor IDE.

## What's Inside

### Rules (`rules/`)

Cursor rules (`.mdc`) that are always applied to AI interactions in this project.

- **git-commit.mdc** — Git commit message specification based on the [Angular commit-message-format](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format). Enforces structured commit messages with type, scope, JIRA key, and summary. Designed to work with GitLab server-side `pre-receive` hooks.

- **riper5.mdc** — The RIPER-5 protocol for structured AI interaction. Defines five sequential modes — Research, Innovate, Plan, Execute, Review — to prevent unauthorized code modifications and ensure disciplined, traceable development with AI agents.

### Skills (`skills/`)

References to external AI agent skills.

- **pensieve.md** — [Pensieve](https://github.com/kingkongshot/Pensieve) marketplace install reference. A project-level knowledge base that captures decisions, maxims, knowledge, and pipelines across development sessions.

## Usage

Clone this repository and open it in [Cursor](https://cursor.com). The `.mdc` rules under `rules/` will be automatically applied to all AI conversations in the workspace.

```bash
git clone https://github.com/kl7sn/ai-tools.git
cd ai-tools
```

To add new rules, create a `.mdc` file in the `rules/` directory with the following frontmatter:

```yaml
---
alwaysApply: true
---
```

## License

[MIT](LICENSE)
