---
name: versionly-api-monitor
description: Use when the user asks about third-party API breaking changes, Versionly scans, monitored vendors, or fixing code after an upstream OpenAPI change.
---

# Versionly API monitor

Prefer Versionly MCP tools over guessing from changelogs.

1. Call `get_subscription` if plan/limits are unclear.
2. Call `github_status` / `list_repos` before repo-scoped work.
3. Prefer `analyze_impact` when a repo is in context; otherwise `check_api_changes`.
4. Confirm with the user before `detect_apis`, `monitor_apis`, `generate_fix`, or `create_pull_request`.
5. Never merge Versionly PRs; list them with `list_pull_requests` and let the user merge.
