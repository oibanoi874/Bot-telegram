# 🤖 Telegram Multi-Function Bot

Bot Telegram đa năng được viết bằng **Python**, sử dụng **python-telegram-bot** và **Flask** để giữ kết nối online.  
Bao gồm các tính năng: 🎲 Game, 🛠 Công cụ, 💰 Hệ thống coin, 📷 QR, 🎬 TikTok downloader, và ⚙️ Config UI trực tiếp trên Telegram.

---

## 🚀 Tính năng nổi bật

### 🎮 Giải trí
- `/taixiu 1 100` – Cược **Tài (1)** hoặc **Xỉu (2)** bằng coin.
- `/socau` – Xem 10 ván gần nhất.
- `/coin` – Xem số coin hiện tại.
- `/daily` – Nhận thưởng coin hàng ngày.

### 🛠 Công cụ tiện ích
- `/qr` – Tạo hoặc đọc mã QR.
- `/ttd <link TikTok>` – Tải video TikTok **không logo** hoặc **âm thanh**.
- `/rutgon <link>` – Rút gọn link bằng **TinyURL**.
- `/deepweb` – Hướng dẫn và cảnh báo khi truy cập **Deep Web**.

### 👤 Người dùng
- `/start` – Chào mừng người dùng.
- `/menu` – Danh sách lệnh.
- `/time` – Xem thời gian hiện tại (Asia/Bangkok).
- `/infouser` – Tạo thẻ thông tin người dùng (vẽ bằng Pillow).
- `/id` – Lấy ID Telegram cá nhân hoặc người khác.
- `/infobot` – Thông tin bot, link liên hệ.

### 👑 Quản trị (Owner)
- `/config` – Giao diện chỉnh config (qua inline button).
- `/idall` – Xem danh sách ID Owner.
- Log hoạt động tự động gửi đến owner.

---

## ⚙️ Cấu trúc file

```

📂 project/
├── app.py               # Mã nguồn chính của bot
├── cf.json              # Config bot (token, owner, link,...)
├── data_taixiu/         # Lưu dữ liệu người dùng, kết quả, config game
├── logs/                # File log hoạt động
├── backgrounds/         # Hình nền cho thẻ user (tùy chọn)
└── requirements.txt     # Danh sách thư viện cần cài

````

---

## 🧩 Yêu cầu

### Python >= 3.9  
Các thư viện cần thiết:

```bash
pip install -r requirements.txt
````

---

## 🪄 Cấu hình ban đầu

Khi chạy lần đầu, bot sẽ tự tạo file `cf.json` với cấu hình mặc định:

```json
{
  "token_main": "YOUR_BOT_TOKEN",
  "token_sub": "",
  "owners": [123456789],
  "log_op": [123456789],
  "port": 8080,
  "daily_reward": 100,
  "daily_cooldown": 14400
}
```

> 🔑 Điền **token bot Telegram** vào `token_main`, và thêm **ID của bạn** vào `owners`.

---

## 🖥️ Chạy bot

### Cách 1: Python trực tiếp

```bash
python app.py
```

### Cách 2: Replit

 Xem chi tiết: [ở đây](http:)

### Cách 3: Katabump

 Xem chi tiết: [ở đđây(https:)
---

## 📜 Một số lệnh quan trọng

| Lệnh            | Mô tả                            |
| --------------- | -------------------------------- |
| `/start`        | Chào người dùng                  |
| `/menu`         | Danh sách các lệnh               |
| `/taixiu 1 100` | Cược 100 coin cho “Tài”          |
| `/ttd <link>`   | Tải video TikTok không logo      |
| `/qr`           | Tạo hoặc đọc mã QR               |
| `/config`       | Giao diện chỉnh config cho owner |
| `/infouser`     | Tạo ảnh thông tin cá nhân        |
| `/idall`        | Hiển thị danh sách Owner         |

---

## 💬 Liên hệ

* 👑 **Tác giả:** [@oibanoi874](https://t.me/oibanoi874)
* 📧 **Email:** [oibanoi874@gmail.com](mailto:oibanoi874@gmail.com)
* 🐙 **GitHub:** [github.com/oibanoi874](https://github.com/oibanoi874)
* ▶️ **YouTube:** [@oibanoi874](https://www.youtube.com/@oibanoi874)

---

## 🧠 Ghi chú

* Có thể thêm hình nền vào thư mục `backgrounds/` để thẻ user đẹp hơn.
* Flask giữ bot **online 24/7** trên nền tảng Replit / VPS.
* Log tự động gửi cho owner khi đủ số lượng tin nhắn (`log_limit`).

---

### 🪶 Code by [@oibanoi874](https://t.me/oibanoi874)

