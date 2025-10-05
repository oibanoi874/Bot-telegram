# 🤖 Bot-telegram

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

## 🚀 3 Cách Chạy Bot

### 🧭 **Cách 1: Chạy trực tiếp trên máy (Windows / Termux / Linux)**
- Cài các package và file cần thiết
    ```bash
    pkg install git -y
    git clone https://github.com/oibanoi874/Bot-telegram
    cd Bot-telegram
    pip install -r requiremententer
    ```
- Sửa file config
    ```bash
    nano cf.json
    ```
- chạy bot
    ```bash
    python app.py
    ```

> 💡 Lệnh `nano cf.json` để vào file cf.json để chỉnh sửa sau khi sửa xong ctr+x rồi nhập y nhấn enter

---

### 🌐 **Cách 2: Chạy trên [Replit](https://replit.com/)**

1. Vào `https://replit.com/@oibanoi874/Bot-telegram-oibanoi874`
2. Vào `Remix this app`
3. Chọn `Remix App`
4. Vào file `cf.json` để sửa
5. Chạy bot 
6. Bot sẽ tự bật Flask keep-alive và chạy ổn định 24/7.

> 💡 Replit có thể cần thêm 1 service ping (vd [UptimeRobot](https://uptimerobot.com/?rid=56b57dd5ed7323)) để giữ bot online liên tục.

---

### 💣 **Cách 3: Chạy trên Katabump**

Katabump cho phép chạy Python liên tục giống Replit, nhưng nhanh hơn.

1. Truy cập [vào đây](https://dashboard.katabump.com/auth/login#9ce953)
2. Tạo tài khoản và sever
3. Tải file: [ở đây](https://www.mediafire.com/file/536rhchozkvprcz/bot-telegram.zip/file)
4. Upload file lên sever và unarcunar fild
5. Chỉnh sửa file cf.json và chạy bot
> 💡 Nhớ `ReNew` mỗi 4 ngày 

- Cách tải chi tiết: [ở đây]()

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
