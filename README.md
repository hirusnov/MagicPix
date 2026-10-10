# MagicPix — Primoria Painter

> **Made by Hirus** | [Discord](https://discord.com/users/386072981799174144)

[![Download MagicPix](https://img.shields.io/badge/⬇%EF%B8%8F%20Download-MagicPix.zip-blue?style=for-the-badge)](https://github.com/hirusnov/MagicPix/releases/download/v.1.0.0/MagicPix.zip)

Tự động vẽ pixel art vào Primoria pixel editor (Clan Image & Board).

📖 [English version below](#-english) &nbsp;|&nbsp; 🇻🇳 Tiếng Việt bên dưới

---

## 🇻🇳 Tiếng Việt

### Hướng Dẫn Nhanh

1. Double-click **`MagicPix.exe`** để khởi động.
2. Chọn **Loại Lưới** ở panel bên phải:
   - **16×16 (Small Board)** — 20 màu, cho bảng nhỏ
   - **32×32 (Large Board)** — 20 màu, cho bảng lớn
   - **Clan 32×32 (60 Colors)** — 60 màu, cho Clan Emblem
3. Nhấn **"Tải Ảnh"** để chọn ảnh PNG/JPG.
4. Dùng **Zoom Ảnh** để phóng to/thu nhỏ vùng muốn chuyển đổi (tuỳ chọn).
5. Calibrate một lần: nhấn **📐 Calibrate Lưới** → chuyển sang cửa sổ game → di chuột tới từng điểm và giữ yên để ghi nhận.
6. Trong game, mở bảng vẽ pixel editor.
7. Nhấn **▶ BẮT ĐẦU VẼ** — bạn có vài giây để alt-tab vào game.

> 💡 **Calibration được tự động lưu.** Chỉ cần làm lại khi đổi độ phân giải màn hình hoặc di chuyển cửa sổ game.

---

### Tính Năng

| Tính năng        | Chi tiết                                                                              |
| ---------------- | ------------------------------------------------------------------------------------- |
| Ảnh → Pixel Art  | Chuyển đổi PNG/JPG bằng thuật toán màu sắc **CIEDE2000**                              |
| Bảng màu game    | **20 màu** cho 16×16 & 32×32 Large Board, **60 màu** cho Clan 32×32                   |
| Zoom Ảnh         | Phóng to/thu nhỏ ảnh gốc trước khi chuyển — **Phóng To / Thu Nhỏ / ↻ Tạo Lại Pixels** |
| Tự cuộn bảng màu | Auto-painter **tự động cuộn** bảng màu trong game khi vẽ Clan 60 màu                  |
| Canvas thủ công  | Vẽ tay bằng công cụ Bút                                                               |
| Undo / Redo      | 60 cấp hoàn tác (Ctrl+Z / Ctrl+Y)                                                     |
| Zoom & Pan       | Cuộn chuột để zoom, kéo chuột giữa để pan                                             |
| Tự động vẽ       | Click từng ô tự động, gộp theo nhóm màu                                               |
| Calibration      | Di chuột tới từng điểm và giữ yên 1.5s, **tự động lưu theo preset**                  |
| Lưu / Mở         | File `.mp` dự án (JSON)                                                               |
| Xuất PNG         | Xuất preview pixel ra PNG                                                             |
| Đa ngôn ngữ      | Chuyển **English / Tiếng Việt** bằng nút 🌐                                           |

---

### Calibration (Một lần mỗi độ phân giải)

Công cụ cần biết chính xác vị trí của lưới vẽ và bảng màu trên màn hình.

1. Mở bảng vẽ pixel editor trong game Primoria.
2. Nhấn **📐 Calibrate Lưới** ở panel bên phải của MagicPix.
3. Chuyển sang cửa sổ game.
4. Di chuột tới từng điểm, giữ chuột **yên 1.5 giây** — sẽ tự động ghi nhận.
   - _Tiếng BEEP xác nhận điểm đã được ghi._
   - _Không cần nhấn bất kỳ phím nào._
5. Ghi nhận 6 điểm theo thứ tự:
   - **Điểm 1**: Tâm ô **TRÊN-TRÁI** của lưới vẽ (hàng 1, cột 1)
   - **Điểm 2**: Tâm ô **TRÊN-PHẢI** của lưới vẽ (hàng 1, cột cuối)
   - **Điểm 3**: Tâm ô **DƯỚI-TRÁI** của lưới vẽ (hàng cuối, cột 1)
   - ⚠️ _Cuộn bảng màu lên đầu hoàn toàn trước khi ghi điểm 4–6._
   - **Điểm 4**: Tâm ô màu **Xanh lam nhạt** — Pastel Blue `#9DBAE4` (ô trên cùng bên trái của bảng màu)
   - **Điểm 5**: Tâm ô màu **Vàng kem** — Cream Yellow `#F6D084` (cùng hàng 1, ô ngay bên phải Điểm 4)
   - **Điểm 6**: Tâm ô màu **Hồng phấn nhạt** — Pastel Pink `#F7ABAB` (hàng 2, so le giữa Điểm 4 và 5)
6. Hộp thoại thành công xuất hiện. **Calibration tự động lưu** — lần sau mở MagicPix sẽ tự tải lại!
7. Nhấn **🎯 Kiểm Tra** để xem con trỏ lướt qua từng điểm và kiểm tra độ chính xác. (Tùy chọn)

---

### Cài Đặt Vẽ

| Cài đặt               | Mô tả                                                                                                           |
| --------------------- | --------------------------------------------------------------------------------------------------------------- |
| **Loại Lưới**         | 16×16 (20 màu) hoặc 32×32 (60 màu)                                                                              |
| **Tốc độ (ms/ô)**     | Thời gian chờ giữa các click. 40ms là an toàn; thấp hơn = nhanh hơn                                             |
| **Thứ Tự Vẽ**         | **Nhóm Màu** (tốt nhất) — vẽ hết tất cả ô cùng màu trước. **Theo Hàng** — vẽ từ trái sang phải, trên xuống dưới |
| **Bỏ qua màu nền**    | Bỏ qua màu nền (tự phát hiện từ 4 góc canvas)                                                                   |
| **Cuộn Bảng 32×32**   | **Tự kéo** — tự động drag cuộn bảng màu; **Không cuộn** — bỏ qua bước cuộn             |
| **Dither khi tải**    | Bật dithering Floyd-Steinberg khi chuyển đổi ảnh                                                                |
| **Màu sắc sống động** | Tăng độ bão hòa & tương phản (phù hợp ảnh thật)                                                                 |
| **Đếm ngược (giây)**  | Thời gian chờ trước khi vẽ — dùng để kịp alt-tab vào game                                                       |

---

### Phím Tắt

| Phím              | Tác dụng                                  |
| ----------------- | ----------------------------------------- |
| `Ctrl+Z`          | Hoàn tác                                  |
| `Ctrl+Y`          | Làm lại                                   |
| `Ctrl+S`          | Lưu dự án                                 |
| `Ctrl+O`          | Mở dự án                                  |
| Cuộn chuột        | Zoom canvas  |
| Kéo chuột giữa    | Pan canvas   |
| Click chuột phải  | Hút màu từ ô |

---

### Mẹo Hay

- **Alt-tab kịp thời**: Tăng Đếm ngược lên 4–5 giây nếu cần thêm thời gian.
- **Click bị bỏ sót**: Tăng ms/ô (ví dụ lên 60–80ms) nếu game không nhận đủ click.
- **Dừng khẩn cấp**: Di chuột đến **góc trên-trái màn hình** để dừng ngay lập tức.
- **Bảng 60 màu**: Auto-painter tự cuộn qua 3 phần — Trên (0–19), Giữa (20–39), Dưới (40–59).
- **Zoom Ảnh**: Phóng to vào mặt/nhân vật, sau đó nhấn **↻ Tạo Lại Pixels** — không cần tải ảnh lại.
- **Xuất ảnh preview**: Nhấn **Xuất PNG** để lưu ảnh pixel art hiện tại ra file.

---

### Discord

Câu hỏi, góp ý, yêu cầu tính năng?  
👉 Nhắn trực tiếp cho Hirus: **[discord.com/users/386072981799174144](https://discord.com/users/386072981799174144)**  
_(hoặc nhấn nút **Discord** trong MagicPix)_

---

---

## 🇬🇧 English

Auto-paint pixel art into the Primoria pixel editor (Clan Image & Board).

### Quick Start

1. Double-click **`MagicPix.exe`** to launch.
2. Choose your **Grid Preset** in the right panel:
   - **16×16 (Small Board)** — 20 colors, for small boards
   - **32×32 (Large Board)** — 20 colors, for large boards
   - **Clan 32×32 (60 Colors)** — 60 colors, for Clan Emblems
3. Click **"Load Image"** to pick a PNG/JPG file.
4. Use **Image Zoom** to crop/zoom the area you want to convert (optional).
5. Calibrate once: click **📐 Calibrate Grid** → switch to game → move mouse to each point and hold still to auto-capture.
6. In-game, open the pixel editor board.
7. Press **▶ START PAINTING** — you have a few seconds to alt-tab into the game.

> 💡 **Calibration is auto-saved.** You only need to redo it if your screen resolution or game window position changes.

---

### Features

| Feature             | Details                                                                         |
| ------------------- | ------------------------------------------------------------------------------- |
| Image → Pixel Art   | Converts any PNG/JPG using **CIEDE2000** perceptual color matching              |
| Game Palette        | **20 colors** for 16×16 & 32×32 Large Board, **60 colors** for Clan 32×32       |
| Image Zoom          | Zoom in/out on source image — **Zoom In / Zoom Out / ↻ Re-generate Pixels**     |
| Auto-Scroll Palette | For 60-color Clan boards, auto-painter **automatically scrolls** in-game palette |
| Manual Canvas       | Draw manually with the Pen tool                                                 |
| Undo / Redo         | 60-level undo stack (Ctrl+Z / Ctrl+Y)                                           |
| Zoom & Pan          | Mouse-wheel zoom, middle-click drag                                             |
| Auto-Painter        | Clicks every cell automatically, batched by color group                         |
| Calibration         | Hold mouse still at each point for 1.5s, **auto-saved per preset**              |
| Save / Load         | `.mp` project files (JSON)                                                      |
| Export PNG          | Export the pixel preview as a PNG image                                         |
| Bilingual UI        | Switch between **English** and **Tiếng Việt** via the 🌐 button                 |

---

### Calibration (Once per resolution)

The tool needs to know exactly where the pixel grid and palette swatches are on your screen.

1. Open the pixel editor board in-game (Primoria).
2. Click **📐 Calibrate Grid** in the right panel of MagicPix.
3. Switch to the game window.
4. Move your mouse to each point and hold still for **1.5 seconds** — it captures automatically.
   - _A beep confirms each capture._
   - _No key press needed._
5. Record 6 points in order:
   - **Point 1**: Center of **Top-Left** pixel cell (row 1, col 1 of the drawing grid)
   - **Point 2**: Center of **Top-Right** pixel cell (row 1, last col of the drawing grid)
   - **Point 3**: Center of **Bottom-Left** pixel cell (last row, col 1 of the drawing grid)
   - ⚠️ _Scroll the palette all the way to the top before capturing points 4–6._
   - **Point 4**: Center of **Pastel Blue** swatch — `#9DBAE4` (top-left hexagon of the palette)
   - **Point 5**: Center of **Cream Yellow** swatch — `#F6D084` (same top row, directly right of Point 4)
   - **Point 6**: Center of **Pastel Pink** swatch — `#F7ABAB` (row 2, staggered between Point 4 and 5)
6. A success dialog appears. **Calibration is automatically saved** — it will reload next time you open MagicPix!
7. Click **🎯 Test** to watch the cursor glide through each position and verify accuracy.

---

### Paint Settings

| Setting             | Description                                                                         |
| ------------------- | ----------------------------------------------------------------------------------- |
| **Grid Preset**     | 16×16 (20 colors) or 32×32 (60 colors)                                              |
| **Speed (ms/cell)** | Delay between clicks. 40ms is safe; lower = faster                                  |
| **Paint Order**     | **Color Group** (best) — all same-color cells first. **Scanline** — row by row      |
| **Skip background** | Skip the background color (auto-detected from canvas corners)                       |
| **32×32 Scroll**    | **Auto Drag** — automatically drags to scroll the palette; **None** — skip scrolling |
| **Dither on load**  | Floyd-Steinberg dithering when converting image                                     |
| **Vibrant colors**  | Boost saturation/contrast for photos                                                |
| **Warmup (s)**      | Seconds before painting starts — time to alt-tab into the game                      |

---

### Keyboard Shortcuts

| Key               | Action                               |
| ----------------- | ------------------------------------ |
| `Ctrl+Z`          | Undo                                 |
| `Ctrl+Y`          | Redo                                 |
| `Ctrl+S`          | Save project                         |
| `Ctrl+O`          | Load project                         |
| Mouse-wheel       | Zoom canvas             |
| Middle-drag       | Pan canvas              |
| Right-click       | Eyedrop color from cell |

---

### Tips

- **Alt-tab timing**: Set Warmup to 4–5s if you need more time to switch windows.
- **Missed clicks**: Increase ms/cell (e.g. 60–80ms) if the game misses clicks.
- **Emergency stop**: Move mouse to the **top-left corner** of the screen to abort immediately.
- **60-color board**: The auto-painter scrolls through 3 palette sections — Top (0–19), Middle (20–39), Bottom (40–59).
- **Image Zoom**: Zoom into a face or subject, then click **↻ Re-generate Pixels** — no need to reload the image.
- **Export preview**: Click **Export PNG** to save the current pixel art as an image file.

---

### Discord

Questions, suggestions, or feature requests?  
👉 Message Hirus directly: **[discord.com/users/386072981799174144](https://discord.com/users/386072981799174144)**  
_(or click the **Discord** button inside MagicPix)_
