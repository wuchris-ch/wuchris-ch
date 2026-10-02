# I build AI developer tools and full-stack systems, and measure how well they work.

These are my public projects: a PR reviewer benchmarked against commercial tools, an evaluation platform for AI agents and a live macro research site. Most of my product work happens in private repositories.

## Selected work

### [PR Review & Regression Testing Platform](https://github.com/wuchris-ch/pr-review-agent-flue)
AI code review that cites exact changed lines, plus a self-hosted platform that proves a suspected bug with a failing test before proposing a fix. Runs as a CLI, GitHub Action or GitHub App.

- Scored on 50 public PRs from Sentry, Grafana, Keycloak, Discourse and Cal.com against 17 commercial reviewers, all re-scored by one judge: 52.4% precision on held-out PRs, 7th of 18.
- In a live run, reproduced 9 of 9 seeded regressions with failing tests. Every fix passed contract tests the agents never saw, and none of 9 valid changes was flagged.

**TypeScript · Python · Temporal · PostgreSQL · Docker**  
[Project site](https://wuchris-ch.github.io/pr-review-agent-flue/) · [Results and method](https://github.com/wuchris-ch/pr-review-agent-flue/blob/main/docs/results.md) · [Latest release](https://github.com/wuchris-ch/pr-review-agent-flue/releases/latest)

### [Agent Reliability & Evaluation Platform](https://github.com/wuchris-ch/agent-eval-platform)
Gates agent releases on repeated trials, checking outcomes with hidden tests and independent state checks instead of the agent's own report.

- Held back a PR reviewer release when 60 trials across 20 cases showed 85.7% security-blocker recall, then traced the misses to citation-line mismatches and a swallowed error.

**Python · Kubernetes (K3s) · PostgreSQL · OpenTelemetry · React**  
[Evidence explorer](https://wuchris-ch.github.io/agent-eval-platform/) · [Architecture](https://wuchris-ch.github.io/agent-eval-platform/architecture.html)

### [Global Macro Research Workbench](https://github.com/wuchris-ch/global-liquidity-credit-tracker)
A live research site that refreshes FRED, BIS, World Bank, NY Fed and market data every 12 hours. It stores immutable source captures, so historical analyses use only data that was available at the time.

**Next.js · TypeScript · Python · FastAPI · DuckDB**  
[Open application](https://global-liquidity-credit-tracker.vercel.app/) · [Release laboratory](https://global-liquidity-credit-tracker.vercel.app/research/lab)

---

More work: [Multi-agent development workflows](https://github.com/wuchris-ch/multi-agent-software-development-platform) · [Coding-agent evaluation harness](https://github.com/wuchris-ch/deepswe-claude-code-eval) · [Distributed task scheduler in Go](https://github.com/wuchris-ch/distributed-task-scheduler) · [Local email classification](https://github.com/wuchris-ch/ollama-email-classifier)
