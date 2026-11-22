# Bản giao việc "Bé Bi Khám Phá" — Game trẻ em giáo dục, bản một người chơi

> Copy toàn bộ file này dán vào Claude / Claude Code / AI builder là chạy.
> Gốc là cấu trúc bản giao việc "Việt Nam Survival" (FPS một người chơi, offline, build tĩnh), đã viết lại toàn bộ nội dung sang game trẻ em giáo dục kiểu BabyBus — nhưng nhân vật, tên game, hình ảnh và lời thoại đều là sáng tạo riêng, KHÔNG sao chép BabyBus.
>
> **Bản chỉnh ngày 2026-11-12 — cho bé trai 6 tuổi (lớp 1), thích xếp khối vuông kiểu Minecraft, máy bay và xe cứu hỏa.** Độ khó nâng lên so với bản 3–6 tuổi: đếm 1–20, cộng/trừ trong 20, đọc từ đơn tiếng Việt, học từ tiếng Anh về phương tiện. 3 sở thích của bé thành 3 mini-game chính. Chỉ học *cơ chế* xếp khối vuông kiểu Minecraft — KHÔNG sao chép texture, nhân vật, tên gọi hay tài sản nào của Minecraft.

---

## === NHIỆM VỤ ===

Dựng game trẻ em giáo dục "Bé Bi Khám Phá", chơi một người, chạy trên trình duyệt (điện thoại / máy tính bảng là chính, máy tính vẫn chơi được). Đối tượng: bé trai 6 tuổi (lớp 1), thích xếp khối vuông kiểu Minecraft, máy bay và xe cứu hỏa. Bé đã đọc được từ đơn giản và đếm được tới 20, nên game dạy đếm 1–20, cộng/trừ trong 20, đọc từ đơn và từ tiếng Anh về phương tiện.

Quy mô nhỏ, nhưng hình ảnh, cảm giác chạm và giọng hướng dẫn phải ở mức app trẻ em lớn. Thà ít mini-game mà game nào cũng hoàn thiện, bé chơi được ngay, còn hơn nhiều game làm dở.

Bạn làm việc không có người giám sát. Không hỏi lại; tự quyết định và ghi vào DECISIONS.md.

Không mua gì. Chỉ được đưa bản build tĩnh lên đúng một tên miền nêu ở mục TRIỂN KHAI; ngoài ra không đăng tải gì ra ngoài.

Thiết kế phải là của riêng dự án. Không sao chép tên, nhân vật (Kiki, Miumiu...), logo, giao diện, nhạc hay hình ảnh của BabyBus, Khan Kids, Cocomelon hay hãng có thật. Không sao chép texture, nhân vật (Steve, Creeper...), tên gọi hay tài sản của Minecraft — chỉ học cơ chế xếp khối vuông chung. Mọi nhân vật, tên địa điểm, biển hiệu trong game dùng tên bịa, do dự án tự sáng tạo.

Không làm, kể cả khi thấy "tiện thì làm luôn": nhiều người chơi, máy chủ trận, kết nối mạng trong lúc chơi, tài khoản, đăng nhập, cơ sở dữ liệu, lưu trữ phía máy chủ, quảng cáo, mua trong ứng dụng, chat, bình luận, liên kết ra ngoài, thu thập dữ liệu trẻ em. Game chạy hoàn toàn trong trình duyệt; tắt mạng sau khi tải xong vẫn chơi được hết. Không viết code "chừa chỗ cho nhiều người chơi / quảng cáo sau này".

Nguyên tắc vàng: **bé không bao giờ "thua".** Không có game over, không trừ điểm, không hết giờ thua, không nhân vật buồn/khóc khi bé làm sai. Sai thì nhân vật gợi ý nhẹ nhàng và cho thử lại không giới hạn.

---

## === PHẠM VI CỐ ĐỊNH ===

### Thế giới trung tâm: Thị Trấn Bé Bi
• Một bản đồ thị trấn nhỏ nhìn từ trên xuống / góc nghiêng 2.5D, vừa một màn hình, không cần cuộn: một khu xây dựng khối vuông, một sân bay nhỏ, một trạm cứu hỏa, một trường tiểu học, một ngã tư có đèn giao thông, một công viên.
• Mỗi địa điểm là một cửa vào một mini-game. Bé chạm vào nhà nào thì vào game đó. Luôn có nút Ngôi Nhà ở góc để về thị trấn.
• Bố cục cố định (không sinh ngẫu nhiên theo seed — trẻ nhỏ cần quen vị trí). Vị trí các nhà không đổi giữa các lần chơi.
• Một kiểu ánh sáng duy nhất cho lần chạy này: buổi sáng nắng nhẹ, trời xanh, mây trắng, màu tươi sáng. Không có ban đêm, mưa, sương mù.

### 6 mini-game cố định (không thêm, không bớt ở lần chạy này)
1. **Xây Nhà Khối Vuông** (ở Khu Xây Dựng — game chính, bé thích nhất): xếp khối vuông lên lưới 10x8, làm theo bản vẽ mẫu (nhà, tháp, cầu) rồi tự sáng tạo. Đếm khối từng màu, cộng số khối ("3 khối đỏ + 4 khối xanh là mấy khối?"). Có nút "Đếm khối" đọc to số khối đã xếp. 5 loại khối: cỏ, gỗ, gạch, kính, mái.
2. **Phi Công Nhí** (ở Sân Bay): máy bay chở khách — đếm hành khách lên/xuống, cộng/trừ trong 20 ("Có 12 khách, thêm 5 khách nữa là mấy khách?"). Xếp hành lý đúng số hiệu chuyến bay. Học từ tiếng Anh: airplane (máy bay), pilot (phi công), airport (sân bay).
3. **Lính Cứu Hỏa** (ở Trạm Cứu Hỏa): lái xe cứu hỏa tới nhà có khói (lửa nhỏ kiểu hoạt hình, không đáng sợ, không có người bị nạn), chạm để xịt nước dập lửa, đếm số lần xịt. Học số khẩn cấp **114** và 3 bước khi thấy cháy: báo người lớn — gọi 114 — không quay lại lấy đồ.
4. **Toán Vui Cùng Xe** (ở Trường Tiểu Học): phép cộng/trừ trong 20 qua xe cộ ("Xe tải chở 9 khối, bốc thêm 6 khối nữa là mấy khối?"). Trả lời bằng bàn phím số to, có hình xe/khối minh họa phép tính.
5. **Đọc Chữ Cùng Máy Bay** (ở Công Viên): ghép từ đơn tiếng Việt về phương tiện (MÁY BAY, XE LỬA, TÀU THỦY, XE CỨU HỎA) — nghe giọng đọc, chọn chữ đúng. Học thêm từ tiếng Anh: fire truck, train, boat.
6. **An Toàn Giao Thông** (ở Ngã Tư): đèn đỏ dừng, đèn xanh đi. Bé giúp nhân vật qua đường đúng vạch, đội mũ bảo hiểm khi đi xe. Thêm luật xe ưu tiên: khi xe cứu hỏa hú còi thì các xe khác phải nép sang một bên nhường đường, bé giúp xếp xe nép vào lề. Không có xe đâm, không có tai nạn — xe luôn dừng lại chờ bé.

• Mỗi mini-game chơi xong trong 3–5 phút. Chơi xong nhận 1 ngôi sao + lời khen + sticker vào Sổ Sticker (lưu local, tối đa 18 sticker).
• Tổng thời lượng một vòng chơi hết 6 game: 18–25 phút. Có nhắc nghỉ sau 20 phút: nhân vật nói "Bé chơi giỏi quá! Mình nghỉ mắt một chút nhé!" — chỉ nhắc, không khóa game.

---

## === QUY TẮC HÌNH ẢNH (áp dụng cho mọi vật thể và mọi màn hình) ===

• Phong cách: chibi tròn trịa, viền dày mềm, mắt to, má hồng, nụ cười. Không góc nhọn, không bóng tối đáng sợ, không nhân vật mặt buồn/giận.
• Bảng màu tươi sáng, bão hòa vừa: nền pastel (xanh trời nhạt, vàng kem, hồng nhạt), màu nhấn rực cho nút bấm (cam, xanh lá). Tương phản chữ/nền tối thiểu 4.5:1. Không dùng màu neon chói, không dùng nền tối.
• Mọi nút bấm tối thiểu 64 x 64 px trên màn hình điện thoại (bé 6 tuổi tay đã khéo hơn bé 3 tuổi), cách nhau tối thiểu 12 px. Nút chính to gấp 1.5 lần nút phụ. Ô xếp khối vuông tối thiểu 48 x 48 px.
• Chữ: font tròn, không chân, tối thiểu 26 px cho chữ hướng dẫn, 40 px cho số đếm và phép tính. Mỗi câu hướng dẫn tối đa 12 chữ. Bé 6 tuổi đã đọc được từ đơn nên chữ là kênh chính, giọng nói vẫn đọc kèm mọi câu để bé nghe theo.
• Không để màn hình nào trống quá 30%: phải có nhân vật, đồ vật, mây, hoa, cỏ hoặc nút bấm. Mọi màn hình đều có mascot đứng góc dẫn dắt.
• Mọi vật thể đều có bóng mềm dưới chân, viền bo tròn. Không có hình hộp trơn, không có mặt phẳng trống rộng.
• Riêng game Xây Nhà dùng phong cách khối vuông (voxel): mọi vật là khối lập phương xếp chồng, màu rõ từng loại (cỏ xanh, gỗ nâu, gạch đỏ, kính xanh nhạt, mái đỏ). Đây là phong cách khối vuông chung, KHÔNG sao chép texture, nhân vật hay tên gọi của Minecraft.
• Vật thể có ít nhất 2 lớp biến thiên: màu chính + bóng/viền đậm hơn ở mép. Không cần texture bẩn/mòn — game trẻ em phải sạch, sáng, rõ.
• Hậu kỳ rất nhẹ: không bloom, không vignette tối, không nhiễu hạt. Chỉ dùng bóng mềm, bo góc, chuyển động nảy (bounce) khi chạm.
• Kỹ thuật chạy chắc được ưu tiên hơn kỹ thuật tham vọng. Hiệu ứng nào gây lỗi hình thì tắt, không để lỗi trong bản giao. Ưu tiên 2D Canvas / Phaser thay vì 3D nặng.

---

## === MỤC TIÊU HỌC TẬP (thay cho MỤC TIÊU MÀN CHƠI) ===

• Mỗi mini-game có đúng 1 mục tiêu học rõ ràng, ghi ở đầu file spec của game đó. Ví dụ game Xây Nhà Khối Vuông: "Bé đếm khối tới 20 và cộng số khối 2 màu (3 đỏ + 4 xanh = 7)." Ví dụ game Phi Công Nhí: "Bé cộng/trừ trong 20 qua số hành khách lên/xuống máy bay." Ví dụ game Lính Cứu Hỏa: "Bé nhớ số 114 và 3 bước khi thấy cháy."
• Chuẩn đầu ra cả game (bé 6 tuổi, lớp 1): đếm thành thạo 1–20, cộng/trừ trong 20 có minh họa hình ảnh, đọc được 10–15 từ đơn về phương tiện, biết 6–8 từ tiếng Anh về phương tiện, nhớ số 114 và luật đèn giao thông + xe ưu tiên.
• Không có điểm số cạnh tranh, không có bảng xếp hạng, không có đếm ngược gây áp lực. Chỉ có: ngôi sao (tối đa 3 sao/game), sticker, lời khen bằng giọng nói.
• Lời khen luân phiên, không lặp một câu: "Giỏi quá!", "Bé làm đúng rồi!", "Hoan hô bé!", "Bé thông minh quá!".
• Màn hình chính là thị trấn nhìn toàn cảnh, có tên game, nút Chơi (to nhất, ở giữa dưới), nút Sổ Sticker, nút Phụ Huynh (có cổng phụ huynh, xem mục AN TOÀN TRẺ EM). Không có nút Settings lộ ra cho bé bấm.
• Bé làm sai 2 lần liên tiếp ở cùng một chỗ thì game tự gợi ý rõ hơn: vật đúng nhấp nháy + giọng nói chỉ "Bé thử chạm vào quả táo đỏ nhé!" — không bao giờ hiện chữ "Sai rồi". Với phép tính, gợi ý bằng hình: hiện đúng số khối/hành khách để bé đếm lại.

---

## === NHÂN VẬT ===

Nhân vật tự sáng tạo, không giống BabyBus, không giống Minecraft:

• **Gấu Bo** (mascot chính): gấu nâu nhỏ, áo yếm xanh, đổi mũ theo game — mũ bảo hộ vàng ở game Xây Nhà, mũ phi công ở game Máy Bay, mũ cứu hỏa đỏ ở game Cứu Hỏa. Dẫn dắt toàn bộ game, nói lời hướng dẫn và lời khen. Luôn xuất hiện ở góc màn hình, nhảy lên khi bé làm đúng.
• **Mèo Mun** (bạn đồng hành): mèo đen nhỏ đeo nơ đỏ, xuất hiện trong game Toán Vui và game Đọc Chữ, làm ví dụ mẫu ("Mun chọn đáp án 7 nè!").
• **Thỏ Cà Rốt**: thỏ trắng tai dài, làm thợ xây trong game Xây Nhà Khối Vuông (đội mũ bảo hộ, cầm bản vẽ mẫu).
• **Cú Mèo Phi Công**: cú mèo đeo kính phi công, hướng dẫn game Phi Công Nhí và dạy từ tiếng Anh về máy bay.
• **Chó Đốm Cứu Hỏa**: chó đốm đội mũ cứu hỏa đỏ, hướng dẫn game Lính Cứu Hỏa và dạy số 114.
• Mỗi nhân vật có 4 biểu cảm: vui, hào hứng, suy nghĩ (nghiêng đầu), cổ vũ (giơ tay). Không có biểu cảm buồn, giận, sợ.
• Chuyển động: đi bộ nảy nhẹ, nhảy lên khi khen, vẫy tay chào khi vào game, vỗ tay khi hoàn thành. Tất cả chuyển động bằng code / sprite đơn giản, không cần xương phức tạp.
• Không có "đối thủ", không có nhân vật phản diện, không có rượt đuổi, không có yếu tố đáng sợ. Lửa trong game Cứu Hỏa là ngọn lửa nhỏ kiểu hoạt hình, không lan, không có khói đen dày hay người bị nạn.

---

## === TƯƠNG TÁC VÀ CẢM GIÁC CHẠM (phần quan trọng nhất, thay cho SÚNG VÀ CẢM GIÁC BẮN) ===

Mọi tương tác đều là chạm/kéo trên màn hình cảm ứng, chuột vẫn dùng được. Các số dưới đây là giá trị khởi điểm, để trong một file cấu hình `config/interaction.json`.

• 4 thao tác: **chạm** (tap), **kéo** (drag), **kéo-thả** (drag & drop), **chọn đáp án số** trên bàn phím số to (cho game toán). Không có thao tác vuốt nhanh, chạm 2 ngón, giữ lâu quá 1 giây, hay phím tắt bắt buộc.
• Phản hồi chạm trong 100 ms: vật được chạm nảy lên (scale 1.0 → 1.2 → 1.0 trong 0.3 giây) + phát tiếng "bụp" vui + rung nhẹ (nếu thiết bị hỗ trợ, rung 15 ms).
• Xếp khối: chạm ô trống để đặt khối đang chọn, chạm khối đã đặt để gỡ. Đặt khối có tiếng "cộp" chắc + khối nảy nhẹ. Kéo ngang để đặt nhiều khối liên tiếp.
• Kéo-thả: vật đi theo ngón tay, vùng thả đúng sáng lên khi vật đến gần trong 80 px. Thả đúng: vật khớp vào với hiệu ứng lấp lánh + tiếng chuông. Thả sai: vật bay về chỗ cũ trong 0.4 giây, không có tiếng chê.
• Nút bấm có 3 trạng thái rõ ràng: bình thường, đang chạm (tối lại 10% + nhỏ lại 5%), đã tắt (mờ 50%, không bấm được).
• Không có thao tác nào cần độ chính xác cao: vùng chạm rộng hơn hình ảnh 20% mỗi phía. Bé chạm gần đúng vẫn tính đúng.
• Mọi màn hình đều có nút Quay Lại (mũi tên to, góc trái trên) và nút Ngôi Nhà (góc phải trên). Bé không bao giờ bị kẹt ở màn hình nào.
• Chuyển màn: trượt ngang mềm 0.4 giây, không nhấp nháy, không chuyển cảnh đột ngột.
• Di chuyển nhân vật trong thị trấn: bé chạm vào nhà là nhân vật tự chạy tới đó (tốc độ vừa phải, 2 giây là tới). Bé không cần điều khiển nhân vật đi bộ bằng joystick.

---

## === VẬT LÝ VÀ VA CHẠM (đơn giản hóa) ===

• Không cần thư viện vật lý WASM nặng. Chỉ cần va chạm hình chữ nhật / hình tròn đơn giản cho kéo-thả và chạm.
• Vật kéo-thả: khi thả trong vùng đích (bán kính 60 px quanh tâm đích) thì tính là đúng. Không có rơi, nảy vật lý phức tạp.
• Xếp khối: khối chỉ đặt được lên ô lưới hoặc chồng lên khối khác (không lơ lửng giữa không trung — nếu bé đặt khối trên cao mà dưới trống thì khối tự rơi xuống ô thấp nhất, kèm tiếng "bịch" vui).
• Không có nhân vật lọt sàn, kẹt góc — vì game 2D màn hình cố định, không có thế giới 3D tự do di chuyển.
• Vật phá được: không có. Không phá đồ, không vỡ kính. Thay vào đó là vật "tương tác vui": chạm vào hoa thì hoa nở, chạm vào mây thì mây bay, chạm vào máy bay thì máy bay bay một vòng.

---

## === HOẠT ẢNH VÀ HIỆU ỨNG ===

• Nhân vật: đi bộ nảy, nhảy khen, vẫy tay, vỗ tay, nghiêng đầu suy nghĩ. Chuyển giữa các động tác bằng pha trộn 0.2 giây, không giật khung.
• Môi trường: mây trôi chậm, máy bay bay ngang thị trấn mỗi 30 giây, xe cứu hỏa chạy quanh công viên, hoa đung đưa, bướm bay quanh. Tất cả chuyển động chậm, nhẹ nhàng, không gây chóng mặt.
• Hạt có giới hạn: sao lấp lánh khi làm đúng (tối đa 20 hạt), bong bóng khi xịt nước cứu hỏa, tim bay khi khen. Không có khói đen, lửa lớn, vụ nổ.
• Hoàn thành game: pháo giấy màu + nhân vật nhảy + nhạc chiến thắng 3 giây + sticker bay vào sổ.
• Màn hình: không có viền đỏ, không mờ/mất màu, không rung màn hình. Khi bé làm đúng, viền màn hình lóe sáng vàng nhẹ 0.5 giây.

---

## === ÂM THANH VÀ GIỌNG NÓI (Web Audio + Web Speech API) ===

• Giọng hướng dẫn tiếng Việt là bắt buộc: dùng Web Speech API giọng vi-VN (ưu tiên giọng nữ, tốc độ 0.9, cao độ 1.1 cho thân thiện). Mọi câu hướng dẫn, câu hỏi, phép tính và lời khen đều có giọng nói. Từ tiếng Anh đọc bằng giọng en-US (ví dụ "airplane"). Nếu trình duyệt không có giọng vi-VN thì dùng giọng mặc định + hiện chữ to.
• Nhạc nền: vui tươi, chậm (80–100 BPM), âm lượng mặc định 30%, không lời. Mỗi mini-game có 1 giai điệu riêng nhưng cùng tông vui. Có nút tắt nhạc riêng, tắt giọng riêng trong khu Phụ Huynh.
• Hiệu ứng tiếng tổng hợp bằng Web Audio (không cần file nhạc ngoài): tiếng "bụp" khi chạm, tiếng "cộp" khi đặt khối, tiếng chuông khi đúng, tiếng còi xe cứu hỏa nhẹ nhàng (không chói), tiếng máy bay vút qua, tiếng lấp lánh khi nhận sao.
• Âm lượng: có limiter ở đầu ra, không mẫu nào vượt ngưỡng. Âm thanh không bao giờ giật mình (không tiếng to đột ngột, không tiếng còi chói).
• Có công tắc Tắt Tất Cả Âm Thanh trên màn hình chính (biểu tượng loa to, bé bấm được).

---

## === AN TOÀN TRẺ EM (MỚI — bắt buộc, kiểm trước khi giao) ===

• **Cổng phụ huynh:** nút Phụ Huynh yêu cầu giữ 3 giây + trả lời 1 phép tính đơn giản (ví dụ 3 + 4 = ?) mới mở. Trong khu Phụ Huynh mới có: tắt nhạc, tắt giọng, xóa tiến trình, xem thời gian chơi, link giới thiệu (không mở trình duyệt ngoài khi bé đang chơi).
• **Không thu thập dữ liệu:** không cookie theo dõi, không analytics gửi ra ngoài, không quảng cáo, không SDK bên thứ ba. Tiến trình chỉ lưu trong localStorage / IndexedDB trên máy bé.
• **Không nội dung không phù hợp:** không bạo lực, không máu, không nhân vật sợ hãi, không chữ chửi thề, không hình ảnh người lạ, không yêu cầu bé nhập tên/thông tin cá nhân. Tên bé (nếu có) chỉ là biệt danh tự chọn, lưu local, không bắt buộc. Nội dung cháy chỉ dạy an toàn, không miêu tả tai nạn hay người bị thương.
• **Thời gian chơi:** sau 20 phút liên tục, hiện nhắc nghỉ bằng giọng nói + hình ảnh dịu dàng. Sau 40 phút, nhắc lần 2. Không khóa game đột ngột.
• **Kiểm tra bằng tay:** trước khi giao, người lớn chơi thử toàn bộ 6 game, xác nhận không có chỗ nào bé có thể bấm ra ngoài, mua hàng, hay thấy nội dung lạ.

---

## === VAI TRÒ ===

• Bạn (model mạnh nhất) là đạo diễn: lập kế hoạch, viết hồ sơ nhân vật/vật thể, tự tay dựng thị trấn mẫu và 2 mini-game mẫu đầu tiên, gộp code, quyết định dừng.
• Agent dựng chạy CÙNG model mạnh nhất. Agent dựng chỉ vào việc sau khi mẫu chuẩn đã đạt điểm: nhân rộng vật thể/mini-game theo mẫu, chạy test, chụp ảnh, đo hiệu năng. Không giao cho model rẻ việc nào chưa có mẫu để đối chiếu. Song song tối đa 4 agent. Mỗi agent nhận bản giao việc tự đủ: mục tiêu học, hồ sơ, quy tắc hình ảnh, file được sửa, cách tự kiểm.
• Agent phản biện chạy model mạnh, ngữ cảnh mới, chỉ nhận ảnh chụp, hồ sơ và thang điểm, không xem code. Nhiệm vụ của nó là tìm lỗi — đặc biệt lỗi "bé không hiểu phải làm gì", nút quá nhỏ, chữ quá nhỏ, màu khó nhìn, phép tính sai đáp án. Điểm của nó là điểm chính thức; bạn không tự chấm đạt cho sản phẩm mình đã gộp.
• Thêm một vai: **người kiểm trẻ em** (do bạn đóng vai): xem mỗi màn hình với mắt của bé 6 tuổi — chỉ nhìn hình, đọc từ đơn và nghe giọng, có hiểu phải làm gì trong 5 giây không? Nếu không hiểu trong 5 giây thì màn hình đó chưa đạt.

---

## === BƯỚC 0. HẠ TẦNG ===

• Vite + TypeScript, Phaser 3 (bản mới nhất, khóa phiên bản) cho game 2D, chạy được trên trình duyệt di động và máy tính. Đọc tài liệu hiện hành, không dựa vào trí nhớ. Nếu Phaser không phù hợp thì dùng Canvas 2D thuần + TypeScript, ghi lý do vào DECISIONS.md. Không dùng Three.js / WebGPU cho game này — quá nặng cho máy tính bảng cũ của trẻ.
• Tách module: game (logic từng mini-game, tick cố định, không import Phaser trực tiếp trong logic học), render, audio (giọng nói + nhạc), input (chạm/kéo thống nhất), ui, storage (localStorage).
• Sim/logic học viết bằng TypeScript, một bản duy nhất. Logic học tất định: cùng thao tác thì ra cùng kết quả; có test kiểm điều này. Riêng bộ sinh phép tính phải có test chứng minh đáp án luôn đúng và nằm trong 0–20.
• Trang xem vật thể/nhân vật: có thước đo kích thước nút (px), xem ở 3 cỡ màn hình: điện thoại 390px, máy tính bảng 768px, máy tính 1280px.
• Script chụp tự động bằng trình duyệt không giao diện: mỗi màn hình chụp ở 3 cỡ màn hình, kèm kiểm tra nút bấm có đủ 64px không. Kiểm ngay rằng ảnh chụp ra không đen và không lỗi; nếu không chụp được thì sửa cho xong trước khi làm bất cứ gì khác.
• Trang thử tương tác: thử chạm/kéo/đặt khối 30 lần, đo độ trễ phản hồi (phải < 100 ms).
• File nhớ: PLAN.md, PROGRESS.md, DECISIONS.md, LESSONS.md. Cập nhật sau mỗi mốc.

---

## === BƯỚC 1. HỒ SƠ NHÂN VẬT & VẬT THỂ ===

Với mỗi nhân vật/vật thể, tìm trên web 3–5 ảnh tham khảo phong cách chibi trẻ em để học hình dáng và màu sắc (chỉ để học, không đưa ảnh vào game, không sao chép nhân vật có sẵn), rồi viết specs/<tên>.md: kích thước theo px, màu chính/phụ, biểu cảm, chuyển động, âm thanh đi kèm, ngân sách dung lượng.
Danh sách cố định, 12 mục: Gấu Bo (3 bộ mũ: bảo hộ, phi công, cứu hỏa), Mèo Mun, Thỏ Cà Rốt thợ xây, Cú Mèo Phi Công, Chó Đốm Cứu Hỏa, bộ khối vuông (cỏ/gỗ/gạch/kính/mái), máy bay + sân bay, xe cứu hỏa + trạm cứu hỏa, bộ số 1–20 + phép tính, bộ từ đơn + từ tiếng Anh phương tiện, bối cảnh thị trấn (khu xây dựng/sân bay/trạm cứu hỏa/trường học), bộ nút bấm + HUD trẻ em, bộ sticker (18 mẫu).

---

## === BƯỚC 2. THỊ TRẤN MẪU VÀ CỔNG DỪNG SỚM ===

• Trước khi dựng cả 6 game, dựng thị trấn + 1 mini-game mẫu (Xây Nhà Khối Vuông — game bé thích nhất) ở chất lượng cuối cùng: đủ nhân vật, giọng nói, nhạc, nút bấm, hiệu ứng khen.
• Bạn tự tay dựng bằng model mạnh nhất, không giao cho model rẻ. Làm 3 phương án bảng màu khác nhau cho cùng thị trấn. Agent phản biện chấm cả ba, bạn giữ phương án điểm cao nhất và cải tiến tiếp trên nó.
• Lặp tới khi 4 ảnh chụp (thị trấn + 3 màn trong game Xây Nhà Khối Vuông) đều đạt từ 8/10 trở lên ở mọi mục. Tối đa 5 vòng.
• CỔNG DỪNG SỚM: hết 5 vòng mà điểm trung bình dưới 7 thì dừng toàn bộ, viết báo cáo kèm ảnh và nguyên nhân. Không dựng tiếp trên nền chưa đạt.
• Khi đạt, ghi lại thông số màu sắc, font, kích thước nút, âm thanh thành STYLE.md. Mọi mini-game sau phải theo file này.
• MẪU CHUẨN: bạn cũng tự tay dựng và đưa qua vòng chấm 4 thứ khó nhất: Gấu Bo (kèm 3 bộ mũ + 4 biểu cảm + nhảy khen), game Xây Nhà Khối Vuông (kèm đếm khối + phản hồi chạm), bộ nút bấm + bàn phím số trẻ em, và hệ thống giọng nói tiếng Việt.

---

## === BƯỚC 3. VÒNG DỰNG, CHỤP, CHẤM (cho từng mini-game còn lại) ===

• Agent dựng làm 5 mini-game còn lại thành module thuần, mỗi game 1 thư mục riêng. Bản giao việc kèm code của mẫu chuẩn gần nhất, ảnh đạt điểm của nó và STYLE.md; agent phải dùng lại bộ nhân vật/nút/âm thanh chung, không tự tạo phong cách mới.
• Chụp mỗi game ở 3 cỡ màn hình + 2 góc (màn bắt đầu, màn chơi giữa chừng, màn hoàn thành).
• Agent phản biện cho điểm 1–10 từng mục: bé có hiểu phải làm gì trong 5 giây không, nút đủ to không, chữ đủ to không, màu sắc hợp STYLE.md không, giọng nói rõ ràng không, phép tính/từ vựng có chính xác không, mục tiêu học có đạt không, hiệu năng. Kèm nhận xét chỉ rõ vị trí và cách sửa.
• Dưới 8 ở bất kỳ mục nào thì làm lại, tối đa 5 vòng. Hết vòng mà chưa đạt thì giữ bản tốt nhất và ghi vào báo cáo.
• Game Lính Cứu Hỏa và An Toàn Giao Thông được 8 vòng thay vì 5 (vì liên quan an toàn, phải chính xác nội dung: số khẩn cấp 114, 3 bước khi thấy cháy, đèn đỏ dừng tuyệt đối, xe cứu hỏa được ưu tiên).
• Sau mỗi game, ghi lỗi lặp lại và câu chỉ dẫn đã sửa được nó vào LESSONS.md, cập nhật mẫu giao việc trước khi giao game tiếp theo. Agent thất bại 2 lần trên cùng một lỗi thì chuyển việc đó lên model mạnh.

---

## === BƯỚC 4. GHÉP THỊ TRẤN VÀ ÂM THANH ===

• Ghép thị trấn + 6 game + Sổ Sticker + khu Phụ Huynh thành một app hoàn chỉnh. Điều hướng không bao giờ kẹt.
• Làm toàn bộ phần ÂM THANH VÀ GIỌNG NÓI.
• Agent phản biện chấm 10 ảnh chụp ở các vị trí cố định, trong đó có màn hình chính (thị trấn) và màn chơi của mỗi game. Cùng thang điểm, tối đa 5 vòng.

---

## === BƯỚC 5. LUẬT CHƠI & AN TOÀN ===

• Làm toàn bộ phần TƯƠNG TÁC, HOẠT ẢNH, MỤC TIÊU HỌC TẬP, AN TOÀN TRẺ EM.
• Giao diện: màn hình chính, khu Phụ Huynh (có cổng), Sổ Sticker, HUD tối giản (chỉ có nút Nhà, nút Loa, nút Quay Lại). Không có Settings lộ ra cho bé.
• Test tự động: logic đếm khối tới 20, phép cộng/trừ trong 20 (đáp án luôn đúng, nằm trong 0–20), logic kéo-thả đúng/sai, logic gợi ý sau 2 lần sai, nội dung an toàn cháy (số 114, 3 bước), cổng phụ huynh, lưu/tải sticker, nhắc nghỉ sau 20 phút, tắt tiếng.

---

## === BƯỚC 6. CHƠI THỬ TỰ ĐỘNG ===

• Viết bot điều khiển qua đúng lớp input thật (chạm/kéo giả lập). Bot chơi hết 6 game, mỗi game 2 lần (1 lần làm đúng hết, 1 lần cố tình làm sai để kiểm gợi ý), trên trình duyệt không giao diện.
• Điều kiện qua: không lỗi nào trong console, không kẹt màn hình quá 3 giây, mọi game đều hoàn thành được, gợi ý hiện đúng sau 2 lần sai, sticker lưu đúng.
• Trong lúc bot chơi, chụp 1 ảnh mỗi 5 giây. Agent phản biện xem cả chuỗi ảnh để tìm lỗi hình, nút đè nhau, chữ tràn, vật lơ lửng. Sửa hết rồi chạy lại.
• Hiệu năng: mục tiêu 60 khung hình/giây ở mức Vừa trên máy tính bảng tầm trung và điện thoại Android 3–4 năm tuổi. Đo trên Chrome (Android) và Safari (iPad) thật nếu có. Nếu chỉ đo được bằng trình duyệt không giao diện thì ghi rõ máy thật là CHƯA ĐO.
• Ngân sách tải, từ lúc mở trang tới khung hình đầu: lần đầu không quá 3 giây trên mạng 4G, lần sau (đã có bộ nhớ đệm) không quá 1.5 giây. Khựng dài nhất trong 5 giây đầu không quá 100 ms.
• Có sẵn công tắc đo từng bước tải (tải file, tải giọng nói, dựng cảnh). Trước khi tối ưu phải đo và chỉ ra bước nào chậm; không tối ưu theo phỏng đoán.
• Tài nguyên (hình ảnh, âm thanh) sinh bằng code hoặc vẽ vector thì lưu vào IndexedDB, khóa theo mã nguồn hàm sinh và tham số.

---

## === BƯỚC 7. KIỂM HÌNH & KIỂM TRẺ EM TỰ ĐỘNG ===

Các phép kiểm sau chạy bằng script và phải ra 0 lỗi trước khi đưa ảnh cho agent phản biện ở bước 4 và bước 6.
• Mọi nút bấm đo được tối thiểu 64 x 64 px ở cỡ điện thoại 390px; không nút nào nhỏ hơn. Ô khối vuông tối thiểu 48 x 48 px.
• Mọi chữ hướng dẫn tối thiểu 26 px; số đếm và phép tính tối thiểu 40 px.
• Không chữ nào tràn khỏi nút hoặc khỏi màn hình ở cả 3 cỡ màn hình.
• Không hai nút nào đè nhau; khoảng cách giữa các nút tối thiểu 12 px.
• Mọi màn hình đều có nút Quay Lại + nút Ngôi Nhà, và đều bấm được.
• Không vật lơ lửng; không khối nào lơ lửng giữa không trung mà dưới trống.
• Kiểm ở cả ba cỡ màn hình. Lỗi chỉ hiện ở điện thoại nhỏ vẫn là lỗi.
• Kiểm giọng nói: mọi câu hướng dẫn đều có file/câu lệnh giọng nói tương ứng, không câu nào chỉ có chữ.
• Kiểm nội dung: mọi phép tính có đáp án đúng trong 0–20; số khẩn cấp hiển thị luôn là 114, không số khác.

---

## === BƯỚC 8. TRIỂN KHAI (chỉ làm khi người dùng đã cấp tên miền) ===

• Làm theo mục TRIỂN KHAI. Sau khi lên, mở bản đang chạy thật bằng trình duyệt không giao diện: vào được game, chơi được 1 mini-game tới lúc nhận sao, không lỗi console, rồi mới báo xong.
• Chưa có tên miền thì bỏ qua bước này và ghi vào báo cáo; không tự chọn nơi đăng.

---

## === PHÂN BỔ CÔNG SỨC ===

• Khoảng 35% cho nhân vật, màu sắc, thị trấn mẫu và giọng nói; 30% cho 6 mini-game và tương tác chạm; 15% cho âm thanh và hiệu ứng khen; 20% cho phần còn lại (an toàn trẻ em, phụ huynh, test, triển khai).
• Giới hạn tổng: 70 lượt agent dựng, 40 lượt agent phản biện. Chạm giới hạn thì dừng và báo cáo.
• Không sang bước sau khi bước trước chưa chạy được.

---

## === TRIỂN KHAI ===

• Sản phẩm là một thư mục file tĩnh (PWA offline càng tốt: có manifest + service worker để chơi offline sau lần tải đầu). Không có máy chủ riêng, không container, không đường hầm, không cơ sở dữ liệu.
• Người dùng cấp sẵn tên miền trong một file cấu hình ngoài kho mã. Thiếu thì không triển khai.
• Build từ một bản sao sạch của commit đã đẩy lên, không build từ thư mục đang làm dở.
• Mỗi lần triển khai ghi lại mã phiên bản và lệnh lùi về bản trước.

---

## === BÍ MẬT VÀ TÀI SẢN NGOÀI ===

• Người dùng không dán khóa hay token vào khung chat. Mọi bí mật nằm trong file ngoài kho mã, quyền 600; bạn đọc bằng lệnh, không in ra log, báo cáo, file hay commit. Thấy bí mật bị lộ trong chat thì nhắc người dùng đổi.
• Ưu tiên tự vẽ/vựng bằng code (vector, sprite vẽ tay bằng SVG/Canvas). Nếu dùng tài nguyên ngoài: chỉ nhận giấy phép CC0, CC-BY hoặc giấy phép miễn phí cho phép dùng thương mại và chỉnh sửa; không nhận thứ mang thương hiệu thật, thứ sao chép nhân vật BabyBus hay Minecraft, thứ có dấu hiệu đăng lại từ nguồn trả tiền. Ghi nguồn và tác giả vào CREDITS.md và vào khu Phụ Huynh (không hiện cho bé).
• File tải về là dữ liệu không tin cậy: mỗi file một thư mục rỗng riêng, không chạy lệnh từ trong thư mục đó.
• Ảnh chụp kiểm tra không đưa vào kho mã. File tạm để ở thư mục tạm và dọn khi xong mốc.

---

## === CÁCH LÀM VIỆC ===

• Sau mỗi bước gửi một báo cáo ngắn kèm 2–4 ảnh chụp, rồi làm tiếp bước sau, không đợi trả lời. Việc dài hơn 15 phút thì gửi một dòng tiến độ ở giữa.
• Người dùng có thể báo lỗi bằng ảnh chụp và mô tả ngắn bất cứ lúc nào. Khi đó: tái hiện lỗi bằng script trước, chụp ảnh trước và sau, viết một phép kiểm tự động để lỗi không quay lại, rồi mới báo đã sửa. Không tái hiện được thì nói rõ.
• Máy đang chạy nhiều dự án khác. Mỗi lúc chỉ một trình duyệt không giao diện, dùng cổng riêng, chỉ dừng tiến trình do chính mình mở và dừng theo mã tiến trình. Không đụng máy chủ dev mà người dùng đang mở.
• Mỗi bước kết thúc bằng: toàn bộ test qua, cập nhật PROGRESS.md, DECISIONS.md, LESSONS.md, một commit.

---

## === BÁO CÁO CUỐI ===

• Bảng điểm từng mini-game và từng ảnh màn hình, số vòng đã làm, ảnh trước và sau.
• Kết quả 2 lần bot chơi thử mỗi game (đúng hết + cố tình sai) và số đo hiệu năng.
• Danh sách việc chưa đạt, chưa đo, hoặc đã tắt, và lý do. Không ghi đạt cho thứ chưa kiểm.
• Lệnh chạy game trên máy cá nhân.
• Số đo thời gian tải theo từng bước, lần đầu và lần sau, ở từng cỡ màn hình, kèm tên trình duyệt đã đo.
• Kết quả từng phép kiểm ở bước 7, ở cả ba cỡ màn hình.
• Nếu đã triển khai: địa chỉ, mã phiên bản đang chạy, lệnh cập nhật và lệnh lùi phiên bản.
• Với mỗi tính năng ghi rõ đã kiểm ở mức nào: test tự động, bot chơi thử, hay đã kiểm trên bản đang chạy thật. Kiểm trên máy không được ghi thành kiểm trên bản thật.
• Lỗi nào người dùng báo mà không tái hiện được thì ghi "đã sửa nguyên nhân có khả năng nhất, chưa chứng minh", không ghi "đã sửa".
• Mục tiêu học của từng game + cách kiểm tra bé đã học được (ví dụ: bé đếm khối đúng tới 20 và làm đúng 4/5 phép cộng trong 20 sau 3 lần chơi).
