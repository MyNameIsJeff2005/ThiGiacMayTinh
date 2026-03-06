
## Giải thích ở phần 2 DFT

### `plt.subplot(121)`

* Hàm `subplot()` được dùng để  **chia cửa sổ hiển thị thành nhiều vùng nhỏ** .
* Tham số `121` có ý nghĩa:
  * **1** : số hàng
  * **2** : số cột
  * **1** : vị trí của biểu đồ hiện tại
* Như vậy, cửa sổ hiển thị được chia thành  **1 hàng và 2 cột** , và biểu đồ đầu tiên được đặt ở  **vị trí bên trái** .

---

### `plt.imshow(img, cmap='gray')`

* Hàm `imshow()` được sử dụng để  **hiển thị ảnh** .
* `img` là **ảnh gốc** đã được đọc từ file.
* `cmap='gray'` chỉ định sử dụng **bảng màu grayscale (ảnh xám)** để hiển thị ảnh.

---

### `plt.title('Input Image')`

* Hàm `title()` được dùng để  **đặt tiêu đề cho hình ảnh hiển thị** .
* Trong trường hợp này tiêu đề là  **"Input Image"** , nghĩa là ảnh đầu vào.

---

### `plt.xticks([]), plt.yticks([])`

* Hai hàm này dùng để  **ẩn các giá trị trục x và trục y** .
* Việc ẩn trục giúp  **hình ảnh hiển thị rõ ràng hơn và dễ quan sát hơn** .

---

# Hiển thị phổ tần số (Magnitude Spectrum)

### `plt.subplot(122)`

* Tiếp tục chia cửa sổ hiển thị thành  **1 hàng và 2 cột** .
* Tham số `122` nghĩa là **hiển thị biểu đồ ở vị trí thứ 2** (bên phải).

---

### `plt.imshow(magnitude_spectrum, cmap='gray')`

* Hiển thị  **phổ biên độ của ảnh trong miền tần số** .
* `magnitude_spectrum` là kết quả sau khi thực hiện  **biến đổi Fourier (DFT)** .
* Các vùng sáng biểu thị  **tần số mạnh** , vùng tối biểu thị  **tần số yếu** .

---

### `plt.title('Magnitude Spectrum')`

* Đặt tiêu đề cho biểu đồ là  **"Magnitude Spectrum"** .
* Điều này giúp người xem hiểu rằng đây là  **phổ biên độ của ảnh sau khi biến đổi Fourier** .

---

### `plt.xticks([]), plt.yticks([])`

* Tiếp tục **ẩn trục tọa độ x và y** để biểu đồ dễ quan sát hơn.

---

# Hiển thị kết quả

### `plt.show()`

* Hàm `show()` dùng để  **hiển thị toàn bộ các hình đã vẽ ra màn hình** .
* Khi chạy trong Jupyter Notebook, lệnh này sẽ  **render tất cả các subplot đã tạo** .
