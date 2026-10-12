# MagicPix — Primoria Painter

> **Made by Hirus** | [Discord](https://discord.com/users/386072981799174144)

[![Download MagicPix](https://img.shields.io/badge/Download-MagicPix.zip-blue?style=for-the-badge)](https://github.com/hirusnov/MagicPix/releases/download/v.1.0.0/MagicPix.zip)

Vẽ pixel art siêu tốc vào game Primoria thông qua công nghệ Instant Autosave (hoàn tất chỉ trong 1 giây, không cần chuột hay calibrate).

[English version below](#english) | Tiếng Việt bên dưới

---

## Tiếng Việt

### Hướng Dẫn Sử Dụng (Nhanh Gọn)

> **Điểm nổi bật**: MagicPix là ứng dụng chạy **độc lập (standalone)**, bạn có thể giải nén và chạy `MagicPix.exe` ở **bất kỳ đâu** (Desktop, Downloads, thư mục tùy chọn). Toàn bộ các file save vẽ trong game sẽ **nằm ngay tại thư mục chứa MagicPix** và tự động đồng bộ hai chiều với game!

1. **Khởi động MagicPix**: Mở **MagicPix.exe**.
2. **Chọn Thư Mục Game**: Tại mục **THƯ MỤC GAME**, nhấn **📁 Chọn…** và trỏ đến thư mục cài đặt game Primoria (nơi có file `Primoria.exe`). MagicPix sẽ tự động lưu lại đường dẫn này cho các lần chạy sau.
3. **Tải ảnh hoặc vẽ tranh**:
   - Nhấn **Tải Ảnh** để chọn bất kỳ ảnh PNG/JPG nào (tự động khớp màu CIEDE2000 chuẩn 60 màu).
   - Dùng **Zoom Ảnh** để phóng to/thu nhỏ vùng cần lấy, sau đó nhấn **Tạo Lại Pixels**.
4. **Nhận diện và Dán vào game**:
   - Mở bảng vẽ trong game (Pixel Editor) hoặc nhấn **➕ Tạo Bản Vẽ Mới (Save Mới)** trực tiếp trên MagicPix.
   - MagicPix **tự động phát hiện** bảng vẽ mới (đánh dấu [MỚI]) và tự đồng bộ kích thước lưới (**16x16** hoặc **32x32**).
   - Nhấn **DÁN VÀO GAME (1 Giây)**.
5. **Xem kết quả**: Mở lại bảng vẽ trong game (hoặc chuyển tab tranh) — tác phẩm xuất hiện ngay lập tức 100% chuẩn xác.

> **Lưu ý**: Các file save bản vẽ nằm ngay trong thư mục chứa `MagicPix.exe`. Bạn có thể sao lưu, chia sẻ file save với bạn bè rất dễ dàng! Bạn cũng có thể bấm **Đọc Tranh từ Game** để kéo bức vẽ đang có vào MagicPix để chỉnh sửa hoặc xuất ra PNG.

---

### Tính Năng Chính

| Tính năng | Chi tiết |
| --- | --- |
| **Instant Save** | Ghi thẳng vào file autosave của game trong ~0.01 giây — **không cần di chuột, không delay, 0% lỗi click** |
| **Auto-Detect** | Tự động phát hiện khi bạn vừa mở bảng vẽ mới trong game và tự chọn ngay file đó |
| **Bảng màu 60 màu** | Hỗ trợ trọn vẹn **60 màu** cho cả hai loại lưới **16x16** và **32x32** |
| **Ảnh -> Pixel Art** | Thuật toán so khớp màu tri giác **CIEDE2000** chuẩn xác nhất |
| **Zoom & Crop Ảnh** | Phóng to/thu nhỏ chủ thể ảnh gốc trước khi chuyển đổi pixel |
| **Tùy chọn xử lý ảnh** | Bỏ qua màu nền, Dither Floyd-Steinberg, Màu sắc sống động (Vibrant mode), Cắt xén giữ tỷ lệ |
| **Panel công cụ** | Bút vẽ (Pen - ✏), Tẩy xóa từng ô (Eraser - ⌫), Hoàn tác (Undo - ↩), Làm lại (Redo - ↪), Xóa toàn bộ canvas (🗑) |
| **Undo / Redo** | 60 cấp hoàn tác (Ctrl+Z / Ctrl+Y) |
| **Lưu & Xuất** | Lưu dự án .mp (JSON) hoặc **Xuất PNG** sắc nét |
| **Đa ngôn ngữ** | Chuyển đổi linh hoạt **Tiếng Việt / English** |

---

### Phím Tắt

| Phím | Tác dụng |
| --- | --- |
| B / P | Chọn Bút vẽ (Pen) |
| E | Chọn Tẩy xóa từng ô (Eraser) |
| Shift + Click/Kéo | Tẩy xóa ô nhanh khi đang dùng Bút |
| Ctrl+Z | Hoàn tác |
| Ctrl+Y | Làm lại |
| Ctrl+S | Lưu dự án (.mp) |
| Ctrl+O | Mở dự án (.mp) |
| Cuộn chuột | Zoom canvas |
| Kéo chuột giữa | Pan / Di chuyển canvas |
| Click chuột phải | Hút màu từ ô (hoặc xóa ô khi đang bật Tẩy) |

---

### Discord & Hỗ Trợ

Câu hỏi, góp ý hoặc yêu cầu tính năng mới:  
Nhắn trực tiếp cho Hirus: **[discord.com/users/386072981799174144](https://discord.com/users/386072981799174144)**  
*(hoặc nhấn nút Discord trên thanh tiêu đề MagicPix)*

---

---

## English

Ultra-fast pixel art injection for Primoria via **Instant Autosave Inject** (complete in 1 second, zero mouse movement, no calibration needed).

### Quick Start

> **Key Highlight**: MagicPix runs **standalone anywhere** (Desktop, Downloads, any folder). You can send `MagicPix.exe` to anyone. All drawing save files created in game will **physically reside right in the folder where MagicPix is located**, seamlessly synchronized with the game!

1. **Launch MagicPix**: Run **MagicPix.exe**.
2. **Select Game Folder**: Under **GAME FOLDER**, click **📁 Select…** and pick your Primoria installation folder (where `Primoria.exe` is located). MagicPix remembers this setting automatically.
3. **Load artwork**:
   - Click **Load Image** to import any PNG/JPG image (perceptual CIEDE2000 60-color matching).
   - Use **Image Zoom** to crop/focus on your subject, then click **Re-generate Pixels**.
4. **Detect & Apply**:
   - Open the drawing board in-game or click **➕ Save as New Canvas** directly in MagicPix.
   - MagicPix **automatically detects** the new canvas (marked [NEW]) and auto-syncs your grid dimensions (**16x16** or **32x32**).
   - Click **INJECT INTO GAME (1 Sec)**.
5. **Done**: Re-open the drawing board in-game — your artwork appears instantly with 100% precision.

> **Note**: Canvas save files reside directly inside the folder containing `MagicPix.exe` for easy backup and sharing. You can also click **Load from Game** to import an existing in-game canvas into MagicPix for editing or exporting to PNG.

---

### Key Features

| Feature | Details |
| --- | --- |
| **Instant Save Inject** | Directly writes to the game save in ~0.01s — **no mouse clicks, zero delay, 0% misclick** |
| **Auto-Detect** | Automatically detects newly opened in-game canvases and selects them immediately |
| **60-Color Palette** | Full **60-color palette** supported for both **16x16** and **32x32** grids |
| **Image -> Pixel Art** | Perceptual **CIEDE2000** color matching for highest artistic fidelity |
| **Image Zoom & Crop** | Zoom in/out on source image before converting pixels |
| **Image Options** | Skip background, Floyd-Steinberg dithering, Vibrant mode, Crop aspect ratio |
| **Toolbar** | Pen tool (✏), Cell Eraser (⌫), Undo (↩), Redo (↪), Clear canvas (🗑) |
| **Undo / Redo** | 60-level undo stack (Ctrl+Z / Ctrl+Y) |
| **Save & Export** | Project files (.mp) and clean PNG export |
| **Bilingual UI** | Switch between **English** and **Tiếng Việt** |

---

### Keyboard Shortcuts

| Key | Action |
| --- | --- |
| B / P | Select Pen tool |
| E | Select Cell Eraser tool |
| Shift + Click/Drag | Quick erase while using Pen |
| Ctrl+Z | Undo |
| Ctrl+Y | Redo |
| Ctrl+S | Save project (.mp) |
| Ctrl+O | Load project (.mp) |
| Mouse-wheel | Zoom canvas |
| Middle-drag | Pan canvas |
| Right-click | Pick color from cell (or erase if Eraser tool active) |

---

### Discord & Support

Questions, feedback, or feature requests?  
Message Hirus directly: **[discord.com/users/386072981799174144](https://discord.com/users/386072981799174144)**
