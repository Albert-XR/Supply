---
layout: page
title: Products
permalink: /products/
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

/* B2B 产品卡片增强样式 */
.product-card {
  display: flex;
  flex-direction: column;
  height: 100%;
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
</style>

<div class="products-page">
  <h1>Our Stainless Steel Products</h1>
  <p class="products-intro">Browse our complete catalog of premium 18/10 stainless steel tableware. All products support OEM/ODM with custom logo and packaging.</p>
  
  <!-- 分类筛选 -->
  <div class="category-filter">
    <button class="filter-btn active" data-filter="all">All</button>
    <button class="filter-btn" data-filter="cutlery-sets">Cutlery Sets</button>
    <button class="filter-btn" data-filter="flatware">Loose Flatware</button>
    <button class="filter-btn" data-filter="kitchen-tools">Kitchen Tools</button>
  </div>

  <!-- 产品网格：从硬编码改为 Jekyll 循环 -->
  <div class="product-grid">
    {% for product in site.products %}
      {% unless product.published == false %}
        {% include product-card.html product=product %}
      {% endunless %}
    {% endfor %}
  </div>
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
