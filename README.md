# Multi-Agent Development Plugin for Antigravity

Autonomous multi-agent development plugin featuring an orchestrator coordinating planner, developer, tester, DevOps engineer, security auditor, and technical writer agents under a strict token-optimized communication protocol.

## Roster
- **orchestrator**: Master coordinator spawned as a subagent to manage lifecycle and dispatch tasks.
- **planner**: Interactive "Grill Me" architecture and structured implementation planner.
- **developer**: Minimal diff implementation specialist focusing on clean, idiomatic changes.
- **tester**: QA engineer and code reviewer enforcing test passes before task completion.
- **devops-engineer**: On-demand specialist managing Dockerfiles, Compose setups, and container deployment.
- **security-auditor**: On-demand specialist auditing CVEs, secrets, and OWASP compliance.
- **tech-writer**: On-demand specialist generating OpenAPI schemas, ADRs, and documentation.

## Installation
Install or clone into your Antigravity plugins directory:
```bash
agy plugin install multiagent
# or clone into ~/.gemini/config/plugins/multiagent
```
