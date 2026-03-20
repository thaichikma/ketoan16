# Phase 2 — M2 Thiết kế

**Mục tiêu:** thiết kế **một luồng chuẩn hóa kỳ** + ranh giới refactor; tránh scope creep.

## Thiết kế

- [ ] Đặc tả API/hàm **resolve_report_period** (input: company, mode, kỳ; output: date_from, date_to, flags)
- [ ] Quyết định: **tách** lớp lấy số vs map dòng báo cáo VN; sơ đồ luồng (text hoặc mermaid)
- [ ] Liệt kê **các báo cáo / dòng** chịu ảnh hưởng; đánh dấu “bắt buộc refactor” vs “chỉ điều chỉnh domain”
- [ ] Chiến lược **backward compatibility**: upgrade module, không phá dữ liệu hiện có
- [ ] Cập nhật [docs/system-architecture.md](../../docs/system-architecture.md) nếu quyết định kiến trúc đã chốt

## Test strategy

- [ ] Ma trận test: tháng vs quý vs năm + biên ngày (đầu/cuối tháng, quý, 31/12–01/01)
- [ ] Quy ước assert: tổng 3 tháng == quý (hoặc quy tắc snapshot đã ký)

## Ước lượng & ký duyệt

- [ ] Breakdown M3: task + estimate (ngày)
- [ ] Gửi mini design (2–4 trang) + estimate; **chữ ký / email chấp thuận** khách trước code lớn

## Definition of done

- [ ] Design + estimate được chấp thuận
- [ ] Branch/feature branch tên rõ (ghi trong plan frontmatter nếu cần)
