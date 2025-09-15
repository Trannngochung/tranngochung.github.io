---
layout: default
title: Trang chủ
---

# Chào mừng đến với blog của mình! 👋

Xin chào! Đây là blog cá nhân của **Minh** được tạo bằng **GitHub Pages + Jekyll**.

## 🚀 Giới thiệu

Mình là một developer đam mê công nghệ và thích chia sẻ kiến thức. Trên blog này, bạn sẽ tìm thấy:

- 📝 **Bài viết về lập trình**: Web development, backend, DevOps
- 🛠️ **Tutorial và hướng dẫn**: Cách sử dụng các công cụ, framework
- 💡 **Tips & tricks**: Những mẹo nhỏ hữu ích trong lập trình
- 📚 **Chia sẻ kinh nghiệm**: Hành trình học tập và làm việc

## 📖 Bài viết mới nhất

<div class="recent-posts">
    {% for post in site.posts limit:3 %}
    <article class="recent-post">
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <div class="post-meta">
            <time>{{ post.date | date: "%d/%m/%Y" }}</time>
            {% if post.categories %}
                <span class="category">{{ post.categories.first }}</span>
            {% endif %}
        </div>
        <p>{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
    </article>
    {% endfor %}
</div>

## 🔗 Liên kết nhanh

- [📚 Tất cả bài viết](/blog/) - Xem tất cả bài viết trên blog
- [👤 Giới thiệu](/about/) - Tìm hiểu thêm về mình
- [📧 Liên hệ](/contact/) - Kết nối với mình

---

*Cảm ơn bạn đã ghé thăm! Hãy khám phá blog và để lại comment nhé! 😊*