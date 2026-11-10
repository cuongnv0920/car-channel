# Storyboard — Video #1 Hộp số tự động / bánh răng hành tinh

> Bản nháp 1, 2026-11-10. Đầu vào: kịch bản bản nháp 3 (đã qua fact-check và **Cổng duyệt #1**). Chưa qua Cổng duyệt #2.
> Tổng thời lượng: **08:04** (484 giây), theo ước tính 150 từ/phút; sẽ khớp lại sau khi có giọng đọc thật.

## Tóm tắt loại hình
| Loại | Số shot | Tổng thời lượng | Ghi chú |
|---|---|---|---|
| ANIMATION-CODE | 14 | 351s (73%) | Mọi cơ chế, công thức, sơ đồ; không tốn credits |
| ĐỒ HỌA | 6 | 86s (18%) | Thẻ chữ, timeline; không tốn credits |
| AI-IMAGE | 4 | 39s (8%) | Bối cảnh lịch sử, Ken Burns |
| AI-VIDEO | 2 | 8s (2%) | Chỉ 2 clip ngắn (hook, kết) |

## Style
Style tạm (brand/style.md chưa có): nền navy #0B1220; mặt trời vàng #FFD23F, giá hành tinh xanh #19B5FF, vành cam #FF8A00; chữ trắng đậm, nhãn tiếng Việt kèm tên gốc.
`brand/style.md` **chưa tồn tại**; đây là giá trị tạm lấy từ gợi ý trong `brand/README.md` (blueprint kỹ thuật + điện ảnh tối) và quy ước màu theo ý nghĩa. Cần bạn chốt brand trước khi sinh ảnh/clip thật.

## Ràng buộc ngân sách (gói Starter)
- **Số dư Higgsfield hiện tại: 0 credits, gói free** (kiểm ngày 2026-11-10). Cần đăng ký Starter trước khi sinh.
- **Chưa có bảng giá credits** từ công cụ (không hiện giá từng lượt sinh), nên **không đưa con số credits cụ thể**. Thay vào đó đặt **trần theo số lượt sinh**:
  - AI-IMAGE: tối đa **4 ảnh chính + 4 ảnh thử/dự phòng** (1k, 16:9).
  - AI-VIDEO: tối đa **2 clip, mỗi clip 4 giây**, luôn làm bản nháp 480p trước rồi mới hoàn thiện nếu đạt.
  - Nếu chi phí thật vượt ngân sách bạn đặt, đổi AI-VIDEO sang AI-IMAGE (Ken Burns), rồi đổi AI-IMAGE sang ĐỒ HỌA.
- Mọi phần giải thích cơ khí dùng ANIMATION-CODE. **Prompt AI không mô tả bánh răng, trục hay hộp số**; chỉ bối cảnh.

## "Thử trước" (theo thứ tự, trước khi sinh hàng loạt)
1. Sinh **1 ảnh thử** (shot 3.1) ở 1k; kiểm tra xe đúng thời đại, không có chữ/logo lạ; ghi lại credits đã tiêu (so số dư trước và sau).
2. Sinh **1 clip nháp 480p** (shot 1.1); kiểm tra tay, cần số, không có mặt/biển số đọc được; ghi lại credits.
3. Từ hai con số thật, tính **tổng chi phí dự kiến** cho phần còn lại, so với ngân sách, rồi mới sinh tiếp.
4. Prototype bánh răng hành tinh (Remotion) với Zs=18, Zr=72, Zp=27: kiểm tra **ăn khớp hình học (Zr = Zs + 2·Zp)** và các tỉ số 5; 1,25; −4; 1 khớp với mô phỏng quay. (Quan hệ hình học này chưa có nguồn trong research; cần kiểm bằng chính mô phỏng.)

## Thành phần Remotion cần dựng (tái sử dụng)
GearSetModel (props: Zs, Zr, Zp, bộ phận bị giữ, đầu vào, đầu ra, tốc độ vào) · RatioReadout · PedalDiagram · BandDrum · PinSlotPair · BlockDiagram · SimpsonSchematic · TimelineCard · TitleCard · Subtitle · Speedometer.
GearSetModel phục vụ các cảnh 1, 4, 6, 7, 8, 9, 10, 11, 13 (khoảng 273s tổng), nên là việc đầu tiên.

## Bảng shot
| Cảnh | Shot | Bắt đầu | Thời lượng | Loại | Mô tả | Credits ước tính |
|---|---|---|---|---|---|---|
| 1 | 1.1 | 00:00 | 4s | AI-VIDEO | Cận cảnh tay gạt cần số tự động về D trong xe ban đêm, ánh đèn táp-lô cam–xanh. Chỉ thấy bên ngoài, không thấy cơ cấu bên trong. | 1 clip (làm bản nháp 480p trước) |
| 1 | 1.2 | 00:04 | 8s | ANIMATION-CODE | Mô hình bánh răng hành tinh quay chậm trên nền tối (cắt từ cảnh 7). | 0 |
| 1 | 1.3 | 00:12 | 6s | ĐỒ HỌA | Thẻ 'Antikythera, thế kỷ 2–1 TCN' kèm sơ đồ minh họa cặp bánh răng chốt–rãnh (ghi chữ 'minh họa', không phải ảnh hiện vật). | 0 |
| 1 | 1.4 | 00:18 | 24s | ANIMATION-CODE | Chữ câu hỏi hiện từng dòng ('Vì sao giữ yên một bộ phận mà mọi thứ đổi khác?') trên mô hình bánh răng, zoom dần. | 0 |
| 2 | 2.1 | 00:42 | 18s | ANIMATION-CODE | Cặp bánh răng chốt–rãnh gắn trên bánh răng khác: kim 'Mặt Trăng' chạy lúc nhanh lúc chậm; thước tốc độ bên cạnh. Nhãn 'minh họa'. | 0 |
| 2 | 2.2 | 01:00 | 12s | ANIMATION-CODE | Biến đổi mượt từ cặp chốt–rãnh sang sơ đồ ba vòng tròn (mặt trời, hành tinh, vành). | 0 |
| 3 | 3.1 | 01:12 | 8s | AI-IMAGE | Ảnh minh họa xe hơi những năm 1900 trên đường đất, tông phim ấm, chuyển động Ken Burns nhẹ. Gắn nhãn 'ảnh minh họa do AI tạo'. | 1 ảnh (1k) |
| 3 | 3.2 | 01:20 | 10s | ĐỒ HỌA | Dòng thời gian: Lanchester (xe sản xuất đầu tiên), Wilson-Pilcher (đầu những năm 1900), Ford Model T (1908). | 0 |
| 3 | 3.3 | 01:30 | 8s | AI-IMAGE | Xe tourer đầu thế kỷ 20 kiểu Model T (kiểm hình dáng thủ công; nếu sai dùng ảnh tư liệu công khai, kiểm bản quyền). Ken Burns. | 1 ảnh (1k) + 1 dự phòng |
| 4 | 4.1 | 01:38 | 30s | ANIMATION-CODE | Ba bàn đạp nhãn tiếng Việt: trái (hết cỡ = thấp, nửa chừng = trung gian, nhả = cao), giữa = lùi, phải = phanh hộp số. Hoạt họa từng trạng thái. | 0 |
| 4 | 4.2 | 02:08 | 13s | ANIMATION-CODE | Dải phanh (band) siết quanh trống, một phần bộ bánh răng bị dừng; chú thích 'phần bị dừng quyết định số'. | 0 |
| 5 | 5.1 | 02:21 | 8s | AI-IMAGE | Phòng thiết kế kỹ thuật thập niên 1930, bàn vẽ, ánh đèn vàng, Ken Burns. Gắn nhãn AI. | 1 ảnh (1k) |
| 5 | 5.2 | 02:29 | 20s | ĐỒ HỌA | Dòng thời gian: đầu những năm 1930 (nhóm Thompson bắt đầu), 1937 (Oldsmobile bán tự động, vẫn cần bàn đạp ly hợp), 1939/1940 (Hydra-Matic). | 0 |
| 5 | 5.3 | 02:49 | 15s | AI-IMAGE | Xe sedan Mỹ kiểu cuối thập niên 1930 trên phố, hoàng hôn, Ken Burns. Gắn nhãn AI; không nhận là Oldsmobile thật. | 1 ảnh (1k) + 1 dự phòng |
| 6 | 6.1 | 03:04 | 22s | ANIMATION-CODE | Sơ đồ khối: động cơ, khớp nối thủy lực, ba bộ hành tinh, trục ra; chữ 'Khớp nối thủy lực ≠ biến mô'; mô-men không tăng. | 0 |
| 6 | 6.2 | 03:26 | 14s | ĐỒ HỌA | Thẻ chữ 'Hàng trăm nghìn chiếc' và hai thẻ tên xe tăng M5 Stuart, M24 Chaffee (chỉ chữ, không vẽ xe). | 0 |
| 7 | 7.1 | 03:40 | 37s | ANIMATION-CODE | Mô hình rã rời: mặt trời (vàng), giá hành tinh (xanh), vành răng (cam), nhãn tiếng Việt kèm tên gốc; chỉ ra đầu vào, đầu ra, bộ phận bị giữ. | 0 |
| 8 | 8.1 | 04:17 | 35s | ANIMATION-CODE | Giữ vành (biểu tượng khóa). Mặt trời vào, giá ra. Hai bộ đếm vòng: 5 vòng mặt trời = 1 vòng giá. Công thức 1 + Zr/Zs = 1 + 72/18 = 5,0. | 0 |
| 9 | 9.1 | 04:52 | 21s | ANIMATION-CODE | Giữ mặt trời. Vành vào, giá ra. Công thức 1 + Zs/Zr, thanh so sánh với cảnh 8: giá trị nằm giữa 1 và 2. | 0 |
| 10 | 10.1 | 05:13 | 28s | ANIMATION-CODE | Giữ giá. Hai mũi tên ngược chiều, dấu trừ nhấp nháy, −72/18 = −4; nhãn 'số lùi'. | 0 |
| 11 | 11.1 | 05:41 | 53s | ANIMATION-CODE | Trạng thái 1: giữ vành, tỉ số 5. Trạng thái 2: khóa hai bộ phận, tỉ số 1. Đổi nhãn đầu vào sang vành, giữ mặt trời, tỉ số 1,25. Đồng hồ tốc độ; chữ 'ví dụ minh họa'. | 0 |
| 12 | 12.1 | 06:34 | 30s | ANIMATION-CODE | Sơ đồ Simpson tổng quát: hai bộ hành tinh, mặt trời nối nhau; hai phanh dải, hai ly hợp sáng lên (không gắn bảng số cụ thể vì chưa xác minh). | 0 |
| 12 | 12.2 | 07:04 | 18s | ĐỒ HỌA | Thẻ bằng sáng chế Simpson: nộp 1944, cấp 1950 (US 2,518,824; dùng bản vẽ công khai nếu có); thẻ TorqueFlite 1956. | 0 |
| 13 | 13.1 | 07:22 | 20s | ANIMATION-CODE | Nhìn lại ba màu của bộ hành tinh, camera kéo ra thành hộp số hoàn chỉnh. | 0 |
| 13 | 13.2 | 07:42 | 4s | AI-VIDEO | Cảnh kết: xe chạy đường vắng lúc chạng vạng, nhìn từ phía sau, không thấy cơ cấu. | 1 clip (nháp 480p trước) |
| 13 | 13.3 | 07:46 | 18s | ĐỒ HỌA | Màn kết: tên kênh (chờ chốt), gợi ý tập sau. | 0 |

## Prompt cho AI (chỉ các shot AI)
- **1.1 (AI-VIDEO, 4s):** `Close-up of a hand moving an automatic gear selector to D inside a car at night, dashboard glow in orange and cyan, shallow depth of field, slow push-in, no text, no faces, 16:9, 4 seconds`
- **3.1 (AI-IMAGE, 8s):** `Illustration of an early 1900s open motor car on a dirt road, sepia and teal film tones, soft morning light, wide shot, no readable text, no logos, 16:9`
- **3.3 (AI-IMAGE, 8s):** `Illustration of a black early 1900s touring car on a country road, tall narrow body, spoked wheels, film grain, wide shot, no readable text, no logos, 16:9`
- **5.1 (AI-IMAGE, 8s):** `Illustration of a 1930s automotive engineering drafting room, engineers at drafting tables seen from behind, warm lamp light, blueprints, film grain, wide shot, no readable text, 16:9`
- **5.3 (AI-IMAGE, 15s):** `Illustration of a late-1930s American sedan on a city street at dusk, teal and amber tones, film grain, wide shot, no readable text, no logos, 16:9`
- **13.2 (AI-VIDEO, 4s):** `Cinematic rear tracking shot of a car driving on an empty road at dusk, orange and teal sky, slight motion blur, no text, no readable plates, 16:9, 4 seconds`

## Quy tắc đăng và nhãn
- Mọi ảnh/clip AI cảnh thực tế (xe, phòng thiết kế, đường) phải **bật nhãn "altered/synthetic content"** khi đăng (nguyên tắc 5); nên ghi "ảnh minh họa do AI tạo" trên hình.
- Không tạo ảnh/clip mô tả cơ khí; không khẳng định ảnh AI là hiện vật hay xe thật (Antikythera, Model T, Oldsmobile).
- Bản vẽ bằng sáng chế: ưu tiên bản công khai; kiểm tra bản quyền trước khi dùng.

## Việc cần bạn quyết
1. Chốt brand (tên kênh, giọng đọc, bảng màu); hiện style chỉ là tạm.
2. Đăng ký Higgsfield Starter để chạy bước "thử trước".
3. Chấp nhận hay không hai clip AI-VIDEO (hook và kết); nếu không, đổi sang ảnh Ken Burns.
4. Ngân sách credits tối đa cho video này, sau khi có số đo thật.
