# 🐦 Flappy Bird Console Game – C++

- **Author**: Hồ Duy Vũ – Software Engineer | AI & Backend Developer
- **GitHub**: https://github.com/Ho-Duy-Vu
- **Email**: duyvu11092004@gmail.com
💻 **Language:** C++  
🖥️ **Platform:** Windows Console  

---

## 📌 Giới Thiệu Dự Án

**Flappy Bird Console Game** là một trò chơi mô phỏng Flappy Bird cổ điển, được xây dựng hoàn toàn bằng **C++ chạy trên Windows Console**.  
Trò chơi sử dụng các kỹ thuật điều khiển con trỏ console, xử lý bàn phím theo thời gian thực và quản lý va chạm.

Dự án nhằm mục đích:
- Rèn luyện tư duy lập trình C++
- Làm quen với xử lý đồ họa dạng text (ASCII)
- Quản lý vòng lặp game và logic va chạm

---

## 🎮 Gameplay

- Người chơi điều khiển chú chim vượt qua các cột ống
- Nhấn **phím Space** để chim bay lên
- Chim rơi tự động theo thời gian (gravity)
- Va chạm vào ống hoặc rơi xuống đất → **Game Over**
- Mỗi cột vượt qua → **tăng điểm**

---

## 🎯 Tính Năng Chính

### 🐦 Điều Khiển Chim
- Chim được vẽ bằng ký tự ASCII
- Chuyển động lên/xuống theo thời gian
- Nhấn **Space** để nhảy

### 🧱 Ống (Pipe)
- Sinh ngẫu nhiên vị trí khe hở
- Di chuyển từ phải sang trái
- Có 2 ống luân phiên tạo độ khó

### 💥 Va Chạm
- Kiểm tra va chạm giữa chim và ống
- Kiểm tra chim rơi khỏi màn hình

### 🧮 Tính Điểm
- Mỗi lần vượt qua 1 cặp ống → +1 điểm
- Hiển thị điểm số realtime

### 📋 Menu Chức Năng
- Start Game
- Hướng dẫn chơi
- Giới thiệu tác giả
- Thoát game

---

## ⌨️ Phím Điều Khiển

| Phím | Chức năng |
|----|----------|
| `Space` | Chim bay lên |
| `ESC` | Thoát game |
| Phím bất kỳ | Bắt đầu / quay lại menu |

---

## 🛠️ Công Nghệ & Thư Viện Sử Dụng

- **C++**
- **Windows API**
- `<windows.h>` – điều khiển console
- `<conio.h>` – bắt phím realtime
- `<time.h>` – random vị trí ống
- `<dos.h>` – delay & xử lý thời gian

---

## 🧠 Các Kỹ Thuật Áp Dụng

- Điều khiển con trỏ console (`gotoxy`)
- Ẩn/hiện con trỏ chuột
- Game loop (vòng lặp vô hạn)
- Xử lý input không đồng bộ (`kbhit`)
- Phát hiện va chạm
- Sinh chướng ngại vật ngẫu nhiên

---

## 📂 Cấu Trúc Chương Trình

```bash
FlappyBird.cpp
├── gotoxy()          # Di chuyển con trỏ console
├── drawBorder()      # Vẽ khung game
├── drawBird()        # Vẽ chim
├── drawPipe()        # Vẽ ống
├── collision()       # Kiểm tra va chạm
├── updateScore()     # Cập nhật điểm
├── play()            # Logic game chính
├── instructions()    # Hướng dẫn chơi
├── gioithieu()       # Giới thiệu tác giả
└── main()            # Menu & điều hướng
▶️ Cách Chạy Chương Trình
1️⃣ Yêu cầu
Windows OS

Trình biên dịch C++ (Dev-C++, Code::Blocks, Visual Studio)

2️⃣ Biên Dịch & Chạy
bash
Sao chép mã
g++ FlappyBird.cpp -o FlappyBird
FlappyBird.exe
Hoặc mở file .cpp trực tiếp bằng IDE và Run.

🚀 Hướng Phát Triển Tương Lai
Tăng độ khó theo thời gian

Thêm âm thanh

Lưu high score

Màu sắc console

Chuyển sang SDL / SFML

👤 Thông Tin Tác Giả
Name: Hồ Duy Vũ

Email: duyvu11092004@gmail.com

⭐ Nếu bạn thấy project hữu ích, hãy cho repo một star để ủng hộ nhé!

less
Sao chép mã

---

### ✅ README này phù hợp cho:
- Bài tập **C/C++**
- Nộp **môn Kỹ thuật lập trình**
- Portfolio sinh viên
- Repo GitHub cá nhân

Nếu bạn muốn:
- 🔹 Viết README **song ngữ Việt – Anh**
- 🔹 Viết **báo cáo Word/PDF từ code**
- 🔹 Giải thích code theo từng hàm (để thuyết trình)
- 🔹 Refactor code + comment chuẩn

👉 nói mình làm tiếp, mình hỗ trợ tới nơi 👍
