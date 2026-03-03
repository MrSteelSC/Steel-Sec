# AGENTS.md

## Cursor Cloud specific instructions

This is a **pure documentation repository** (cybersecurity knowledge-base). There is no application code, no build system, no automated tests, and no runtime services.

### Repository structure

- `ir/` — Incident response playbooks & checklists
- `pentest/` — Nmap profiles & pentest notes
- `dfir/` — Forensic acquisition notes
- `resources/` — Cheat sheets & quick references

All content is Markdown (`.md`) files plus a logo image. See `README.md` for the full table of contents.

### Linting

Run markdown lint on all files:

```sh
markdownlint-cli2 "**/*.md"
```

The repo currently has pre-existing lint warnings (189 as of initial setup). These are stylistic issues in the existing docs, not introduced by agent changes.

### Local preview

Serve GitHub-flavored Markdown preview locally with `grip`:

```sh
grip README.md 0.0.0.0:8080
```

Then open `http://localhost:8080/` in a browser. Internal links between docs work via grip's file serving. `grip` requires network access for GitHub's rendering API on first load; it falls back to local rendering if offline.

### No build / test / deploy steps

There is nothing to build, no automated tests to run, and no deployment pipeline. Contributions are purely edits to `.md` files.
