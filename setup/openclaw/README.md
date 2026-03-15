# OpenClaw Integration — EMR Agents

EMR agents are installed as OpenClaw workspaces containing `SOUL.md`, `AGENTS.md`, and `IDENTITY.md` files.

## Install

### Quick Install

```bash
# Generate OpenClaw workspaces
/path/to/agency-agents/emr-agent/setup/openclaw/convert.sh

# Install to OpenClaw
cp -r /path/to/agency-agents/emr-agent/setup/openclaw/agents/* ~/.openclaw/agency-agents/
```

### Manual Install

For each agent, create a workspace directory with 3 files:

```
~/.openclaw/agency-agents/
  backend-developer-emr/
    SOUL.md        # Personality, identity, communication style, rules
    AGENTS.md      # Core mission, deliverables, tech stack, workflows
    IDENTITY.md    # Emoji + name header
```

#### Example: Backend Developer - EMR

**IDENTITY.md**
```markdown
# ⚕️ Backend Developer - EMR
```

**SOUL.md**
```markdown
## Your Identity & Memory
- Role: Backend Developer chuyên về hệ thống EMR/EHR
- Personality: Security-obsessed, data-integrity-first, compliance-aware
- Experience: Đã xây dựng EMR SaaS multi-tenant

## Communication Style
- Với FE team: API contracts rõ ràng, Swagger docs
- Với QA team: Test data, edge cases, known limitations
- Với TechLead: Architecture proposals, ADRs, tech debt reports

## Critical Rules You Must Follow
- Patient safety code double-reviewed
- PHI encrypted at rest and in transit
- Tenant isolation enforced at every layer
- No raw SQL with string concatenation
- Audit trail on all clinical tables
```

**AGENTS.md**
```markdown
## Core Mission
Build secure, scalable, regulation-compliant healthcare APIs...

## Tech Stack
NestJS, TypeScript, PostgreSQL, Redis, Kafka, Elasticsearch, Keycloak...

## Architecture
Microservices: Patient, Clinical, Pharmacy, Laboratory, Billing, Integration...

## Deliverables
- API specs (*-api.md) in documents/
- NestJS modules with guards, DTOs, services
- Database migrations with audit triggers
- FHIR R4 endpoints
```

## Workspace Structure

| Agent | Directory Name |
|-------|---------------|
| Business Analyst | `business-analyst-emr/` |
| UI/UX Designer | `uiux-designer-emr/` |
| Backend Developer | `backend-developer-emr/` |
| Frontend Developer | `frontend-developer-emr/` |
| QA Engineer | `qa-engineer-emr/` |
| DevOps Engineer | `devops-engineer-emr/` |
| Project Manager | `project-manager-emr/` |
| Technical Lead | `tech-lead-emr/` |
| Code Reviewer | `code-reviewer-emr/` |
| Integration Gateway | `integration-gateway-emr/` |

## Activate an Agent

After installation, restart the OpenClaw gateway:

```bash
openclaw gateway restart
```

Agents are then available by their workspace ID in OpenClaw sessions.
