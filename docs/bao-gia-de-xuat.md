# Báo giá đề xuất - Dự án Odoo 16 báo cáo Kế toán VN

> Phiên bản: v1.0 (2026-03-20)  
> Hiệu lực báo giá: 15 ngày

## 1) Phạm vi giá

- Sửa lệch số liệu báo cáo giữa lọc tháng / quý / năm trong phạm vi đã thống nhất.
- Refactor logic để dễ bảo trì.
- Bổ sung test case + dữ liệu giả lập biên thời gian (đầu/cuối tháng, quý, giáp năm).
- UAT và bàn giao tài liệu.

## 2) Mô hình thanh toán theo milestone (khuyến nghị)

| Milestone | Nội dung | Thời gian ước lượng | Chi phí (VND) |
|-----------|----------|---------------------|---------------|
| **M1** | Discovery: tái hiện lỗi, phân tích nguyên nhân, báo cáo kỹ thuật | 3-7 ngày | **12.000.000 - 22.000.000** |
| **M2** | Design: đặc tả refactor + test strategy + estimate chi tiết | 2-4 ngày | **8.000.000 - 14.000.000** |
| **M3** | Build: implement refactor + test automation + mock data | 10-25 ngày | **45.000.000 - 120.000.000** |
| **M4** | UAT: chạy checklist với kế toán + sửa lỗi trong scope | 3-7 ngày | **12.000.000 - 28.000.000** |
| **M5** | Handover: release notes, hướng dẫn deploy, hỗ trợ sau go-live | 2-5 ngày | **6.000.000 - 15.000.000** |

### Tổng ngân sách tham khảo

- **Nhỏ (1-2 báo cáo trọng yếu):** ~ **60-90 triệu VND**
- **Trung bình (3-5 báo cáo):** ~ **90-150 triệu VND**
- **Lớn (toàn bộ nhóm báo cáo VN liên quan):** ~ **150-220+ triệu VND**

## 3) Phương án đơn giá ngày công (nếu khách yêu cầu)

- Senior Odoo 16 + kế toán VN: **4.000.000 - 7.000.000 VND/ngày**
- Báo giá cuối cùng = ngày công thực tế theo milestone đã nghiệm thu.

## 4) Điều kiện báo giá

- Có DB mẫu (ẩn danh) tái hiện được lỗi hoặc có dữ liệu đủ để dựng lại lỗi.
- Có ví dụ số liệu lệch cụ thể (tháng vs quý) tối thiểu 1 báo cáo.
- Có xác nhận định nghĩa nghiệm thu "khớp" (phát sinh kỳ hay snapshot).

## 5) Ngoài phạm vi (mặc định)

- Tùy biến mới không liên quan lỗi lệch số liệu.
- Làm sạch toàn bộ technical debt ngoài khu vực báo cáo trong scope.
- Tích hợp hệ thống ngoài Odoo (DWH, BI, middleware) trừ khi có add-on hợp đồng.

## 6) Điều khoản thanh toán đề xuất

- Cọc **30%** khi bắt đầu M1.
- Thanh toán theo từng milestone ngay khi có biên bản/email nghiệm thu:
  - M1: 20%
  - M2: 10%
  - M3: 25%
  - M4: 10%
  - M5: 5%
- Hoặc phương án đơn giản: thanh toán 100% theo từng milestone đã hoàn tất.

## 7) Cam kết nghiệm thu

- Cùng loại báo cáo trong scope: đối chiếu tháng/quý/năm theo tiêu chí đã ký phải nhất quán.
- Bộ test case đã thống nhất chạy pass trên môi trường Odoo mục tiêu.
- Code refactor rõ ràng, có comment ở các điểm nghiệp vụ chính.

## 8) Ghi chú quan trọng

- Đây là **báo giá tham khảo ban đầu**. Sau khi hoàn thành M1, sẽ chốt giá M3/M4/M5 chính xác hơn theo mức độ custom thực tế.
