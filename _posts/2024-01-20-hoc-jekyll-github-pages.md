---
layout: post
title: "Học Jekyll và GitHub Pages - Tạo blog miễn phí"
date: 2024-01-20 14:30:00 +0700
author: "Hùng"
categories: ["Tutorial"]
tags: ["jekyll", "github-pages", "blog", "tutorial"]
---

# Học Jekyll và GitHub Pages - Tạo blog miễn phí

Hôm nay mình sẽ chia sẻ cách tạo một blog miễn phí bằng Jekyll và GitHub Pages.

## Jekyll là gì?

Jekyll là một **static site generator** được viết bằng Ruby. Nó cho phép bạn tạo website tĩnh từ các file Markdown, HTML, CSS và JavaScript.

### Ưu điểm của Jekyll:
- ✅ **Nhanh**: Website tĩnh load cực nhanh
- ✅ **Miễn phí**: Host miễn phí trên GitHub Pages
- ✅ **SEO tốt**: Dễ tối ưu cho search engine
- ✅ **Bảo mật**: Không có database, ít lỗ hổng
- ✅ **Version control**: Sử dụng Git để quản lý

## GitHub Pages là gì?

GitHub Pages là dịch vụ hosting miễn phí của GitHub, cho phép bạn host website tĩnh trực tiếp từ repository.

## Cách tạo blog Jekyll

### Bước 1: Tạo repository
```bash
# Tạo repository mới trên GitHub
# Tên repository: username.github.io
```

### Bước 2: Cấu trúc thư mục dự án
```
blog/
├── _config.yml
├── _layouts/
│   ├── default.html
│   └── post.html
├── _posts/
│   └── 2024-01-15-bai-viet-dau-tien.md
├── assets/
│   └── style.css
└── index.md
```

### Bước 3: Viết bài viết
Tạo file trong thư mục `_posts/` với format:
```
YYYY-MM-DD-ten-bai-viet.md
```

## Kết luận

Jekyll + GitHub Pages là combo tuyệt vời để tạo blog miễn phí. Đặc biệt phù hợp cho developer muốn viết blog kỹ thuật.

Bạn có muốn thử tạo blog cho riêng mình không? Hãy để lại comment nhé!
