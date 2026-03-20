---
title: Odoo 16 — Sửa lệch báo cáo Kế toán Localization Việt Nam
status: in-progress
priority: P1
effort: high
branch: main
tags: [odoo16, enterprise, l10n_vn, accounting-reports]
created: 2026-03-20
updated: 2026-03-20
---

# Plan: Báo cáo kế toán VN — nhất quán tháng / quý / năm

## Mục tiêu

Rà soát nguyên nhân lệch số giữa lọc kỳ, refactor logic, test + dữ liệu giả lập, nghiệm thu có chữ ký.

## Tiến độ tổng quan

| Phase | File | Mô tả |
|-------|------|--------|
| 0 | [phase-00-pre-bid.md](./phase-00-pre-bid.md) | Pre-bid, khảo sát, proposal M1 |
| 1 | [phase-01-m1-discovery.md](./phase-01-m1-discovery.md) | M1 Discovery |
| 2 | [phase-02-m2-design.md](./phase-02-m2-design.md) | M2 Thiết kế |
| 3 | [phase-03-m3-build.md](./phase-03-m3-build.md) | M3 Build |
| 4 | [phase-04-m4-uat.md](./phase-04-m4-uat.md) | M4 UAT |
| 5 | [phase-05-m5-handover.md](./phase-05-m5-handover.md) | M5 Bàn giao |

**Cách dùng:** đánh dấu `[x]` khi xong từng task trong từng file phase; cập nhật `status` ở frontmatter file này khi đóng phase (`pending` → `in-progress` → `completed`).

## Liên kết tài liệu

- [docs/project-overview-pdr.md](../../docs/project-overview-pdr.md)
- [docs/khao-sat-khach-hang.md](../../docs/khao-sat-khach-hang.md)
