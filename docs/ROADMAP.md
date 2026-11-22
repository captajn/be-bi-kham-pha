# Lộ trình: Bé Bi Khám Phá lớp 1–5

Mỗi lớp là một mức độ khó trong cùng 6 mini-game. Bé chọn lớp ở màn hình
chính; bộ sinh câu hỏi đổi theo lớp. Nội dung theo chương trình tiểu học
Việt Nam (mức độ tham khảo, kiểm lại với sách giáo khoa trước khi chốt câu
hỏi từng lớp).

## Nội dung theo lớp

### Lớp 1 (đã có bản demo + spec đầy đủ)
- Đếm 1–20, cộng/trừ trong 20 có minh họa hình ảnh.
- Đọc từ đơn tiếng Việt về phương tiện; 6–8 từ tiếng Anh (airplane, pilot,
  fire truck, train, boat...).
- Nhớ số khẩn cấp 114, đèn đỏ dừng / đèn xanh đi, nhường xe cứu hỏa.

### Lớp 2 (mới)
- Cộng/trừ trong 100 (có nhớ), đếm tới 100.
- Bảng nhân 2, 3, 4, 5 qua hành khách / hành lý / khối.
- Đo độ dài: cm, m; so sánh dài – ngắn qua đường băng, xe cứu hỏa.

### Lớp 3 (mới)
- Nhân/chia trong 100, bảng nhân/chia đầy đủ.
- Phân số đơn giản: 1/2, 1/3, 1/4 qua chia khối, chia hành khách.
- Chu vi hình vuông / hình chữ nhật qua sân bay, khu xây dựng.

### Lớp 4 (mới)
- Số đến hàng triệu: đọc, viết, so sánh số lớn (dân số thị trấn, số khách/năm).
- Nhân/chia số có nhiều chữ số; cộng/trừ phân số cùng mẫu số.
- Diện tích hình vuông / hình chữ nhật; góc vuông, đường thẳng song song.

### Lớp 5 (mới)
- Số thập phân: đọc, so sánh, cộng/trừ (giá vé, cân hành lý).
- Tỉ số phần trăm đơn giản (khách đã lên máy bay đạt bao nhiêu %).
- Diện tích hình tam giác / hình thang; thể tích hình hộp chữ nhật qua xếp khối.
- Vận tốc đơn giản: xe cứu hỏa đi bao xa trong bao lâu (số tròn, dễ tính).

## 4 milestone cho Devin Bot

### M1 — Nền tảng + hoàn thiện lớp 1 (tuần 1–2)
- Tách `index.html` một file thành module: `src/games/` (mỗi game 1 thư mục),
  `src/audio/`, `src/input/`, `src/storage/`, `src/config/`.
- Thêm màn chọn lớp (1–5), lớp 2–5 hiện "sắp có" cho tới khi có nội dung.
- Hoàn thiện 3 game còn thiếu ở độ khó lớp 1: Toán Vui Cùng Xe, Đọc Chữ Cùng
  Máy Bay, An Toàn Giao Thông (theo `docs/spec-lop-1.md`).
- Cổng phụ huynh (giữ 3 giây + 1 phép tính), nhắc nghỉ sau 20 phút.
- Tiêu chí xong: chơi hết 6 game không lỗi console, nút ≥ 64px, chữ ≥ 26px.

### M2 — Nội dung lớp 2–3 (tuần 3–4)
- Bộ sinh câu hỏi theo lớp: `question-bank` có cấu hình độ khó từng lớp,
  test tự động chứng minh đáp án luôn đúng.
- Lớp 2: cộng/trừ trong 100, bảng nhân 2–5, đo độ dài.
- Lớp 3: nhân/chia trong 100, phân số 1/2–1/4, chu vi.
- Tiêu chí xong: mỗi lớp có ít nhất 50 câu hỏi sinh động, không trùng lặp
  liên tiếp; bot chơi thử qua hết.

### M3 — Nội dung lớp 4–5 + khu phụ huynh (tuần 5–6)
- Lớp 4: số lớn, nhân/chia nhiều chữ số, phân số, diện tích.
- Lớp 5: số thập phân, tỉ số %, thể tích, vận tốc đơn giản.
- Khu phụ huynh: xem tiến trình từng lớp (số sao, sticker, thời gian chơi),
  tắt nhạc/giọng, xóa tiến trình — tất cả lưu local.
- Tiêu chí xong: 5 lớp đều chơi được hết 6 game; phụ huynh xem được tiến trình.

### M4 — PWA + hiệu năng + kiểm thử (tuần 7)
- Manifest + service worker: chơi offline sau lần tải đầu.
- Đo và tối ưu: tải lần đầu ≤ 3 giây trên 4G, 60fps trên máy tầm trung.
- Bot chơi thử tự động: mỗi game 2 lượt (đúng hết + cố tình sai để kiểm gợi ý),
  chụp ảnh từng màn, 0 lỗi console.
- Tiêu chí xong: báo cáo hiệu năng + ảnh chụp 3 cỡ màn hình (390 / 768 / 1280px).

## Không làm (giới hạn rõ ràng)
- Không nhiều người chơi, không máy chủ, không tài khoản, không đăng nhập.
- Không quảng cáo, không mua trong ứng dụng, không analytics gửi ra ngoài.
- Không sao chép nhân vật, texture hay tên gọi của BabyBus / Minecraft.
