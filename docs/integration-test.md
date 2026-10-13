# GitHub Integration Test Specification

**Document ID:** KRY-GH-TEST-001  
**Status:** Draft  
**Owner:** Kryterea Integration Test  
**Version:** 1.0

## 1. Objective

Verify that a Kryterea project can access permitted files in a connected GitHub repository and recognize subsequent changes.

## 2. Sample requirements

| ID | Requirement | Acceptance criterion |
| --- | --- | --- |
| GH-001 | Discover repository documentation. | All three Markdown files are listed with their paths. |
| GH-002 | Read Markdown content. | Headings, tables, and links remain understandable. |
| GH-003 | Detect committed updates. | A changed document is visible after synchronization. |
| GH-004 | Respect disabled connections. | New GitHub access is blocked while the connection is disabled. |

## 3. Test procedure

1. Connect GitHub through Kryterea settings.
2. Associate this repository with a Kryterea project.
3. Locate this document at `docs/integration-test.md`.
4. Inspect requirements `GH-001` through `GH-004`.
5. Change the value of **Version** to `1.1` and commit to GitHub.
6. Trigger or await the supported synchronization process.
7. Confirm Kryterea displays the updated version and correct source path.

## 4. Evidence to capture

- Repository and branch selected.
- File path and commit identifier.
- Time of synchronization.
- Observed result for each requirement.
- Error details if a step fails.

## 5. Result

**Execution status:** Not run  
**Observed version:** Pending  
**Notes:** Complete after testing.

Return to the [documentation index](README.md).
