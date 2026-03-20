# Deployment Guide (khung)

## Môi trường

- **Staging** trùng hoặc gần production: cùng phiên bản Odoo 16, cùng module VN.
- DB copy **đã ẩn danh** để tái hiện lỗi; không dùng production trực tiếp cho thử nghiệm phá dữ liệu.

## Triển khai sau sửa

1. Merge module vào branch đã thỏa thuận.
2. `-u module_name` (upgrade) trên staging.
3. Chạy test tự động (CI hoặc `odoo-bin ... --test-enable`).
4. UAT với khách: checklist báo cáo + biên ngày.
5. Lên production theo quy trình khách (backup, maintenance window nếu cần).

## Ghi chú license

- Không đóng gói lại Odoo Enterprise core; chỉ deploy custom/localization thuộc quyền sở hữu / license hợp lệ.
