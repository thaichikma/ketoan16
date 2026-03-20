# Design Guidelines — Logic báo cáo

## Mục tiêu thiết kế

- **Nhất quán số liệu** giữa các granularity kỳ (tháng / quý / năm) khi định nghĩa nghiệp vụ là “cộng dồn phát sinh” hoặc khi so sánh snapshot đã thống nhất.
- **Dễ bảo trì:** developer mới đọc được luồng từ filter → số.

## Nguyên tắc

1. **Single source of truth** cho `(date_from, date_to, include_initial_balance, fiscal context)`.
2. **Tách lớp:** period resolution ≠ aggregation ≠ presentation (dòng B01/B02/…).
3. **DRY:** không copy-paste domain theo từng loại filter.
4. **KISS:** chỉ thêm nhánh kỳ khi có quy định pháp lý / nghiệp vụ khác biệt — và ghi comment nguồn quy định.

## Chống tái phát

- Mỗi báo cáo trong scope có ít nhất một test: **tổng các tháng trong quý == báo cáo quý** (hoặc quy tắc snapshot đã ký).

## UI/UX (wizard báo cáo)

- Nhãn filter rõ: theo ngày hạch toán / chứng từ (nếu có lựa chọn).
- Tránh hai cách đặt tên khác nhau cho cùng một kỳ (gây hiểu nhầm UAT).
