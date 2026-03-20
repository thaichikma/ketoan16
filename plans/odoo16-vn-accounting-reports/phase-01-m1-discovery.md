# Phase 1 — M1 Discovery

**Mục tiêu:** tái hiện lỗi, xác định nguyên nhân gốc, phạm vi file/hàm; **không** refactor lớn trong phase này (trừ PoC nhỏ nếu cần chứng minh).

## Môi trường

- [ ] Clone / mở module trên staging hoặc local dev trùng version khách
- [ ] Restore DB mẫu; xác minh đăng nhập, company, FY, tiền tệ
- [ ] Liệt kê module `l10n_vn*` và custom liên quan (`pip list` / Apps nếu cần)

## Tái hiện

- [ ] Mở đúng báo cáo khách nêu; lặp lại **hai** cách lọc (tháng / quý) và ghi screenshot + số
- [ ] So sánh với ví dụ khách gửi — khớp mức “cùng lỗi”
- [ ] Thử thêm: lọc **năm**, **custom date range** (nếu trong phạm vi) để xem có nhánh khác lệch không

## Phân tích kỹ thuật

- [ ] Trace **date_from / date_to** (wizard, context, `account.report`) cho từng lọc
- [ ] Kiểm tra **initial balance / opening** có bị cộng trùng hoặc thiếu theo kỳ không
- [ ] Đối chiếu **fiscal year** vs calendar cho filter quý/tháng
- [ ] Ghi **domain** hoặc SQL/expression khác biệt giữa hai lần chạy (diff ngắn)
- [ ] Đọc code: đánh dấu file Python/XML, hàm, class có `if` theo period/month/quarter
- [ ] Phân loại: lỗi **date**, **công thức dòng**, **dữ liệu**, hay **hiểu nghiệp vụ**

## Báo cáo M1

- [ ] Viết báo cáo 5–15 trang (hoặc 1 doc ngắn + phụ lục): tóm tắt điều hành + chi tiết kỹ thuật
- [ ] Danh sách **nguyên nhân gốc** (có thể nhiều) + mức độ tin cậy
- [ ] **Phạm vi sửa** đề xuất + rủi ro + estimate **M2/M3** (ngày/tuần)
- [ ] Gửi khách; họp walkthrough 30–60’

## Definition of done

- [ ] Khách xác nhận đã đọc / đồng ý hướng xử lý (hoặc ghi nhận ý kiến chỉnh scope)
- [ ] Cập nhật [plan.md](./plan.md) nếu đổi status phase; tick task ở file này
