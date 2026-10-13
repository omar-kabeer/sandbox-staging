# Kryterea GitHub Integration Test

A lightweight repository for testing Kryterea's GitHub integration against real Markdown files.

## Purpose

Use this repository to verify that Kryterea can connect to GitHub, discover repository content, read documentation, and detect changes without modifying production code or documents.

## Repository structure

```text
.
├── README.md
└── docs/
    ├── README.md
    └── integration-test.md
```

## Test workflow

1. Connect your GitHub account in Kryterea settings.
2. Select this repository from a Kryterea project.
3. Verify Kryterea discovers both README files and `docs/integration-test.md`.
4. Open or import the documentation and check that headings, lists, and relative links remain intact.
5. Edit `docs/integration-test.md` on GitHub and commit the change.
6. Refresh or resynchronize the connection in Kryterea, then confirm the updated content appears.
7. Disable the GitHub connection in settings and verify Kryterea respects the disabled state.
8. Re-enable it and confirm the repository can be accessed again.

## Expected outcome

The integration identifies the correct repository and file paths, respects connection permissions, preserves Markdown content, and reflects committed changes when synchronization runs.

> This repository contains synthetic test content only. Do not add credentials, tokens, or sensitive information.

See [docs/README.md](docs/README.md) for the documentation index.
