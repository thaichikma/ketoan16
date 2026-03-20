# Phase 4 — M4 UAT (User Acceptance)

**Mục tiêu:** khách xác nhận số liệu trên staging theo **định nghĩa nghiệm thu đã ký**.

## Chuẩn bị

- [ ] Deploy build M3 lên **staging**; `-u` module; smoke test đăng nhập
- [ ] Chuẩn bị **checklist UAT** từ danh sách báo cáo scope + từng cặp filter (tháng/quý/năm)
- [ ] Mời **đầu mối kế toán** + IT

## Thực hiện UAT

- [ ] Đi từng báo cáo: so sánh tháng vs quý (và năm nếu trong scope)
- [ ] Ghi **pass/fail** + screenshot hoặc file số cho fail
- [ ] Phân loại fail: bug code vs hiểu nhầm nghiệp vụ — xử lý lần lượt

## Sửa lỗi sau UAT

- [ ] Tạo task/fix cho từng fail; ưu tiên P0 (chặn nghiệm thu)
- [ ] Re-deploy; **regression test** tự động + spot check UAT

## Nghiệm thu

- [ ] Biên bản nghiệm thu có chữ ký / email xác nhận “đạt” theo tiêu chí đã ký
- [ ] Đính kèm hoặc link kết quả test pass cuối

## Definition of done

- [ ] Không còn fail mở trong scope đã ký
- [ ] Biên bản UAT đã lưu (PDF/email)
