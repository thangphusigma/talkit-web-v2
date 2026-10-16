# Microsoft TalkIt! trên web

Trang tĩnh chạy máy ảo x86 (v86) trong trình duyệt, gắn sẵn đĩa `talkit.iso` (TALKIT!.EXE + 3 DLL) vào ổ D:.

## Đưa lên GitHub Pages
1. Tạo repo mới (Public) trên github.com.
2. Add file → Upload files → chọn TẤT CẢ file trong thư mục này (kể cả `.nojekyll`) → Commit.
3. Settings → Pages → Source: "Deploy from a branch" → Branch: `main`, thư mục `/ (root)` → Save.
4. Đợi 1–2 phút, mở `https://<tên-bạn>.github.io/<tên-repo>/`.

## Lưu ý
- Windows không nằm trong repo. Trang tải ảnh đĩa từ `https://i.copy.sh/` (máy chủ của dự án v86). Muốn tự host thì đổi `?cdn=`.
- `user32.dll`, `shell32.dll`, `msvcrt40.dll` trong zip gốc là bản của Wine nên KHÔNG đưa vào đĩa (sẽ làm hỏng Windows thật). Windows 2000 có sẵn MFC40 và MSVCRT40.
- v86: BSD-2-Clause. SeaBIOS: LGPL.
