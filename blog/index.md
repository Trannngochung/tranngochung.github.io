---
layout: default
title: "Tất cả bài viết"
---

# 📚 Tất cả bài viết

<div class="blog-intro">
    <p>Chào mừng bạn đến với blog của mình! Đây là nơi mình chia sẻ kiến thức về lập trình, công nghệ và những trải nghiệm học tập.</p>
</div>

<div class="posts-list">
    {% for post in site.posts %}
    <article class="post-preview">
        <header>
            <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
            <div class="post-meta">
                <time datetime="{{ post.date | date_to_xmlschema }}">
                    📅 {{ post.date | date: "%d/%m/%Y" }}
                </time>
                {% if post.author %}
                    <span class="author">👤 {{ post.author }}</span>
                {% endif %}
            </div>
        </header>
        
        <div class="post-excerpt">
            {% if post.excerpt %}
                {{ post.excerpt | strip_html | truncatewords: 30 }}
            {% else %}
                {{ post.content | strip_html | truncatewords: 30 }}
            {% endif %}
        </div>
        
        <footer class="post-preview-footer">
            {% if post.categories %}
            <div class="categories">
                📁 {% for category in post.categories %}
                    <span class="category">{{ category }}</span>
                {% endfor %}
            </div>
            {% endif %}
            
            {% if post.tags %}
            <div class="tags">
                🏷️ {% for tag in post.tags %}
                    <span class="tag">{{ tag }}</span>
                {% endfor %}
            </div>
            {% endif %}
            
            <a href="{{ post.url | relative_url }}" class="read-more">Đọc tiếp →</a>
        </footer>
    </article>
    {% endfor %}
</div>

{% if site.posts.size == 0 %}
<div class="no-posts">
    <p>Chưa có bài viết nào. Hãy quay lại sau nhé! 😊</p>
</div>
{% endif %}
