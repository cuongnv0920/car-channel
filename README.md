# car-channel

Kênh YouTube nghiêm túc về ô tô do AI vận hành. Mỗi video giải thích chi tiết vận hành của một bộ phận, kèm lịch sử ngắn. Ngôn ngữ chính: tiếng Việt.

## Cấu trúc

| Thư mục | Nội dung |
|---|---|
| `.claude/skills/` | Skill của các agent: researcher, scriptwriter, fact-checker, storyboarder |
| `projects/NNN-ten-video/` | `research/`, `script/`, `assets/` cho từng video |
| `brand/` | Nhận diện kênh (giọng, phong cách hình ảnh) |
| `pipeline/` | Mã pipeline tự động (về sau) |
| `docs/` | Kế hoạch và ghi chú |

## Quy trình mỗi video

research → script → fact-check → **[duyệt #1]** → storyboard → assets → giọng/nhạc → ráp → QA → **[duyệt #2]** → upload

Hai cổng duyệt của người không tự động hóa. Không bao giờ tự đăng.

## Tài liệu

- Kế hoạch tổng thể: [`docs/00-ke-hoach-tong-the.md`](docs/00-ke-hoach-tong-the.md)
- Nhánh Facebook (phụ, tách riêng): [`docs/01-nhanh-facebook-khao-sat-doi-thu.md`](docs/01-nhanh-facebook-khao-sat-doi-thu.md)
- Quy tắc cho agent: [`CLAUDE.md`](CLAUDE.md)

## Trạng thái

Video #1 (hộp số tự động / bánh răng hành tinh): research, kịch bản, fact-check và storyboard đã xong; đã qua duyệt #1. Chưa dựng animation và chưa sinh asset AI.

## Bí mật

Khóa API (Higgsfield, ElevenLabs, YouTube) đặt trong `.env`, không commit. Xem `.gitignore`.
