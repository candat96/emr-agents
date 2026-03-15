# Tích hợp Claude Code — EMR Agents

Các agent EMR hoạt động trực tiếp với Claude Code mà không cần chuyển đổi định dạng — format `.md` kết hợp YAML frontmatter chính là định dạng gốc của Claude Code.

## Cài đặt

```bash
# Sao chép tất cả agent EMR vào thư mục agents của Claude Code
cp emr-agent/*-emr.md ~/.claude/agents/
```

Hoặc cài đặt chọn lọc từng agent cụ thể:

```bash
# Chỉ cài Backend + Frontend Developer
cp emr-agent/backend-developer-emr.md ~/.claude/agents/
cp emr-agent/frontend-developer-emr.md ~/.claude/agents/
```

## Kích hoạt Agent

Trong bất kỳ phiên Claude Code nào, gọi agent theo tên:

```
Activate Backend Developer - EMR and help me implement the patient registration API.
```

```
Use the Code Reviewer - EMR agent to review this pull request.
```

```
Activate Integration Gateway - EMR and generate the QCVN 01 XML message builder.
```

## Cấu hình theo phạm vi dự án

Để các agent chỉ khả dụng trong dự án EMR của bạn:

```bash
# Từ thư mục gốc dự án EMR
mkdir -p .claude/agents
cp /path/to/agency-agents/emr-agent/*-emr.md .claude/agents/
```

## Tích hợp CLAUDE.md

Thêm vào file `CLAUDE.md` của dự án để cung cấp ngữ cảnh cho Claude Code:

```markdown
# Dự án EMR SaaS

## Công nghệ sử dụng
- Backend: NestJS + TypeScript + TypeORM
- Frontend: Next.js + React + TypeScript + Tailwind + shadcn/ui
- Cơ sở dữ liệu: PostgreSQL (theo từng tenant) + Redis + Elasticsearch
- Xác thực: Keycloak (OIDC) — 1 realm mỗi tenant
- Hàng đợi tin nhắn: Kafka
- Tiêu chuẩn: HL7 FHIR R4, ICD-10, LOINC, SNOMED CT
- Tuân thủ: QCVN 01-04:2025/BYT, NĐ 13/2023, TT 46/2018

## Thư mục Agent
Xem `.claude/agents/` để tìm các agent EMR chuyên biệt.
```

## Danh sách Agent

| Agent | File | Mục đích sử dụng |
|-------|------|-------------------|
| Phân tích nghiệp vụ | `business-analyst-emr.md` | Yêu cầu, user story, quy trình lâm sàng |
| Thiết kế UI/UX | `uiux-designer-emr.md` | Hệ thống thiết kế y tế, đặc tả giao diện lâm sàng |
| Lập trình Backend | `backend-developer-emr.md` | API NestJS, đa tenant, FHIR, Keycloak |
| Lập trình Frontend | `frontend-developer-emr.md` | Giao diện lâm sàng Next.js, trợ năng, thời gian thực |
| Kiểm thử QA | `qa-engineer-emr.md` | Kiểm thử an toàn bệnh nhân, cô lập tenant, SSO |
| Kỹ sư DevOps | `devops-engineer-emr.md` | K8s, Helm, CI/CD, VPC, giám sát |
| Quản lý dự án | `project-manager-emr.md` | Lập kế hoạch sprint, chiến lược go-live, quản lý rủi ro |
| Trưởng nhóm kỹ thuật | `tech-lead-emr.md` | Quyết định kiến trúc, ADR, tiêu chuẩn mã nguồn |
| Đánh giá mã nguồn | `code-reviewer-emr.md` | Review PR, kiểm tra an toàn bệnh nhân, audit bảo mật |
| Cổng tích hợp | `integration-gateway-emr.md` | Tuân thủ QCVN, BHXH, VNeID, CSDL quốc gia |
