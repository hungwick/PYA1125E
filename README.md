# PYA1125E
ĐỒ ÁN

##  Xây dựng hệ thống dự báo nhu cầu và tối ưu chuỗi cung ứng trên nền tảng Odoo

---
Sinh viên thực hiện: Lương Mạnh Hùng

## 📁 1. CẤU TRÚC THƯ MỤC

Thư mục nộp bài được tổ chức theo cấu trúc như sau:

```
PYA1125E_LuongManhHung/
│
├── 01_Cơ sở dữ liệu/
│   ├── DoAnTN_2026-03-29_13-45-17.zip
│   └── dataset_banh_mi.csv
│
├── 02_Code/
│   ├── odoo_addons/
│   │   └── smart_inventory_forecast/
│   │
│   ├── ai_training/
│   │   ├── generate_dataset.py
│   │   ├── train_model.py
│   │   └── ai_model_universal.pkl
│   │
│   └── requirements.txt
│
├── 03_Các tài liệu/
│   ├── LuongManhHung_Slide thuyết trình.pptx
│   ├── LuongManhHung_Hướng dẫn cài đặt.pdf
│   ├── LuongManhHung_Báo cáo.pdf
│   └── LuongManhHung_Video demo.mp4
```

---

## 🗄️ 2. CƠ SỞ DỮ LIỆU

Thư mục **01_Cơ sở dữ liệu** bao gồm:

* `database_dump.sql`: file export database từ Odoo
* `dataset_banh_mi.csv`: dữ liệu giả lập dùng để train AI

---

## 💻 3. MÃ NGUỒN

Thư mục **02_Code** bao gồm:

### 🔹 Module Odoo

* `smart_inventory_forecast/`
* Chứa toàn bộ logic:

  * Dự báo nhu cầu
  * Tính toán nhập hàng
  * Tạo đơn mua hàng

---

### 🔹 AI Training

* `generate_dataset.py`: sinh dữ liệu giả lập
* `train_model.py`: huấn luyện mô hình
* `ai_model_universal.pkl`: model đã train

---

### 🔹 Thư viện

* `requirements.txt`: danh sách thư viện cần cài

---

## 📊 4. TÀI LIỆU

Thư mục **03_Các tài liệu** gồm:

* Slide thuyết trình
* Hướng dẫn cài đặt
* Báo cáo đồ án
* Video demo hệ thống

---

## ⚙️ 5. HƯỚNG DẪN CHẠY HỆ THỐNG

### Bước 1: Cài đặt môi trường

```bash
pip install -r requirements.txt
```

---

### Bước 2: Khởi động Odoo

* Cài đặt Odoo 19
* Thêm module vào addons path
* Update module

---

### Bước 3: Load database

* Import file `DoAnTN_2026-03-29_13-45-17.zip`

---

### Bước 4: Sử dụng hệ thống

* Vào menu: AI Forecast
* Tạo dự báo
* Chạy AI
* Tạo đơn mua hàng

---

## 🤖 6. MÔ HÌNH AI

* Thuật toán: Decision Tree
* Input:

  * Thứ
  * Tháng
  * Cuối tuần
* Output:

  * Nhóm nhu cầu A/B/C

Model được lưu tại:

```
ai_model_universal.pkl
```

---

## 🎯 7. CHỨC NĂNG CHÍNH

* Dự báo nhu cầu bằng AI
* Tính toán số lượng cần nhập
* Kiểm tra tồn kho thực tế
* Làm tròn theo quy cách đóng gói
* Tự động tạo đơn mua hàng

---

## ⚠️ 8. LƯU Ý

* Dữ liệu sử dụng là dữ liệu giả lập
* Hệ thống chưa tích hợp POS
* AI chỉ phân loại (không dự báo số lượng cụ thể)
