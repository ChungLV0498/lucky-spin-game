# Hệ Thống Vòng Quay May Mắn & Bốc Thăm 3D

Ứng dụng bốc thăm trúng thưởng 3D tương tác thời gian thực trên nền tảng Web, được xây dựng phục vụ các sự kiện tổng kết, tiệc tất niên và hội nghị nội bộ.

- **Trải nghiệm trực tiếp:** [https://chunglv0498.github.io/lucky-spin-game/](https://chunglv0498.github.io/lucky-spin-game/)
- **Công nghệ nền tảng:** HTML5 Canvas, TagCanvas Engine, JavaScript (ES6+), CSS3

---

## 1. Giới Thiệu Dự Án

Ứng dụng mô phỏng quả cầu 3D chứa danh sách nhân sự tham gia bốc thăm. Khối cầu có khả năng xoay tự do theo không gian 3 chiều với gia tốc mượt mà, cho phép tương tác bằng chuột hoặc phím bấm. Khi dừng quay, thuật toán chọn ngẫu nhiên người trúng giải, kích hoạt hiệu ứng pháo hoa chúc mừng và tự động lưu trữ kết quả để tránh mất dữ liệu khi tải lại trang.

---

## 2. Tính Năng Kỹ Thuật

- **Mô phỏng quả cầu 3D thời gian thực:** Sử dụng kỹ thuật chiếu tọa độ 3D trên thẻ Canvas của HTML5, hỗ trợ xoay tự do theo các trục và phóng to/thu nhỏ bằng chuột.
- **Hỗ trợ song ngữ Việt - Trung:** Toàn bộ giao diện điều khiển, thông báo và nút bấm hỗ trợ song ngữ, phục vụ môi trường làm việc đa quốc gia.
- **Quản lý danh sách giải thưởng linh hoạt:** Cho phép lựa chọn cơ cấu giải thưởng (Giải Nhất, Giải Nhì, Giải Ba, Khuyến Khích) hoặc tùy chỉnh số lượng người trúng trong mỗi lượt quay.
- **Lưu trữ trạng thái bền vững:** Kết quả bốc thăm được lưu vào bộ nhớ cục bộ trình duyệt (LocalStorage), chống mất mát dữ liệu khi mất điện hoặc vô tình tải lại trình duyệt.
- **Trang tra cứu danh sách trúng thưởng riêng biệt:** Cung cấp bảng tổng hợp danh sách trúng giải (`result.html`) để đối chiếu và trao thưởng minh bạch.

---

## 3. Hướng Dẫn Vận Hành

1. Mở liên kết ứng dụng: [https://chunglv0498.github.io/lucky-spin-game/](https://chunglv0498.github.io/lucky-spin-game/)
2. Chọn giải thưởng tương ứng ở thanh điều khiển bên dưới.
3. Nhấn **Bắt đầu (开始)**: Quả cầu 3D sẽ tăng tốc quay ngẫu nhiên.
4. Nhấn **Dừng (停止)**: Hệ thống chốt danh sách người may mắn trúng giải và hiển thị bảng vinh danh kèm hiệu ứng pháo giấy.
5. Nhấn **Xem kết quả (获胜名单)** để mở bảng tổng hợp toàn bộ các đợt quay.
6. Để xóa kết quả và bắt đầu lượt mới: Nhấp chuột phải vào nút **Làm mới (重置)** và xác nhận.

---

## 4. Cấu Trúc Dự Án

```
├── index.html                  # Giao diện chính và khối cầu xoay 3D
├── result.html                 # Bảng tra cứu danh sách người trúng giải
├── css/
│   ├── reset.css               # Chuẩn hóa hiển thị CSS
│   └── wall.css                # Kiểu dáng giao diện và hiệu ứng sân khấu
├── js/
│   ├── tagcanvas.js            # Thư viện tính toán khối cầu 3D Canvas
│   ├── member.js               # Danh sách nhân sự và dữ liệu bốc thăm
│   └── zepto.js                # Xử lý sự kiện DOM tối ưu dung lượng
└── audio/                      # Tệp âm thanh quay thưởng và chúc mừng
```

---

## 5. Tác Giả & Bản Quyền

- **Kỹ sư phát triển:** Lê Văn Chung ([@ChungLV0498](https://github.com/ChungLV0498))
- **Mã nguồn:** Giấy phép MIT
