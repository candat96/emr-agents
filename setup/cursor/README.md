# Cursor Integration — EMR Agents

Converts EMR agents into Cursor `.mdc` rule files. Rules are **project-scoped** — install them from your EMR project root.

## Install

### Quick Install (Script)

```bash
# From your EMR project root
cd /your/emr-project
/path/to/agency-agents/emr-agent/setup/cursor/install.sh
```

### Manual Install

```bash
# From your EMR project root
mkdir -p .cursor/rules

# Copy and convert each agent
for agent in /path/to/agency-agents/emr-agent/*-emr.md; do
  slug=$(basename "$agent" .md)
  # Strip YAML frontmatter, add Cursor frontmatter
  sed '1{/^---$/!q;};1,/^---$/d' "$agent" > ".cursor/rules/${slug}.mdc"
done
```

Or manually create `.mdc` files — example for Backend Developer:

```yaml
---
description: Senior Backend Developer specializing in EMR/EHR systems. Expert in NestJS, PostgreSQL, microservices, multi-tenant SaaS, HL7 FHIR, ICD-10, LOINC, and Vietnam healthcare compliance.
globs: "src/**/*.ts,src/**/*.module.ts,src/**/*.service.ts,src/**/*.controller.ts"
alwaysApply: false
---

# Backend Developer - EMR Agent Personality
...
```

## Recommended Glob Patterns

| Agent | Suggested Globs |
|-------|----------------|
| Backend Developer | `src/**/*.ts,src/**/*.module.ts,src/**/*.service.ts,src/**/*.controller.ts` |
| Frontend Developer | `src/**/*.tsx,src/**/*.ts,src/components/**/*,src/app/**/*` |
| UI/UX Designer | `src/components/**/*.tsx,src/styles/**/*,tailwind.config.*` |
| DevOps Engineer | `Dockerfile,docker-compose.*,helm/**/*,k8s/**/*,.gitlab-ci.yml,terraform/**/*` |
| QA Engineer | `**/*.spec.ts,**/*.test.ts,**/*.e2e-spec.ts,playwright/**/*` |
| Code Reviewer | `**/*.ts,**/*.tsx` |
| Integration Gateway | `src/integration/**/*,src/gateway/**/*,**/*.xsd,**/*.xml` |
| Business Analyst | `documents/**/*.md,feature.md` |
| Project Manager | `documents/00-*` |
| Technical Lead | `documents/00-adr/**/*,documents/00-architecture*` |

## Activate a Rule

In Cursor, reference an agent in your prompt:

```
@backend-developer-emr Build the patient registration API with FHIR R4 support.
```

Or enable as always-on by setting `alwaysApply: true` in the frontmatter:

```yaml
---
description: ...
globs: "src/**/*.ts"
alwaysApply: true
---
```

## Always-On Recommendations

For an EMR project, consider setting these as `alwaysApply: true`:
- **Code Reviewer** — Always enforce patient safety and security checks
- **Technical Lead** — Always enforce architecture standards
