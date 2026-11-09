# Kênh YouTube về xe do AI vận hành

Kênh nghiêm túc về ô tô: mỗi video giải thích chi tiết vận hành của MỘT bộ phận, kèm lịch sử ngắn.
Đọc `docs/00-ke-hoach-tong-the.md` để nắm kế hoạch tổng thể.

## Quyết định đã chốt
- Ngôn ngữ: **tiếng Việt** cho khán giả Việt (có thể thêm tiếng Anh sau — viết kịch bản theo cấu trúc dễ dịch).
- Giai đoạn đầu: **giọng đọc + hình minh họa**, không có nhân vật dẫn.
- Độ dài: **tối đa 15 phút**, tùy độ phức tạp của bộ phận (có thể 5–15 phút).
- Gói dịch vụ: Higgsfield **Starter**, ElevenLabs **Starter** → tiết kiệm credits, nâng cấp khi dự án tiến triển.
- Video #1: hộp số tự động / bánh răng hành tinh (`projects/001-hop-so-tu-dong`).

## Nguyên tắc bất di bất dịch
1. **Chính xác kỹ thuật trước tiên.** Mọi khẳng định kỹ thuật/lịch sử phải có nguồn và qua fact-checker.
2. **Hai cổng duyệt của người:** #1 sau fact-check kịch bản, #2 trước khi đăng. Không bao giờ tự đăng.
3. **Cơ chế cơ khí = animation lập trình** (Remotion/Three.js). AI video chỉ cho cảnh điện ảnh/lịch sử/cảm xúc.
4. **Tiết kiệm credits:** thử bằng ảnh/clip ngắn trước, chỉ sinh video dài khi storyboard đã duyệt.
5. Bật nhãn "altered/synthetic content" khi đăng cảnh thực tế do AI tạo.
6. Không làm hàng loạt nội dung lặp khuôn; mỗi video phải có góc nhìn riêng.

## Cấu trúc
- `.claude/skills/` — researcher, scriptwriter, fact-checker, storyboarder
- `projects/NNN-ten-video/` — `research/`, `script/`, `assets/` cho từng video
- `brand/` — nhận diện kênh (giọng, phong cách hình ảnh)
- `pipeline/` — mã pipeline tự động (về sau)
- `docs/` — kế hoạch và ghi chú

## Quy trình mỗi video
research → script → fact-check → [DUYỆT #1] → storyboard → assets → giọng/nhạc → ráp → QA → [DUYỆT #2] → upload
