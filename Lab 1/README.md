# SO SÁNH SỰ KHÁC BIỆT GIỮA PIL VÀ OPENCV

## 1. Cách đọc ảnh và kiểu dữ liệu

### PIL
- Sử dụng hàm `Image.open()`.
- Kết quả trả về là một object của lớp `PIL.Image`.

### OpenCV
- Sử dụng hàm `cv2.imread()`.
- Kết quả trả về là một `numpy array` chứa các giá trị số nguyên 8-bit (uint8).

---

## 2. Không gian màu

- **PIL**:  
  Ảnh được đọc theo thứ tự kênh màu **RGB (Red – Green – Blue)**.

- **OpenCV**:  
  Ảnh được đọc theo thứ tự kênh màu **BGR (Blue – Green – Red)**.

---

## 3. Cách hiển thị ảnh

### PIL
- Chỉ cần gọi tên biến chứa ảnh, ảnh sẽ tự động hiển thị trong Jupyter Notebook.

### OpenCV
- Hàm `cv2.imshow()` thường gây lỗi hoặc làm treo Jupyter Notebook, do đó không được sử dụng trực tiếp.
- Thay vào đó, ảnh được hiển thị bằng thư viện `matplotlib.pyplot` với hàm `plt.imshow(image)`.
- Do sự khác biệt giữa không gian màu RGB và BGR, cần chuyển đổi ảnh trước khi hiển thị bằng:
  ```python
  cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
