# Code Standards (dự kiến — Odoo / Python)

Áp dụng khi module Odoo được thêm vào repo.

## Python

- PEP 8; đặt tên rõ: `resolve_report_period`, `get_date_range_for_filter`, v.v.
- Ưu dùng exception Odoo (`UserError`, `ValidationError`) cho lỗi người dùng.
- Logging (`_logger`) cho nhánh nghiệp vụ phức tạp, không `print`.

## Odoo

- Kế thừa model/view bằng XML/Python; không sửa core Enterprise trực tiếp.
- Bảo mật: ACL / record rules nếu thêm model mới.
- Chuỗi giao diện: bọc `_()` cho text hiển thị.

## Báo cáo / refactor

- **Một nơi** resolve kỳ báo cáo; comment ngắn ở chỗ quy tắc **kế toán VN / FY** không hiển nhiên.
- Tránh if/else sâu: ưu tiên helper + data-driven mapping.

## Test

- `odoo.tests.common.TransactionCase` (hoặc tương đương Odoo 16).
- Dữ liệu: tạo COA + bút toán tại **biên ngày**; assert tổng tháng vs quý theo nghiệm thu.
