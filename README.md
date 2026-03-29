# PYA1125E
ĐỒ ÁN
Tên đề tài: Xây dựng hệ thống dự báo nhu cầu và tối ưu chuỗi cung ứng trên nền tảng Odoo

Sinh viên thực hiện: Lương Mạnh Hùng

---

1. MÔ TẢ HỆ THỐNG

Hệ thống được xây dựng nhằm hỗ trợ doanh nghiệp dự báo nhu cầu và tối ưu hóa nhập hàng dựa trên dữ liệu thực tế.

Các chức năng chính:

* Dự báo nhu cầu bằng AI (Nhóm A/B/C)
* Tính toán số lượng cần nhập dựa trên tồn kho và safety stock
* Làm tròn số lượng nhập theo quy cách đóng gói
* Tạo đơn mua hàng (Purchase Order)

---

2. CÔNG NGHỆ SỬ DỤNG

* Odoo 19
* Python
* Machine Learning (scikit-learn)
* PostgreSQL

---

3. CẤU TRÚC THƯ MỤC

* 1_SourceCode: mã nguồn module Odoo
* 2_Database: file backup database
* 3_Report: báo cáo đồ án
* 4_Slides: slide thuyết trình
* 5_InstallationGuide: hướng dẫn cài đặt
* 6_DemoVideo: video demo

---

4. HƯỚNG DẪN

Xem chi tiết trong file:
5_InstallationGuide/HuongDanCaiDat.docx

---

5. GHI CHÚ

* Hệ thống sử dụng dữ liệu giả lập phù hợp với mô hình cửa hàng bánh mì sinh viên
* AI được huấn luyện dựa trên dữ liệu thời gian (ngày, tháng, thứ)
