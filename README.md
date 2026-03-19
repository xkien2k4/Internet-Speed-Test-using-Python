#  Internet Speed Test (Python GUI)

##  Giới thiệu

Đây là ứng dụng **kiểm tra tốc độ mạng Internet** được xây dựng bằng Python với giao diện đồ họa (GUI).
Chương trình cho phép người dùng đo các thông số mạng một cách trực quan và nhanh chóng.

---

##  Chức năng chính

*  Tự động tìm **server gần nhất**
*  Đo **tốc độ Download**
*  Đo **tốc độ Upload**
*  Hiển thị **Ping (độ trễ)**
*  Hiệu ứng hiển thị tốc độ (animation)
*  Thông báo trạng thái theo thời gian thực
*  Lưu lịch sử test vào file `history.txt`**

---

##  Công nghệ sử dụng

* **Python**
* **Tkinter** (thiết kế giao diện)
* **speedtest-cli** (đo tốc độ mạng)
* **threading** (tránh treo ứng dụng)

---

## 📥 Cài đặt

### 1. Cài Python

Tải tại: https://www.python.org/

---

### 2. Cài thư viện cần thiết

Mở Terminal / CMD:

```bash
pip install speedtest-cli
```

---

## ▶️ Cách chạy chương trình

```bash
python test.py
```

---

##  Giao diện chương trình

* Nút **START TEST** để bắt đầu
* Thanh loading hiển thị tiến trình
* Hiển thị:

  * Server đang test
  * Download (Mbps)
  * Upload (Mbps)
  * Ping (ms)

---

## 📂 Cấu trúc dự án

```
Internet-Speed-Test-using-Python/
│── test.py
│── history.txt
│── README.md
```

---

##  Nguyên lý hoạt động

* Sử dụng thư viện `speedtest-cli` để kết nối tới server gần nhất
* Thực hiện đo tốc độ tải xuống và tải lên
* Kết quả được xử lý và hiển thị lên giao diện
* Sử dụng `threading` để chạy song song, tránh treo GUI

---

##  Ví dụ kết quả

```
Download: 52.34 Mbps
Upload: 18.21 Mbps
Ping: 12.5 ms
```

---

##  Hướng phát triển

*  Thêm biểu đồ tốc độ
*  Hiển thị vị trí server trên bản đồ
*  Đóng gói thành file .exe
*  Lưu dữ liệu lên cloud
