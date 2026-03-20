# Project Roadmap

## Pre-bid / Trước khi báo giá trọn gói

| Bước | Việc | Kết quả |
|------|------|---------|
| 1 | Gửi [khao-sat-khach-hang.md](./khao-sat-khach-hang.md) + xin 1 ví dụ lệch (export/PDF) | Yêu cầu rõ ràng |
| 2 | Họp 30–45’: định nghĩa nghiệm thu + phạm vi báo cáo | Biên bản ngắn |
| 3 | Xác nhận quyền truy cập: dev/staging, Git/module, DB mẫu ẩn danh | Checklist |
| 4 | Proposal: **Milestone 1 có giá cố định**; M2/M3 sau M1 | Giảm rủi ro |

**Nguyên tắc:** Không cam kết giá cố định cho toàn bộ báo cáo VN trước khi có kết quả M1.

## Milestones sau ký hợp đồng

| ID | Tên | Nội dung chính | Deliverable |
|----|-----|----------------|-------------|
| **M1** | Discovery | Tái hiện lỗi, trace domain/date/initial balance, đọc code report | Báo cáo KT 5–15 trang, danh sách file/hàm |
| **M2** | Thiết kế | Chuẩn hóa “resolve kỳ”, ranh giới refactor vs patch | Mini design 2–4 trang + estimate M3 |
| **M3** | Build | Refactor, test tự động, data demo | PR / version module, test pass |
| **M4** | UAT | Chạy với khách trên staging, đối chiếu số | Biên bản nghiệm thu |
| **M5** | Handover | Ghi chú upgrade, rủi ro, vận hành | Tài liệu bàn giao |

## Ma trận “đủ điều kiện báo giá full”

| Hạng mục | Bắt buộc trước giá trọn gói? |
|----------|------------------------------|
| Ví dụ số lệch cụ thể | Có — nếu không chỉ báo giá M1 |
| DB tái hiện được | Có |
| Danh sách báo cáo trong scope | Nên có |
| Định nghĩa khớp tháng–quý đã ký | Có (trước code sâu) |
| Source module custom | Có nếu lỗi nằm ở custom |

## Ước lượng tham khảo (phụ thuộc mức độ sau M1)

- M1: ~3–7 ngày làm việc (có mã + DB mẫu).
- M2–M3: ~1.5–6+ tuần tùy số báo cáo và độ phức tạp custom.
