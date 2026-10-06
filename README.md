# Kĩ năng viết kịch bản

Skill viết và chỉnh kịch bản review sản phẩm bằng tiếng Việt, theo giọng thực tế **“em – các anh”**. Nguyên tắc chính: **facts trước, marketing sau; hình ảnh chứng minh đi cùng lời nói**.

## Skill hỗ trợ gì?

- Kịch bản YouTube, video ngắn, lời thoại và shotlist từ brief, tài liệu, URL hoặc bản nháp.
- Chuyển thông số và công nghệ thành lợi ích sử dụng cụ thể.
- Kiểm chứng claim kỹ thuật, so sánh và khả năng tương thích/lắp đặt.
- Giữ hook, cách xưng hô và lựa chọn biên tập đã được người dùng chốt.
- Bổ sung hook, tiêu đề, chữ ảnh bìa, mô tả video và CTA khi được yêu cầu.

Skill dùng được cho nhiều nhóm sản phẩm; một số tài liệu có ví dụ riêng về đèn xe và bài học biên tập Titan Black/Fadil.

## Cài đặt

Tải hoặc clone repository, rồi đặt toàn bộ thư mục vào thư mục skills cá nhân với tên `product-review-script`:

```text
~/.codex/skills/product-review-script/
```

Trên Windows, đường dẫn thường là `%USERPROFILE%\.codex\skills\product-review-script`.

Giữ nguyên các thư mục `agents/` và `references/` bên cạnh `SKILL.md`.

## Cách dùng

Gọi skill và cung cấp thông tin sản phẩm cùng yêu cầu đầu ra, ví dụ:

```text
Dùng $product-review-script viết kịch bản review YouTube 3–5 phút
từ tài liệu và URL sản phẩm dưới đây. Xưng em – các anh.
Ghép lời thoại với cảnh quay, đánh dấu các claim cần xác minh.
```

```text
Dùng $product-review-script chỉnh bản nháp thành lời thoại TikTok
60–90 giây. Giữ nguyên hook đã chốt, bổ sung nỗi đau và CTA.
Không tự tạo kết quả test khi chưa có footage.
```

## Cấu trúc

```text
product-review-script/
├── SKILL.md
├── README.md
├── agents/
│   └── openai.yaml
└── references/
    ├── evidence-and-claims.md
    ├── marketing-engine.md
    ├── output-templates.md
    ├── review-framework.md
    ├── titan-black-fadil-lessons.md
    └── voice-style.md
```

`SKILL.md` chứa quy trình chính. Các tài liệu tham chiếu bổ sung giọng viết, khung review, kiểm chứng nguồn, góc marketing và mẫu đầu ra. `agents/openai.yaml` chứa cấu hình giao diện của skill.

## Nguyên tắc nội dung

Không bịa thông số hoặc kết quả thử nghiệm. Phân biệt fact đã xác nhận, quan sát trong điều kiện test, giải thích cơ chế và claim cần xác minh. Các bài học theo sản phẩm không thay thế nguồn thông số hiện hành.
