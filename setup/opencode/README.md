# OpenCode Integration — EMR Agents

OpenCode agents are `.md` files with YAML frontmatter stored in `.opencode/agents/`. Agents are invoked on-demand via `@agent-name`.

## Install

### Project-Scoped (Recommended)

```bash
# From your EMR project root
mkdir -p .opencode/agents

# Copy agents with color conversion (named → hex)
for agent in /path/to/agency-agents/emr-agent/*-emr.md; do
  slug=$(basename "$agent" .md)
  cp "$agent" ".opencode/agents/${slug}.md"
done
```

Then update each file's frontmatter to add `mode: subagent` and convert colors to hex:

```yaml
---
name: Backend Developer - EMR
description: Senior Backend Developer specializing in EMR/EHR systems...
mode: subagent
color: "#3498DB"
---
```

### Global Install

```bash
mkdir -p ~/.config/opencode/agents
cp /path/to/agency-agents/emr-agent/*-emr.md ~/.config/opencode/agents/
```

## Color Mapping

| Agent Color (source) | Hex Code |
|---------------------|----------|
| blue | `#3498DB` |
| cyan | `#00FFFF` |
| green | `#2ECC71` |
| red | `#E74C3C` |
| purple | `#9B59B6` |
| orange | `#F39C12` |

## Activate an Agent

In OpenCode, invoke a subagent with `@`:

```
@backend-developer-emr Help me implement the FHIR Patient resource endpoint.
```

```
@code-reviewer-emr Review the prescription module for patient safety issues.
```

```
@integration-gateway-emr Generate the QCVN 01 XML builder for BA-01 records.
```

## Available Agents

| Agent | Slug | Color |
|-------|------|-------|
| Business Analyst | `@business-analyst-emr` | `#3498DB` |
| UI/UX Designer | `@uiux-designer-emr` | `#9B59B6` |
| Backend Developer | `@backend-developer-emr` | `#3498DB` |
| Frontend Developer | `@frontend-developer-emr` | `#00FFFF` |
| QA Engineer | `@qa-engineer-emr` | `#2ECC71` |
| DevOps Engineer | `@devops-engineer-emr` | `#F39C12` |
| Project Manager | `@project-manager-emr` | `#3498DB` |
| Technical Lead | `@tech-lead-emr` | `#E74C3C` |
| Code Reviewer | `@code-reviewer-emr` | `#9B59B6` |
| Integration Gateway | `@integration-gateway-emr` | `#F39C12` |
