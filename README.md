# Multi-Agent Development Plugin for Antigravity

Autonomous multi-agent development plugin featuring an orchestrator coordinating planner, developer, tester, DevOps engineer, security auditor, technical writer, data engineer, and UI tester agents under a strict token-optimized communication protocol.

## Roster
- **orchestrator**: Master coordinator spawned as a subagent to manage project lifecycle, dispatch DAG tasks in parallel, sandbox workspaces, and handle rollback guards.
- **planner**: Interactive "Grill Me" architecture and structured implementation planner with DAG dependency tracking.
- **developer**: Minimal diff implementation specialist focusing on clean, idiomatic changes, atomic git commits, and local sanity checks.
- **tester**: QA engineer and code reviewer enforcing test passes and lint review before task completion (strictly scoped to test files).
- **devops-engineer**: On-demand specialist managing Dockerfiles, Compose setups, and container deployment.
- **security-auditor**: On-demand specialist auditing CVEs, secrets, and OWASP compliance.
- **tech-writer**: On-demand specialist generating OpenAPI schemas, ADRs, and documentation.
- **data-engineer**: On-demand specialist handling database migrations, SQL query tuning, ORM models, seed scripts, and rollback strategies.
- **ui-tester**: On-demand specialist executing headless browser tests (Playwright/Puppeteer), DOM assertions, and UI regression checks.

## Key Capabilities
- **Workspace Sandboxing**: Developers operate in isolated branches (`Workspace: branch`) or worktrees, merging only upon tester PASS verdict.
- **Parallel DAG Dispatch**: Orchestrator parses `DEPENDS_ON` task metadata to run decoupled worker pairs concurrently.
- **Model-Tier Optimization**: Automated routing using `inherit`/`pro` for heavy architectural and dev work, and `flash` for fast audit, doc, and test passes.
- **Rollback Guard**: Automatic reset and dirty-tree eviction upon retry exhaustion to prevent corrupting the main working tree.
- **Strict Authoring Boundaries**: Planners write only plan specs; testers write only test suites; developers handle source code changes.

## Installation
Install or clone into your Antigravity plugins directory:
```bash
agy plugin install multiagent
# or clone into ~/.gemini/config/plugins/multiagent
```
