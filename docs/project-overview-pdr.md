# Project Overview & PDR — Odoo 16 · Báo cáo kế toán Localization Việt Nam

## Tóm tắt

Dự án nhằm **rà soát, sửa và refactor** logic sinh báo cáo kế toán trên **Odoo 16 Enterprise** khi dùng module **Kế toán Việt Nam (Vietnam Accounting Localization)**, khắc phục **lệch số liệu** giữa các cách lọc kỳ (tháng / quý / năm) và đảm bảo **nghiệm thu có thể kiểm chứng bằng test**.

## Vấn đề

- Cùng loại báo cáo, **lọc theo tháng** vs **lọc theo quý** cho kết quả **không khớp**.
- Nghi ngờ: nhiều nhánh `if/else` lồng nhau trong logic báo cáo → một số kỳ bị tính sai hoặc bỏ sót.
- Ảnh hưởng: độ tin cậy báo cáo tài chính gửi khách hàng.

## Mục tiêu

1. Xác định **nguyên nhân gốc** chênh lệch.
2. **Refactor** luồng tính toán, giảm điều kiện phức tạp; ưu tiên **một nguồn chuẩn hóa kỳ** (date range / context).
3. **Nhất quán** khi lọc tháng, quý, năm (theo định nghĩa nghiệm thu đã ký).
4. **Kiểm thử** toàn bộ báo cáo trong phạm vi sau sửa.
5. **Bộ dữ liệu giả lập** (test data) với biên: đầu/cuối tháng, đầu/cuối quý, giáp năm.

## Phạm vi ngoài code (cần khóa với khách)

- Module VN: Enterprise chuẩn, fork, hay custom.
- Danh sách **cụ thể** báo cáo trong nghiệm thu.
- Định nghĩa **“khớp”**: phát sinh kỳ vs số dư cuối kỳ; đơn vị tiền; một hay nhiều company.

## Ràng buộc & rủi ro

- **License Odoo Enterprise:** làm việc trên môi trường khách, không phân phối source core.
- Một phần “lệch” có thể do **hiểu nghiệp vụ** hoặc **cấu hình FY**, không phải bug — cần tài liệu khảo sát và ví dụ số trước khi refactor lớn.

## Tiêu chí nghiệm thu (mục tiêu)

- Cùng loại báo cáo: số liệu lọc theo tháng và theo quý **khớp hoàn toàn** (theo định nghĩa đã ký + sai số làm tròn nếu có).
- Bộ test case giả lập **chạy được trên Odoo**, pass 100% trong phạm vi.
- Code sau refactor **rõ ràng**, có **comment** ở các đoạn logic nghiệp vụ chính.

## Tham chiếu nội bộ

- Lộ trình chi tiết: [project-roadmap.md](./project-roadmap.md)
- Khảo sát / yêu cầu dữ liệu khách: [khao-sat-khach-hang.md](./khao-sat-khach-hang.md)
- Kiến trúc & nguyên nhân thường gặp: [system-architecture.md](./system-architecture.md)
