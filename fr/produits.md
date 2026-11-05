---
layout: page
lang: fr
permalink: /fr/produits/
title: Produits
description: "Découvrez les couverts en acier inoxydable DINGYONG : ménagères en coffret, couverts de table, séries dorées et multifinish — pour la vente en gros, les hôtels et le retail, tous disponibles en OEM/ODM avec logo et emballage personnalisés."
---

<style>
.products-page h1 { text-align: center; margin-bottom: 10px; }
.products-intro { text-align: center; color: #666; margin-bottom: 40px; }

/* 分类筛选 */
.category-filter {
  display: flex;
  justify-content: center;
  gap: 15px;
  margin-bottom: 30px;
  flex-wrap: wrap;
}
.filter-btn {
  padding: 8px 20px;
  border: 2px solid #e0e0e0;
  background: white;
  border-radius: 25px;
  cursor: pointer;
  font-size: 0.9em;
  transition: all 0.3s;
}
.filter-btn:hover, .filter-btn.active {
  border-color: #e94560;
  color: #e94560;
  font-weight: bold;
}

/* 产品网格 */
.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 25px;
  margin: 30px 0;
}

/* B2B 产品卡片增强样式 —— 整卡可点（点击空白/标签由事件委托转到详情页） */
.product-card {
  display: flex;
  flex-direction: column;
  height: 100%;
  cursor: pointer;
}

.product-info {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.product-image-wrapper {
  position: relative;
  width: 100%;
  aspect-ratio: 1/1;
  overflow: hidden;
}

.product-image-wrapper .product-image {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.3s;
}

.product-card:hover .product-image-wrapper .product-image {
  transform: scale(1.05);
}

.badge {
  position: absolute;
  top: 10px;
  left: 10px;
  padding: 4px 10px;
  border-radius: 4px;
  font-size: 0.7rem;
  font-weight: 700;
  text-transform: uppercase;
  color: #fff;
  z-index: 2;
}

.badge-new { background: #10b981; }
.badge-hot { background: #f59e0b; }

.product-series {
  margin: 0 0 10px;
  font-size: 0.85rem;
  color: #888;
}

.product-specs {
  display: flex;
  gap: 8px;
  margin-bottom: 12px;
  flex-wrap: wrap;
}

.spec {
  font-size: 0.75rem;
  color: #555;
  background: #f5f5f5;
  padding: 4px 10px;
  border-radius: 20px;
}

.product-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  margin-bottom: 16px;
}

.tag {
  font-size: 0.7rem;
  color: #777;
  border: 1px solid #e0e0e0;
  padding: 3px 8px;
  border-radius: 4px;
}

.product-actions {
  display: flex;
  gap: 8px;
  margin-top: auto;
}

.btn-view,
.btn-quote {
  flex: 1;
  text-align: center;
  padding: 10px;
  border-radius: 8px;
  text-decoration: none;
  font-size: 0.85rem;
  font-weight: 600;
  transition: all 0.2s;
}

.btn-view {
  background: #f5f5f5;
  color: #333;
}

.btn-view:hover {
  background: #e8e8e8;
}

.btn-quote {
  background: #e94560;
  color: #fff;
}

.btn-quote:hover {
  background: #d63a52;
}

/* 法语版全目录入口提示 */
.full-catalog-note {
  max-width: 820px;
  margin: 0 auto 10px;
  padding: 16px 20px;
  background: #f8f9fa;
  border-radius: 10px;
  color: #555;
  font-size: 0.92em;
  line-height: 1.6;
}
.full-catalog-note a { color: #e94560; font-weight: 600; text-decoration: none; }
.full-catalog-note a:hover { text-decoration: underline; }
</style>

<div class="products-page">
  <h1>Nos produits en acier inoxydable</h1>
  <p class="products-intro">Nos gammes phares présentées en français. Tous nos produits sont disponibles en OEM/ODM avec logo et emballage personnalisés.</p>

  <div class="full-catalog-note">
    Vous consultez notre sélection en français. Le <a href="/products/">catalogue complet ({{ site.products.size }} références)</a> est disponible en anglais — n'hésitez pas à nous <a href="/fr/contact/">contacter</a> pour toute référence qui ne figure pas ici.
  </div>

  <!-- 分类筛选 -->
  <div class="category-filter">
    <button class="filter-btn active" data-filter="all">Tous</button>
    <button class="filter-btn" data-filter="cutlery-sets">Ménagères et coffrets</button>
    <button class="filter-btn" data-filter="flatware">Couverts</button>
    <button class="filter-btn" data-filter="kitchen-tools">Accessoires de cuisine</button>
    <button class="filter-btn" data-filter="festival-gift-sets">Coffrets de fêtes</button>
  </div>

  <!-- 产品网格：法语集合 -->
  <div class="product-grid">
    {% for product in site.products_fr %}
      {% unless product.published == false %}
        {% include product-card.html product=product %}
      {% endunless %}
    {% endfor %}
  </div>

  <!-- 采购指南（内链博客，英文）-->
  <section style="margin-top:50px;border-top:1px solid #eee;padding-top:30px;">
    <h2 style="text-align:center;">Guides d'achat</h2>
    <p class="products-intro">Quelle spécification convient à votre marché ? Nos guides détaillés sont en anglais :</p>
    <ul style="max-width:820px;margin:0 auto;line-height:2;">
      {% for post in site.posts %}
      <li><a href="{{ post.url }}" style="color:#e94560;font-weight:600;">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </section>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  var buttons = document.querySelectorAll('.filter-btn');
  var cards = document.querySelectorAll('.product-card');

  buttons.forEach(function(btn) {
    btn.addEventListener('click', function() {
      // 切换按钮激活状态
      buttons.forEach(function(b) { b.classList.remove('active'); });
      btn.classList.add('active');

      var filter = btn.getAttribute('data-filter');
      cards.forEach(function(card) {
        var cat = card.getAttribute('data-category');
        if (filter === 'all' || cat === filter) {
          card.style.display = '';
        } else {
          card.style.display = 'none';
        }
      });
    });
  });
});
</script>
