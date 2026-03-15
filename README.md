# EMR SaaS — AI Agent Team

A complete set of **10 specialized AI agents** for building a multi-tenant Electronic Medical Record (EMR) SaaS platform compliant with Vietnamese healthcare regulations and international standards.

## The Team

| # | Agent | Emoji | Role | Key Expertise |
|---|-------|-------|------|---------------|
| 1 | [Business Analyst](business-analyst-emr.md) | 📋 | Requirements & clinical workflows | 16 modules, ~535 features, VN + international healthcare standards |
| 2 | [UI/UX Designer](uiux-designer-emr.md) | 🎨 | Healthcare design system | Clinical alerts, patient safety UX, WCAG AA, design tokens |
| 3 | [Backend Developer](backend-developer-emr.md) | ⚕️ | API & microservices | NestJS, multi-tenant DB, FHIR R4, Keycloak SSO, RBAC |
| 4 | [Frontend Developer](frontend-developer-emr.md) | 💻 | Clinical UI | Next.js, React, NextAuth.js + Keycloak, real-time WebSocket |
| 5 | [QA Engineer](qa-engineer-emr.md) | 🧪 | Testing & validation | Patient safety tests, tenant isolation, SSO/RBAC, FHIR conformance |
| 6 | [DevOps Engineer](devops-engineer-emr.md) | 🚀 | Infrastructure & CI/CD | K8s, Helm, Terraform, VPC 3-tier, GitLab CI/CD, Prometheus |
| 7 | [Project Manager](project-manager-emr.md) | 🧭 | Delivery & go-live | Phased rollout (6 phases), Scrum, change management for hospitals |
| 8 | [Technical Lead](tech-lead-emr.md) | 🏛️ | Architecture & quality | ADRs, code standards, cross-team coordination, tech debt |
| 9 | [Code Reviewer](code-reviewer-emr.md) | 🔍 | PR review & gatekeeper | Patient safety in code, security audit, tenant isolation checks |
| 10 | [Integration Gateway](integration-gateway-emr.md) | 🔗 | National data exchange | QCVN 01-04:2025/BYT, BHXH claims, VNeID, 137+ code tables |

## Tech Stack

```
Frontend:    Next.js + React + TypeScript + Tailwind + shadcn/ui
Backend:     NestJS + TypeScript + TypeORM
Database:    PostgreSQL (per-tenant) + Redis + Elasticsearch
Auth/SSO:    Keycloak (OIDC) — 1 realm per tenant
Messaging:   Kafka
Registry:    Harbor (harbor.emr.vn)
Infra:       Docker + Kubernetes + Terraform + GitLab CI/CD
Standards:   HL7 FHIR R4, ICD-10, LOINC, SNOMED CT
Integration: QCVN 01-04:2025/BYT, BHXH XML 4210, VNeID
Compliance:  NĐ 13/2023 (PDPD), NĐ 53/2022, TT 46/2018, TT 13/2025, HIPAA
```

## Architecture

```
Multi-Tenant SaaS: 1 Clinic = 1 PostgreSQL Database + 1 Keycloak Realm

┌─────────────────────────────────────────────────┐
│              Nginx Ingress (TLS 1.3)             │
│          *.emr.vn wildcard routing                │
└───────────────────────┬─────────────────────────┘
                        │
┌───────────────────────▼─────────────────────────┐
│               API Gateway (NestJS)               │
│         Rate Limit · Auth · Tenant Routing       │
└──┬──────┬──────┬──────┬──────┬──────┬──────┬────┘
   │      │      │      │      │      │      │
 Patient Clinical Pharmacy Lab  Billing Integration ...
 Service Service  Service Service Service Gateway
   │      │      │      │      │      │
   └──────┴──────┴──────┴──────┴──────┘
                  │
        PostgreSQL (per-tenant)
        Redis · Kafka · Elasticsearch
```

## Healthcare Standards & Compliance

### Vietnamese Regulations
| Standard | Description |
|----------|------------|
| QCVN 01:2025/BYT | EMR data exchange — 29 record types, 137+ code tables |
| QCVN 02:2025/BYT | Healthcare workforce data exchange |
| QCVN 03:2025/BYT | Pharmaceutical catalog data exchange |
| QCVN 04:2025/BYT | Medical device data exchange |
| TT 13/2025/TT-BYT | EMR implementation guidelines |
| TT 46/2018/TT-BYT | EMR regulations |
| NĐ 13/2023/NĐ-CP | Personal Data Protection Decree (PDPD) |
| NĐ 53/2022/NĐ-CP | Data localization |
| NĐ 102/2025/NĐ-CP | Health data management |
| QĐ 130/QĐ-BYT | BHXH insurance data output standards |

### International Standards
| Standard | Usage |
|----------|-------|
| HL7 FHIR R4 | Clinical data interoperability |
| ICD-10 | Diagnosis coding |
| LOINC | Lab test coding |
| SNOMED CT | Clinical terminology |
| ATC | Drug classification |
| DICOM | Medical imaging |
| HIPAA | Security framework reference |

## Project Structure

```
emr-agent/
├── README.md                          # This file
├── feature.md                         # 16 modules, ~535 features
├── business-analyst-emr.md            # BA agent
├── uiux-designer-emr.md              # UI/UX agent
├── backend-developer-emr.md           # Backend agent
├── frontend-developer-emr.md          # Frontend agent
├── qa-engineer-emr.md                 # QA agent
├── devops-engineer-emr.md             # DevOps agent
├── project-manager-emr.md            # PM agent
├── tech-lead-emr.md                   # Tech Lead agent
├── code-reviewer-emr.md              # Code Reviewer agent
├── integration-gateway-emr.md         # Integration Gateway agent
├── documents/                         # Shared documents (agents read/write here)
│   ├── QCVN_HSBADT_V1.0.docx        # QCVN 01:2025/BYT source
│   ├── 4.QCVN-Nhan luc y te*.docx   # QCVN 02:2025/BYT source
│   ├── 5.QCVN-Thuoc-Nhom4*.docx     # QCVN 03:2025/BYT source
│   ├── 6.QCVN-QLTBYT*.docx          # QCVN 04:2025/BYT source
│   └── 8.PHỤ LỤC E-*.docx           # Administrative division codes
└── setup/                             # IDE/tool integration guides
    ├── claude-code/README.md          # Claude Code setup
    ├── cursor/README.md               # Cursor setup
    ├── openclaw/README.md             # OpenClaw setup
    └── opencode/README.md             # OpenCode setup
```

## Document Flow

All agents collaborate through the `documents/` folder:

```
BA-EMR ─────→ documents/*.md (requirements)
                  │
         ┌───────┼───────┬───────────┐
         ▼       ▼       ▼           ▼
      UX-EMR  BE-EMR  FE-EMR    IG-EMR
      *-ux.md *-api.md *-fe.md  *-integration.md
         │       │       │           │
         └───────┼───────┘           │
                 ▼                   │
              QA-EMR                 │
              *-test.md              │
                 │                   │
                 ▼                   ▼
              DevOps-EMR      (National DBs)
              *-infra.md

TechLead-EMR ──→ 00-architecture*.md, 00-adr/, 00-coding-standards.md
PM-EMR ────────→ 00-project-plan.md, 00-risk-register.md
CR-EMR ────────→ PR review comments, escalations to TechLead
```

## IDE Setup

Choose your tool:

| Tool | Guide | Scope |
|------|-------|-------|
| [Claude Code](setup/claude-code/README.md) | Native `.md` format, no conversion | Global or project |
| [Cursor](setup/cursor/README.md) | Convert to `.mdc` rule files | Project-scoped |
| [OpenCode](setup/opencode/README.md) | Add `mode: subagent`, hex colors | Project or global |
| [OpenClaw](setup/openclaw/README.md) | Split into SOUL/AGENTS/IDENTITY | Global |

## Go-Live Phases

| Phase | Sprints | Duration | Modules |
|-------|---------|----------|---------|
| 0: Foundation | 1-4 | 2 months | Infra, design system, auth, CI/CD |
| 1: Core Clinical | 5-12 | 4 months | Patient, Appointments, EMR, Pharmacy |
| 2: Diagnostics & Billing | 13-18 | 3 months | Lab, Imaging, Billing/BHXH |
| 3: Extended | 19-24 | 3 months | Inventory, Reporting, Admin, Telemedicine |
| 4: Portal & Advanced | 25-30 | 3 months | Patient Portal, FHIR Gateway, Nursing, Surgery |
| 5: Pilot & Rollout | 31-36 | 3 months | Pilot, training, phased rollout |

## License

Part of [The Agency](https://github.com/tsanford01/agency-agents) — AI agent collection for software teams.
