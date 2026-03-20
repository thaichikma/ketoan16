# Phase 5 — M5 Handover & đóng dự án

**Mục tiêu:** production an toàn + tài liệu vận hành; đóng hợp đồng / thanh toán cuối.

## Production (nếu trong scope)

- [ ] Backup DB production theo quy trình khách
- [ ] Deploy + `-u` module trong cửa sổ bảo trì (nếu cần)
- [ ] Smoke test báo cáo chính sau go-live
- [ ] Theo dõi 24–48h: kênh hỗ trợ agreed

## Tài liệu bàn giao

- [ ] **Release notes:** version module, thay đổi chính, breaking changes (nếu có)
- [ ] Hướng dẫn **upgrade** và rollback (mức cao)
- [ ] Cập nhật [docs/deployment-guide.md](../../docs/deployment-guide.md) và [docs/project-overview-pdr.md](../../docs/project-overview-pdr.md) nếu có sai lệch so với thực tế
- [ ] Liệt kê **rủi ro còn lại** / out-of-scope để khách nắm

## Đóng dự án

- [ ] Gửi hóa đơn / xác nhận thanh toán milestone cuối (theo hợp đồng)
- [ ] Lưu trữ artifact: báo cáo M1, design M2, log UAT, mã merge cuối
- [ ] Cập nhật [plan.md](./plan.md) frontmatter `status: completed`

## Definition of done

- [ ] Khách xác nhận bàn giao bằng email
- [ ] Plan + phase files: toàn bộ task liên quan đã `[x]`
