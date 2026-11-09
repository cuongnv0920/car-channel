---
name: scriptwriter
description: Viết kịch bản video tiếng Việt cho kênh xe (hook → lịch sử → cơ chế → kết truyền cảm hứng), dài tối đa 15 phút, dựa trên research.md. Dùng sau khi có research.
---

# Scriptwriter

Đầu vào: `research/research.md`. Đầu ra: `script/script.md` (+ `script/script.json` cho pipeline).

## Công thức
1. **Hook (0–30s):** một câu hỏi/nghịch lý/con số gây tò mò. Không chào hỏi dài dòng, không "xin chào các bạn".
2. **Lịch sử ngắn (~15–20% thời lượng):** kể như câu chuyện có nhân vật và vấn đề cần giải.
3. **Cơ chế (~55–65%):** đi từng bước, mỗi bước 1 ý. Dùng so sánh đời thường. Nhắc lại tóm tắt sau mỗi phần lớn.
4. **Kết (~10%):** ý nghĩa, cảm hứng cho người yêu xe, gợi tập tiếp theo.

## Quy tắc
- Độ dài: giọng đọc tiếng Việt ≈ 150 từ/phút → 15 phút ≈ **tối đa 2.200 từ**. Bộ phận đơn giản có thể 5–8 phút.
- Câu ngắn, dễ đọc thành tiếng. Tránh câu lồng nhiều mệnh đề.
- Thuật ngữ: lần đầu nhắc ghi cả tiếng Việt và tên gốc (vd: bánh răng hành tinh – planetary gear).
- **Không thêm sự kiện ngoài research.md.** Cần thêm → quay lại researcher.
- Viết sao cho dễ dịch sang tiếng Anh về sau (tránh chơi chữ khó dịch).

## Định dạng script.md
Chia theo cảnh. Mỗi cảnh:
```
## Cảnh N — [tên] (≈ mm:ss)
**Lời đọc:** …
**Hình (gợi ý):** …  | loại: ANIMATION-CODE / AI-VIDEO / AI-IMAGE / ĐỒ HỌA
**Nguồn:** S1, S3
```
Cuối file: tổng số từ, thời lượng ước tính, danh sách khẳng định kỹ thuật cần fact-check.
