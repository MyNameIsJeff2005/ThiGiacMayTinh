## Giải thích cơ chế hoạt động Manipulating Images

### 1. Đọc ảnh
- Ảnh được đọc từ file bằng thư viện xử lý ảnh (PIL hoặc OpenCV).
- Ảnh sau khi đọc được lưu trong một biến để tiếp tục xử lý.

---

### 2. Thực hiện biến đổi ảnh
- Ảnh được **lật theo chiều dọc** bằng cách đảo vị trí các pixel trên và dưới.
- Ảnh được **lật theo chiều ngang (soi gương)** bằng cách đảo vị trí các pixel trái và phải.
- Các phép biến đổi này không làm thay đổi ảnh gốc mà tạo ra các ảnh mới.

---

### 3. Giải thích code hiển thị ảnh
- Sử dụng `matplotlib` để tạo một khung hiển thị.
- `subplot` được dùng để chia cửa sổ hiển thị thành nhiều phần.
- Mỗi ảnh sau khi xử lý được hiển thị ở một vị trí khác nhau để dễ so sánh.
- Trục tọa độ được tắt để tập trung quan sát nội dung ảnh.

---

### 4. Kết quả
- Hiển thị thành công ảnh sau khi lật dọc và ảnh sau khi soi gương.
- Có thể quan sát rõ sự khác biệt giữa các phép biến đổi ảnh.
