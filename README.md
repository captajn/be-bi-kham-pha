# Bé Bi Khám Phá

Game giáo dục trên trình duyệt cho trẻ tiểu học Việt Nam (lớp 1–5), phong cách
BabyBus nhưng nhân vật, tên gọi và hình ảnh đều sáng tạo riêng. Chơi một người,
không tài khoản, không quảng cáo, không mua trong ứng dụng, không thu thập dữ
liệu trẻ em. Chạy hoàn toàn trong trình duyệt, tắt mạng sau khi tải xong vẫn
chơi được.

> English summary: a free educational web game for Vietnamese primary-school
> kids (grades 1–5). Six mini-games teach maths, Vietnamese reading, English
> vehicle words, fire safety (emergency number 114) and road safety. Static
> HTML/CSS/JS, no build step, no backend, no accounts, no ads.

## Chơi thử ngay

Mở `index.html` bằng trình duyệt, hoặc chạy server tĩnh:

```bash
python3 -m http.server 8000
# mở http://localhost:8000
```

## Hiện trạng (thật, không nói quá)

- `index.html`: bản demo chơi được — 3 mini-game (Xây Nhà Khối Vuông,
  Phi Công Nhí, Lính Cứu Hỏa), độ khó lớp 1, có giọng đọc tiếng Việt
  (Web Speech API), sticker lưu local.
- `docs/spec-lop-1.md`: bản thiết kế đầy đủ cho 6 mini-game ở độ khó lớp 1
  (đếm 1–20, cộng/trừ trong 20, đọc từ đơn, từ tiếng Anh về phương tiện,
  số khẩn cấp 114, luật giao thông + xe ưu tiên).
- Chưa có: chọn lớp 2–5, 3 mini-game còn lại (Toán Vui Cùng Xe, Đọc Chữ
  Cùng Máy Bay, An Toàn Giao Thông) ở bản demo, PWA offline, dashboard
  phụ huynh. Đó chính là việc cần làm tiếp — xem `docs/ROADMAP.md`.

## 6 mini-game

1. **Xây Nhà Khối Vuông** — xếp khối vuông theo mẫu, đếm và cộng số khối.
2. **Phi Công Nhí** — đếm hành khách lên/xuống, cộng/trừ qua chuyến bay.
3. **Lính Cứu Hỏa** — dập lửa hoạt hình, học số 114 và 3 bước khi thấy cháy.
4. **Toán Vui Cùng Xe** — phép tính qua xe cộ, bàn phím số to.
5. **Đọc Chữ Cùng Máy Bay** — ghép từ đơn tiếng Việt, học từ tiếng Anh.
6. **An Toàn Giao Thông** — đèn đỏ dừng, đèn xanh đi, nhường xe ưu tiên.

Nguyên tắc vàng: **bé không bao giờ "thua"** — không game over, không trừ
điểm, không hết giờ thua. Sai thì gợi ý nhẹ nhàng và cho thử lại không giới hạn.

## Lộ trình lớp 1–5

Mỗi lớp là một mức độ khó riêng trong cùng 6 mini-game, theo chương trình
tiểu học Việt Nam. Chi tiết từng lớp và 4 milestone trong `docs/ROADMAP.md`:

- **M1** — Hoàn thiện 6 game ở độ khó lớp 1 + tách module + chọn lớp.
- **M2** — Nội dung lớp 2–3 (cộng/trừ trong 100, bảng nhân/chia, phân số đơn giản).
- **M3** — Nội dung lớp 4–5 (số lớn, phân số, số thập phân, tỉ số %) + khu phụ huynh.
- **M4** — PWA offline, tối ưu hiệu năng, bot chơi thử tự động.

## Công nghệ

- HTML/CSS/JavaScript thuần, file tĩnh, không cần build.
- Giọng đọc: Web Speech API (`vi-VN` cho tiếng Việt, `en-US` cho từ tiếng Anh).
- Lưu tiến trình: `localStorage` trên máy bé, không gửi ra ngoài.
- Mục tiêu: chạy mượt 60fps trên điện thoại Android 3–4 năm tuổi và iPad.

## Giấy phép

MIT — xem `LICENSE`. Mọi nhân vật (Gấu Bo, Mèo Mun, Thỏ Cà Rốt, Cú Mèo Phi
Công, Chó Đốm Cứu Hỏa) là sáng tạo riêng của dự án, không sao chép BabyBus
hay Minecraft.
