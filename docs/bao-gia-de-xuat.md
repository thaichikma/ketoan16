# Bao gia de xuat - Du an Odoo 16 bao cao Ke toan VN

> Phien ban: v1.0 (2026-03-20)  
> Hieu luc bao gia: 15 ngay

## 1) Pham vi gia

- Sua lech so lieu bao cao giua loc thang / quy / nam trong pham vi da thong nhat.
- Refactor logic de de bao tri.
- Bo sung test case + du lieu gia lap bien thoi gian (dau/cuoi thang, quy, giap nam).
- UAT va ban giao tai lieu.

## 2) Mo hinh thanh toan theo milestone (khuyen nghi)

| Milestone | Noi dung | Thoi gian uoc luong | Chi phi (VND) |
|-----------|----------|---------------------|---------------|
| **M1** | Discovery: tai hien loi, phan tich nguyen nhan, bao cao ky thuat | 3-7 ngay | **12.000.000 - 22.000.000** |
| **M2** | Design: dac ta refactor + test strategy + estimate chi tiet | 2-4 ngay | **8.000.000 - 14.000.000** |
| **M3** | Build: implement refactor + test automation + mock data | 10-25 ngay | **45.000.000 - 120.000.000** |
| **M4** | UAT: chay checklist voi ke toan + sua loi trong scope | 3-7 ngay | **12.000.000 - 28.000.000** |
| **M5** | Handover: release notes, huong dan deploy, ho tro sau go-live | 2-5 ngay | **6.000.000 - 15.000.000** |

### Tong ngan sach tham khao

- **Nho (1-2 bao cao trong yeu):** ~ **60-90 trieu VND**
- **Trung binh (3-5 bao cao):** ~ **90-150 trieu VND**
- **Lon (toan bo nhom bao cao VN lien quan):** ~ **150-220+ trieu VND**

## 3) Phuong an don gia ngay cong (neu khach yeu cau)

- Senior Odoo 16 + ke toan VN: **4.000.000 - 7.000.000 VND/ngay**
- Bao gia cuoi cung = ngay cong thuc te theo milestone da nghiem thu.

## 4) Dieu kien bao gia

- Co DB mau (an danh) tai hien duoc loi hoac co du lieu du de dung lai loi.
- Co vi du so lieu lech cu the (thang vs quy) toi thieu 1 bao cao.
- Co xac nhan dinh nghia nghiem thu "khop" (phat sinh ky hay snapshot).

## 5) Ngoai pham vi (mac dinh)

- Tuy bien moi khong lien quan loi lech so lieu.
- Lam sach toan bo technical debt ngoai khu vuc bao cao trong scope.
- Tich hop he thong ngoai Odoo (DWH, BI, middleware) tru khi co add-on hop dong.

## 6) Dieu khoan thanh toan de xuat

- Coc **30%** khi bat dau M1.
- Thanh toan theo tung milestone ngay khi co bien ban/email nghiem thu:
  - M1: 20%
  - M2: 10%
  - M3: 25%
  - M4: 10%
  - M5: 5%
- Hoac phuong an don gian: thanh toan 100% theo tung milestone da hoan tat.

## 7) Cam ket nghiem thu

- Cung loai bao cao trong scope: doi chieu thang/quy/nam theo tieu chi da ky phai nhat quan.
- Bo test case da thong nhat chay pass tren moi truong Odoo muc tieu.
- Code refactor ro rang, co comment o cac diem nghiep vu chinh.

## 8) Ghi chu quan trong

- Day la **bao gia tham khao ban dau**. Sau khi hoan thanh M1, se chot gia M3/M4/M5 chinh xac hon theo muc do custom thuc te.
