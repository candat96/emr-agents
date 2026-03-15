# Claude Code Integration — EMR Agents

EMR agents work natively with Claude Code. No conversion needed — the `.md` + YAML frontmatter format is Claude Code's native format.

## Install

```bash
# Copy all EMR agents to Claude Code agents directory
cp emr-agent/*-emr.md ~/.claude/agents/
```

Or selectively install specific agents:

```bash
# Only backend + frontend developers
cp emr-agent/backend-developer-emr.md ~/.claude/agents/
cp emr-agent/frontend-developer-emr.md ~/.claude/agents/
```

## Activate an Agent

In any Claude Code session, reference an agent by name:

```
Activate Backend Developer - EMR and help me implement the patient registration API.
```

```
Use the Code Reviewer - EMR agent to review this pull request.
```

```
Activate Integration Gateway - EMR and generate the QCVN 01 XML message builder.
```

## Project-Scoped Setup

To make agents available only within your EMR project:

```bash
# From your EMR project root
mkdir -p .claude/agents
cp /path/to/agency-agents/emr-agent/*-emr.md .claude/agents/
```

## CLAUDE.md Integration

Add to your project's `CLAUDE.md` to give Claude Code project context:

```markdown
# EMR SaaS Project

## Tech Stack
- Backend: NestJS + TypeScript + TypeORM
- Frontend: Next.js + React + TypeScript + Tailwind + shadcn/ui
- Database: PostgreSQL (per-tenant) + Redis + Elasticsearch
- Auth: Keycloak (OIDC) — 1 realm per tenant
- Messaging: Kafka
- Standards: HL7 FHIR R4, ICD-10, LOINC, SNOMED CT
- Compliance: QCVN 01-04:2025/BYT, NĐ 13/2023, TT 46/2018

## Agent Directory
See `.claude/agents/` for specialized EMR agents.
```

## Available Agents

| Agent | File | Use For |
|-------|------|---------|
| Business Analyst | `business-analyst-emr.md` | Requirements, user stories, clinical workflows |
| UI/UX Designer | `uiux-designer-emr.md` | Healthcare design system, clinical UI specs |
| Backend Developer | `backend-developer-emr.md` | NestJS APIs, multi-tenant, FHIR, Keycloak |
| Frontend Developer | `frontend-developer-emr.md` | Next.js clinical UI, accessibility, real-time |
| QA Engineer | `qa-engineer-emr.md` | Patient safety testing, tenant isolation, SSO tests |
| DevOps Engineer | `devops-engineer-emr.md` | K8s, Helm, CI/CD, VPC, monitoring |
| Project Manager | `project-manager-emr.md` | Sprint planning, go-live strategy, risk management |
| Technical Lead | `tech-lead-emr.md` | Architecture decisions, ADRs, code standards |
| Code Reviewer | `code-reviewer-emr.md` | PR review, patient safety checks, security audit |
| Integration Gateway | `integration-gateway-emr.md` | QCVN compliance, BHXH, VNeID, national DB |
