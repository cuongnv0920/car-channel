# Research — Hộp số tự động / bộ bánh răng hành tinh (video #1)

> Ngày nghiên cứu: 2026-11-10. Trạng thái: **bản nháp chờ fact-check**.
> Lượt 2 (cùng ngày) đã bổ sung nguồn gốc: bằng sáng chế Simpson (S12), sách hướng dẫn Ford 1919 (S13), Grace's Guide về Lanchester (S14). Hydra-Matic và TorqueFlite vẫn chưa có tài liệu nhà sản xuất gốc. Phần "Câu hỏi còn mở" ghi rõ cái nào đã giải quyết.
> Quy ước: `[CẦN XÁC MINH]` = chỉ có một nguồn yếu hoặc các nguồn mâu thuẫn.

## Tóm tắt 5 dòng

1. Bộ bánh răng hành tinh (epicyclic / planetary gear) gồm bánh răng mặt trời, giá hành tinh (carrier) mang các bánh răng hành tinh, và vành răng ngoài (ring). Giữ cố định một bộ phận và dẫn động bộ phận khác sẽ cho một tỉ số truyền khác nhau (S1, S6).
2. Ý tưởng bánh răng "gắn trên bánh răng" rất cổ, không phải phát minh năm 1900. Cơ cấu Antikythera (~80 TCN) được cho là có dùng nó (S1, S10).
3. Trên xe hơi, bộ bánh răng hành tinh xuất hiện sớm hơn cả năm 1900: xe Lanchester đầu tiên (1896) đã có "epicyclic change-speed gears" (S14), rồi Wilson-Pilcher (1901–1904), Ford Model T (1908) (S3, S4, S9).
4. GM Hydra-Matic (xe model 1940) được xem là hộp số tự động hoàn toàn đầu tiên sản xuất hàng loạt: 4 cấp số, 3 bộ hành tinh, nối động cơ qua khớp nối thủy lực chứ không phải biến mô (S2, S3).
5. Hộp số tự động hiện đại dùng nhiều bộ hành tinh, chuyển số bằng ly hợp và phanh dải/phanh đĩa chặn từng bộ phận. Bộ Simpson (nộp đơn 1944, cấp bằng 1950) rất phổ biến vì gọn và dùng chung bánh răng (S7, S12).

## Cơ chế vận hành

### Thành phần của một bộ hành tinh đơn (S1, S6)
- **Sun gear** — bánh răng mặt trời, nằm giữa.
- **Planet gears** — các bánh răng hành tinh, ăn khớp với mặt trời và vành răng, gắn trên giá.
- **Carrier** — giá hành tinh, giữ các bánh răng hành tinh và quay quanh tâm.
- **Ring gear / annulus** — vành răng ngoài, răng bên trong.

Ba bộ phận đồng trục: mỗi bộ phận có thể là đầu vào, đầu ra hoặc bị giữ cố định.

### Công thức tỉ số truyền (Zs = số răng mặt trời, Zr = số răng vành)
Hai nguồn độc lập cho cùng công thức (S1 Wikipedia, S6 tec-science):

| Giữ cố định | Vào → Ra | Tỉ số | Ghi chú |
|---|---|---|---|
| Vành răng | Mặt trời → giá | **1 + Zr/Zs** | Giảm tốc mạnh, lớn hơn 2 (S6) |
| Mặt trời | Vành → giá | **1 + Zs/Zr** | Giữa 1 và 2 (S6) |
| Giá | Mặt trời → vành | **−Zr/Zs** | Dấu âm: **đảo chiều quay** — nguyên lý số lùi (S1, S6) |
| Không giữ gì, khóa hai bộ phận | — | **1 : 1** | Truyền thẳng (S6) |

Phương trình Willis: `nr·Zr = nc·(Zr + Zs) − Zs·ns` (S6).

**Ví dụ tính tay để làm prototype animation** (tự tính từ công thức trên, không lấy từ nguồn): Zs = 18, Zr = 72 → vành giữ cố định, mặt trời vào, giá ra: tỉ số = 1 + 72/18 = **5,0**. Ví dụ này khớp với ví dụ trong kết quả tìm kiếm tec-science.
- Quan hệ hình học Zr = Zs + 2·Zp (Zp = răng hành tinh) `[CẦN XÁC MINH]`: tôi chưa đọc được nguồn nêu rõ công thức này.

### Hộp số tự động dùng bộ hành tinh thế nào (S1, S3, S7)
- Ly hợp và phanh dải/phanh đĩa **giữ hoặc nối** mặt trời, giá hay vành. Mỗi tổ hợp cho một cấp số (S1).
- Nhiều bộ hành tinh được ghép nối tiếp trong một vỏ (S1).
- Giữa động cơ và hộp số là **khớp nối thủy lực** (Hydra-Matic, 1939) rồi **biến mô** (Dynaflow, 1948) thay ly hợp ma sát (S2, S3).
- **Bộ Simpson:** hai bộ hành tinh có **mặt trời nối với nhau** (một trục chung), cho 3 số tiến và 1 số lùi, chỉ cần 2 phanh dải và 2 ly hợp (S7, S12). Bằng sáng chế mô tả: đầu vào dẫn động vành răng của một bộ cho số tiến, hoặc mặt trời cho số lùi; phanh giữ mặt trời và một giá hành tinh; một ly hợp có thể khóa bộ thành truyền thẳng (S12). Ở số 1 giữ giá B; ở số 2 giữ mặt trời; số lùi dùng chung bánh răng với số 1 (S7).
- Tỉ số TorqueFlite 727 (3 cấp): **2,45 / 1,45 / 1,00**, số lùi khoảng **2,20–2,21** tùy nguồn (S16). Một nguồn ghi số 1 là 2,54 nhưng nhiều khả năng sai hoặc là biến thể khác. Chưa đọc được bảng tỉ số trong sách hướng dẫn (S12b); `[CẦN XÁC MINH]` con số lùi chính xác.

### Hydra-Matic nguyên bản (S2)
- 4 số tiến + số lùi, 3 bộ hành tinh, khớp nối thủy lực hai phần tử (không nhân mô-men).
- Tỉ số xe du lịch theo Wikipedia: **3,82 / 2,63 / 1,45 / 1,00**. Xe tải nhẹ: 4,08 / 2,63 / 1,55 / 1,00 (S2). Một nguồn khác ghi bản 1940 là **3,66 / 2,53 / 1,44 / 1,00** (S15). Hai bộ số liệu lệch nhau, có thể do khác đời hoặc khác nguồn: `[CẦN XÁC MINH]`, chưa dùng trong lời đọc.
- Số bộ hành tinh: **3** theo Wikipedia (S2), Mac's Motor City Garage (S15) và một bài khác (S9). Chỉ bình luận dưới bài của Severson nói 2 bộ, nên xem là ngoại lệ yếu. Vẫn nên đối chiếu một tài liệu GM gốc.
- Khớp nối thủy lực "thẳng" tỉ số hiệu dụng 1:1 nên không nhân mô-men; đó là lý do cần 4 cấp số (S15).

## Lịch sử

| Mốc | Sự kiện | Nguồn |
|---|---|---|
| ~500 TCN | Người Hy Lạp nêu khái niệm epicycle (chuyển động thiên văn, chưa phải bánh răng) | S1 |
| ~80 TCN | Cơ cấu Antikythera: bánh răng của Mặt Trăng dùng bánh răng gắn trên bánh răng; phần Mặt Trời và hành tinh không còn nguyên | S1, S10 |
| Thế kỷ 11 | Ibn Khalaf al-Muradi (Al-Andalus) dùng bánh răng hành tinh trong đồng hồ nước | S11 (chỉ qua tóm tắt tìm kiếm, `[CẦN XÁC MINH]`) |
| Thế kỷ 14 | Richard of Wallingford mô tả bánh răng hành tinh cho đồng hồ thiên văn | S1 |
| 1896–1897 | Xe Lanchester đầu tiên (1896) và xe phaeton hai chỗ (1897) có "epicyclic change-speed gears" | S14 |
| 1900 | Một nguồn nói Lanchester làm xe hộp số hành tinh điều khiển tay từ 1900; Grace's Guide cho thấy thật ra sớm hơn | S9, S14 |
| 1901–1904 | Xe Wilson-Pilcher (Anh): hộp số hai bộ hành tinh, bốn tỉ số; tiền thân hộp số Wilson | S3, S9 |
| 1904 | Hộp số Sturtevant, thường được coi là "hộp số tự động thực sự đầu tiên"; hay hỏng đột ngột | S3 (nguồn gốc bị gắn thẻ kiểm chứng thất bại) |
| 1908 | Ford Model T dùng hộp số hành tinh 2 số tiến + số lùi, điều khiển bằng 3 bàn đạp | S3, S4 |
| 1928 | Hộp số tiền chọn (pre-selector) Wilson: bằng sáng chế và công ty Self-Changing Gears | S9 |
| 1932 | Nhóm của Earl A. Thompson (Cadillac) bắt đầu làm hộp số "không cần sang số" | S2 |
| 1933–1935 | REO Self-Shifter: bán tự động, vẫn cần bàn đạp ly hợp | S3 |
| 1937–1939 | Oldsmobile Automatic Safety Transmission: bán tự động, 2 số, ước tính ~25.000 chiếc, phản ứng khách hàng kém | S3, S8 |
| 1939 | Hydra-Matic bắt đầu sản xuất (5/1939); xe Oldsmobile đầu tiên giao tháng 10/1939 | S2 |
| 1941 | Cadillac cung cấp Hydra-Matic | S2 |
| 1948 | Buick Dynaflow: biến mô đầu tiên | S3 |
| 1944 → 1950 | Howard W. Simpson (Dearborn, Michigan) nộp đơn 16/9/1944, được cấp US 2,518,824 ngày 15/8/1950, đứng tên cá nhân | S12 |
| 1956 | Chrysler TorqueFlite, hộp số đầu tiên dùng bộ Simpson | S3, S7 |

Con số quy mô: gần 200.000 chiếc Hydra-Matic bán trước khi ngừng sản xuất xe du lịch tháng 2/1942; 1 triệu chiếc đến năm 1949 (S2). Quân sự: xe tăng M5 Stuart (hai hộp số, mỗi hộp nối hai động cơ Cadillac V8) và M24 Chaffee (S2).

Model T: sản xuất từ 1/10/1908 đến 26/5/1927, hơn 15 triệu xe. Ba bàn đạp: trái chọn số thấp/trung gian/cao, giữa là số lùi, phải là phanh hộp số (S4). **Sách hướng dẫn Ford 1919 xác nhận (S13):** bàn đạp trái ép hết là số thấp, nửa chừng là trung gian, nhả ra là số cao; bàn đạp giữa là số lùi; bàn đạp phải là "transmission brake"; cần tay kéo hết về sau là phanh khẩn cấp tác động lên bánh sau bằng guốc phanh nở trong tang trống. Hộp số chọn số bằng cách dừng một phần của bộ bánh răng bằng dải (band), giống phanh dải. Sách mô tả hai số tiến (thấp và cao); gần như mọi lúc chạy ở số cao. Dây đai (band) có thể lệch chỉnh khiến xe bò (creep) (S4). Nhóm thiết kế: Childe Harold Wills, Joseph A. Galamb, Eugene Farkas, Henry Ford giám sát (S4). **Không có nguồn nào ghi ai thiết kế riêng hộp số hành tinh của Model T.**

## Ngộ nhận phổ biến và sự thật thú vị (ứng viên hook)

1. **"Phát minh thiên tài từ năm 1900" là chưa chính xác.** Ý tưởng cơ bản có từ thời Hy Lạp cổ đại. Điều đáng kể là *đưa nó vào ô tô và làm nó tự chuyển số*. Kịch bản không được viết "phát minh năm 1900".
2. **Hydra-Matic không dùng biến mô.** Nó dùng khớp nối thủy lực nên không nhân mô-men; biến mô đến sau (Dynaflow 1948) (S2, S3). Nhiều người nhầm.
3. **Model T "ba số" thực ra là hai số tiến.** Vì ba số gồm cả số lùi (S4, S13). Phanh chân (bàn đạp phải) là phanh hộp số, còn phanh bánh sau là cần tay (S13).
4. **Hộp số tự động đầu tiên "thật sự chạy được" là Hydra-Matic, không phải hộp số tự động đầu tiên.** Trước đó có Sturtevant 1904, REO 1933, Oldsmobile 1937, và hộp số thủy lực Brazil 1932 (S3).
5. **Thủ thuật toán học:** giữ vành răng cố định, tỉ số có thể lớn tùy ý (1 + Zr/Zs > 2), còn giữ mặt trời thì không bao giờ vượt quá 2 (S6). Đây là chi tiết đẹp để animate.
6. **Hộp số của xe du lịch từng ra chiến trường:** Hydra-Matic được dùng trên M5 Stuart và M24 Chaffee (S2).

## Từ khóa tiếng Việt gợi ý (chưa đo lượng tìm kiếm)

- hộp số tự động hoạt động như thế nào
- bộ bánh răng hành tinh là gì / cấu tạo bánh răng hành tinh
- bánh răng mặt trời, vành răng, giá hành tinh
- hộp số tự động AT cấu tạo nguyên lý
- khớp nối thủy lực, biến mô, hộp số 4 cấp
- Hydra-Matic, Ford Model T hộp số

## Bảng nguồn

| ID | Nguồn | Loại | Độ tin cậy |
|---|---|---|---|
| S1 | Wikipedia — Epicyclic gearing — https://en.wikipedia.org/wiki/Epicyclic_gearing | Bách khoa, trích Uicker/Pennock/Shigley 2003 v.v. | Trung bình; một số ý gắn "citation needed" |
| S2 | Wikipedia — Hydramatic — https://en.wikipedia.org/wiki/Hydramatic | Bách khoa; trích Severson 2010, Flory 2008, Car and Driver 1988 | Trung bình |
| S3 | Wikipedia — Automatic transmission — https://en.wikipedia.org/wiki/Automatic_transmission | Bách khoa | Trung bình; nhiều mốc không có tham chiếu |
| S4 | Wikipedia — Ford Model T — https://en.wikipedia.org/wiki/Ford_Model_T | Bách khoa; trích Kimes 1989, Fahnestock 1921 | Trung bình |
| S6 | tec-science — Planetary gear set — https://www.tec-science.com/?p=28857 | Bài kỹ thuật giáo dục | Khá cho công thức |
| S7 | Aaron Severson — Secrets of the Simpson Gearset — https://ateupwithmotor.com/terms-technology-definitions/simpson-gearset/ | Bài lịch sử kỹ thuật, tác giả chuyên ngành | Khá; tỉ số TorqueFlite lấy từ bình luận |
| S8 | Aaron Severson — Hydra-Matic History part 1 — https://ateupwithmotor.com/terms-technology-definitions/hydramatic-history-part-1/ | Như trên | Phần thân bài khá; chi tiết kỹ thuật chủ yếu từ bình luận (yếu) |
| S9 | Wikipedia — Preselector gearbox; Grace's Guide — Self-Changing Gears; Jaguar Heritage — Wilson pre-selector | Tóm tắt từ kết quả tìm kiếm, chưa đọc toàn văn | Yếu cho đến khi đọc nguồn |
| S12 | Google Patents — US 2,518,824 "Transmission" (H. W. Simpson, nộp 1944, cấp 1950) — https://patents.google.com/patent/US2518824A/en | **Bằng sáng chế gốc** (đã đọc 100.000/110.000 ký tự đầu) | Cao |
| S12b | Chrysler TorqueFlite 727/904 Service Manual 1966–1977 — https://poly318.com/wp-content/uploads/2023/07/1966_1977_TorqueFlite_727_904_Service_Manual.pdf | Tài liệu nhà sản xuất | Chưa đọc được (tệp quá lớn để tải) |
| S13 | 1919 Ford Model T Manual (Internet Archive, văn bản OCR) — https://archive.org/stream/1919_Ford_Model-T_Manual/1919_Ford_Model-T_Manual_djvu.txt | **Sách hướng dẫn nhà sản xuất** (đọc 100.000/133.825 ký tự đầu; OCR có chỗ lỗi) | Cao cho đời 1919; chưa phải đời 1908–09 |
| S14 | Grace's Guide — Lanchester Engine Co — https://www.gracesguide.co.uk/Lanchester_Engine_Co | Lịch sử công nghiệp Anh | Khá; không nêu bằng sáng chế |
| S15 | Mac's Motor City Garage — Inside the 1940 GM Hydra-Matic — https://macsmotorcitygarage.com/inside-th-1940-gm-hydra-matic-the-first-modern-automatic-transmission/ | Bài blog lịch sử, không trích tài liệu gốc | Trung bình |
| S16 | Tóm tắt tìm kiếm: DieselHub, DrivingLine, Wikipedia về TorqueFlite 727 | Thứ cấp | Trung bình; con số lùi lệch nhau |
| S10 | The Past — Antikythera mechanism — https://the-past.com/feature/the-antikythera-mechanism-an-ancient-greek-machine-rewriting-the-history-of-technology/ | Bài tạp chí khảo cổ | Trung bình; chỉ qua tóm tắt tìm kiếm |
| S11 | Decoding the Heavens (Jo Marchant) — blog; Wikipedia mirror về al-Muradi | Tóm tắt tìm kiếm | Yếu |

(S5 bỏ trống có chủ đích để không đánh lệch số thứ tự khi bổ sung nguồn.)

## Câu hỏi còn mở (cần làm trước khi viết kịch bản)

1. **Nguồn gốc cho các mốc còn lại.** Đã có: bằng sáng chế Simpson (S12), sách Ford 1919 (S13). Còn thiếu: tài liệu GM/Oldsmobile/Cadillac về Hydra-Matic, bằng sáng chế Thompson/GM, Wilson 1928, sách giáo trình hoặc bài SAE.
2. ~~Hydra-Matic có bao nhiêu bộ hành tinh~~ — **Đã xử lý:** 3 bộ theo ba nguồn (S2, S9, S15); bình luận nói 2 bộ là ngoại lệ yếu. Vẫn nên có tài liệu GM gốc.
3. ~~Lanchester có dùng hộp số hành tinh từ 1900 không~~ — **Đã xử lý:** Grace's Guide ghi xe Lanchester 1896 và 1897 đã có epicyclic gears (S14). Mốc "1900" của nguồn cũ là không chính xác. Chưa rõ loại hộp số cụ thể và có phải "đầu tiên trên ô tô" không (không được khẳng định).
4. ~~Model T có phanh bánh xe không~~ — **Đã xử lý:** có phanh khẩn cấp bánh sau bằng cần tay; phanh chân là phanh hộp số (S13). Wikipedia viết "không có phanh bánh" là nói gọn, không dùng cho lời đọc.
5. **Ai thiết kế hộp số hành tinh của Model T**, có bằng sáng chế liên quan không? Vẫn chưa có nguồn.
6. **Tỉ số Hydra-Matic nguyên bản:** 3,82 (S2) hay 3,66 (S15) cho số 1? Cần tài liệu GM.
7. **Bảng phần tử giữ/nối ở từng số của TorqueFlite** (số 3 của Simpson, số lùi chính xác 2,20 hay 2,21): cần đọc sách hướng dẫn Chrysler (S12b), tệp quá lớn để tải tự động, nên cần tải thủ công hoặc chia nhỏ.
8. **Góc nhìn riêng của video** (nguyên tắc 6): đối thủ chỉ giải thích lướt. Kênh nên làm sâu ở phần lịch sử và tỉ số truyền chính xác. Cần bạn chốt.
