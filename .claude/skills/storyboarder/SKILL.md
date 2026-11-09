---
name: storyboarder
description: Chuyển kịch bản đã duyệt thành storyboard theo cảnh, quyết định cảnh nào dùng animation lập trình, ảnh AI hay video AI, và ước tính credits Higgsfield. Dùng sau Cổng duyệt #1.
---

# Storyboarder

Đầu vào: kịch bản đã qua Cổng duyệt #1. Đầu ra: `assets/storyboard.md` (+ `storyboard.json`).

## Quy tắc chọn loại hình
- **ANIMATION-CODE** (Remotion/Three.js): mọi thứ giải thích cơ chế, chuyển động bánh răng, dòng dầu, sơ đồ — phải chính xác. Ưu tiên tuyệt đối cho phần cơ chế.
- **AI-IMAGE** (Higgsfield `generate_image`): bối cảnh lịch sử, chân dung thời đại, minh họa tĩnh có chuyển động nhẹ (Ken Burns). Rẻ nhất → dùng nhiều nhất.
- **AI-VIDEO** (Higgsfield `generate_video`): chỉ cho vài khoảnh khắc điện ảnh (hook, cảnh xe chạy, kết). Clip 3–5 giây. Giới hạn số lượng vì gói Starter.
- **ĐỒ HỌA**: tiêu đề chương, số liệu, timeline.

## Mỗi cảnh ghi
`cảnh | thời lượng | loại hình | prompt/mô tả chi tiết | tham chiếu phong cách (brand/style.md) | credits ước tính`

## Ràng buộc ngân sách (Starter)
- Đặt trần credits cho video; cảnh vượt trần → đổi sang AI-IMAGE hoặc ANIMATION-CODE.
- Liệt kê "thử trước": sinh 1 ảnh/clip thử cho mỗi phong cách trước khi sinh hàng loạt.
- Không mô tả chi tiết cơ khí trong prompt AI-VIDEO (AI vẽ sai bánh răng, trục).
