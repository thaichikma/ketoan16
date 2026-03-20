# Phase 3 — M3 Build

**Mục tiêu:** implement refactor, test tự động, dữ liệu demo; toàn bộ test trong scope **pass**.

## Implementation

- [ ] Tạo nhánh `feature/vn-report-period-consistency` (hoặc tên đã chốt)
- [ ] Implement **period resolver** + thay thế dần các nhánh date trùng lặp
- [ ] Refactor báo cáo theo danh sách M2; **comment** logic nghiệp vụ VN / FY không hiển nhiên
- [ ] Chạy linter/format theo chuẩn dự án (nếu có)
- [ ] Self-review: diff không chứa thay đổi ngoài phạm vi

## Test & dữ liệu

- [ ] Thêm `tests/` — `TransactionCase` (hoặc pattern Odoo 16 tương đương) cho từng nhóm báo cáo trong scope
- [ ] Tạo **dữ liệu giả lập**: XML/Python — biên thời gian, nhiều kỳ, giáp năm
- [ ] Chạy `odoo-bin` với `--test-enable` (hoặc CI) — **0 fail**
- [ ] Ghi lệnh chạy test vào README module hoặc `docs/deployment-guide.md`

## Pull request

- [ ] Mô tả PR: nguyên nhân, cách sửa, ảnh hưởng, hướng dẫn upgrade `-u`
- [ ] Peer review (nếu có team)
- [ ] Merge vào branch staging theo quy trình khách

## Definition of done

- [ ] CI / test local pass 100% phạm vi
- [ ] PR merged vào nhánh deploy staging (hoặc module nâng version trên staging)
