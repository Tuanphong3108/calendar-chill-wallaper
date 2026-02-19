# ⛏ Minecraft At A Glance – Smart Weather Wallpaper

Một **live wallpaper HTML duy nhất** phong cách **Minecraft + Pixel Weather + Material You**
hiển thị:

* Thời tiết thời gian thực 🌤
* Nhiệt độ đổi màu theo mức độ nóng/lạnh 🌡
* Quote Minecraft ngẫu nhiên 🎮
* Đồng hồ + lịch tự động theo múi giờ 🕒
* Background Minecraft theo tháng 🏞

Toàn bộ dự án chỉ cần **1 file `index.html`** để chạy.
UI hoạt động offline, chỉ cần mạng khi gọi API thời tiết.

---

# ✨ Tính năng

## 🌦 Thời tiết thời gian thực

* Lấy dữ liệu từ **Open-Meteo API**
* Tự động nhận **timezone theo vị trí**
* Cập nhật mỗi **10 phút**
* Icon **ngày / đêm riêng**
* Hỗ trợ **thời tiết cực đoan**:

  * ≥ **35°C** → Very Hot 🔥
  * ≤ **5°C** → Very Cold ❄

---

## 🌡 Màu nhiệt độ thông minh

| Nhiệt độ | Màu        | Trạng thái   |
| -------- | ---------- | ------------ |
| ≥ 35°C   | Cam đỏ     | Nóng cực hạn |
| 28–34°C  | Vàng cam   | Nóng         |
| 20–27°C  | Trắng      | Dễ chịu      |
| 6–19°C   | Cyan       | Mát          |
| ≤ 5°C    | Xanh dương | Lạnh sâu     |

---

## 🎮 Quote Minecraft ngẫu nhiên

* Hơn **100+ câu quote**
* **30%** dùng quote theo thời tiết
* Còn lại là **Minecraft facts/tips**
* Tự đổi mỗi **30 giây**

---

## 🕒 Đồng hồ & lịch tự động

* Đồng hồ số theo **múi giờ thực**
* Lịch tháng:

  * Highlight **ngày hiện tại**
  * Tự đổi khi sang ngày mới
* Background **Minecraft đổi theo tháng**

---

## 🎨 Giao diện Material You + Pixel Weather

* Font **Google Sans Flex**
* Icon **Google Pixel Weather**
* Hỗ trợ **Light / Dark mode**
* Hiệu ứng mượt:

  * Fade background
  * Transition màu nhiệt độ
  * Loader khi khởi động

---

# 🛠 Hướng dẫn sử dụng

## Bước 1: Tải file

1. Mở file **`index.html`** trong repository này.
2. Tải xuống máy.
3. Mở bằng **Notepad**.

---

## Bước 2: Đổi tọa độ vị trí

1. Trong Notepad, tìm đoạn:

```js
const TARGET_LAT = <vĩ độ>;
const TARGET_LON = <kinh độ>;
```

2. Giữ nguyên cửa sổ đó.

3. Mở trình duyệt → vào **https://maps.google.com**

4. Nhấn **“Xác định vị trí”** và cấp quyền nếu được hỏi.

5. Bấm vào **dấu chấm xanh** vị trí của bạn.

6. Ở đáy màn hình sẽ thấy:

```
<số thập phân 1>, <số thập phân 2>
```

* Dán **số thứ nhất** vào `TARGET_LAT`
* Dán **số thứ hai** vào `TARGET_LON`

7. **Lưu file**.

---

## Bước 3: Dùng làm live wallpaper

1. Di chuyển file **`index.html`** vào **một thư mục riêng**.
   (Trong thư mục chỉ cần duy nhất file này.)

2. Mở **Microsoft Store** → cài **Lively Wallpaper**.

3. Mở Lively:

   * Nhấn dấu **“+”**
   * Chọn **file HTML**
   * Nhấn **OK**

4. Chọn wallpaper vừa thêm để **đặt làm hình nền**.

---

## Bước 4: Bật giao diện tự động (khuyến nghị)

1. Nhấn **bánh răng** góc trên phải Lively.
2. Vào **Chủ đề**.
3. Chọn **Tối → Hệ thống**.

Hoàn tất. 🎉

---

# 📂 Cấu trúc dự án

```
root/
 └─ index.html
```

Chỉ **một file duy nhất** – cực gọn, cực nhẹ.

---

# 🔌 Công nghệ sử dụng

* **Open-Meteo** → dữ liệu thời tiết
* **Google Pixel Weather Icons** → bộ icon
* **TailwindCSS** → layout nhanh
* **Material You** → phong cách giao diện
* **Lively Wallpaper** → chạy HTML làm desktop wallpaper

---

# ⚠ Lưu ý

* Cần **internet** để cập nhật thời tiết.
* Nếu mất mạng → hiển thị **quote lỗi Minecraft**.
* Open-Meteo **miễn phí**, giới hạn rất cao → dùng thoải mái.

---

# ❤️ Credits

* Mojang & cộng đồng Minecraft
* Google Pixel Weather team
* Open-Meteo
* Và **Phong** – chủ nhân chiếc wallpaper chill nhất hệ mặt trời 🌍
