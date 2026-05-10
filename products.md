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
.product-card {
  border: 1px solid #e8e8e8;
  border-radius: 12px;
  overflow: hidden;
  transition: box-shadow 0.3s, transform 0.3s;
  background: white;
}
.product-card:hover {
  box-shadow: 0 8px 25px rgba(0,0,0,0.1);
  transform: translateY(-5px);
}
.product-image {
  width: 100%;
  height: 220px;
  object-fit: cover;
  background: #f5f5f5;
}
.product-info { padding: 20px; }
.product-info h3 {
  font-size: 1.1em;
  margin-bottom: 8px;
  color: #1a1a2e;
}
.product-meta {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 12px;
}
.product-price {
  color: #e94560;
  font-size: 1.2em;
  font-weight: bold;
}
.product-moq {
  color: #888;
  font-size: 0.85em;
}
.product-desc {
  color: #666;
  font-size: 0.9em;
  line-height: 1.5;
  margin-bottom: 15px;
}
.product-tags {
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
  margin-bottom: 15px;
}
.tag {
  background: #f0f0f0;
  padding: 4px 12px;
  border-radius: 15px;
  font-size: 0.8em;
  color: #555;
}
.product-actions {
  display: flex;
  gap: 10px;
}
.btn {
  flex: 1;
  padding: 10px;
  text-align: center;
  border-radius: 6px;
  text-decoration: none;
  font-size: 0.9em;
  font-weight: bold;
  transition: opacity 0.2s;
}
.btn:hover { opacity: 0.85; }
.btn-primary {
  background: #e94560;
  color: white;
}
.btn-secondary {
  background: #f0f0f0;
  color: #333;
}

/* 询盘引导 */
.cta-bottom {
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  color: white;
  padding: 50px 30px;
  text-align: center;
  border-radius: 12px;
  margin: 50px 0;
}
.cta-bottom h2 { margin-bottom: 15px; }
.cta-bottom p { opacity: 0.9; margin-bottom: 25px; }
</style>

<div class="products-page">
  <h1>Our Stainless Steel Products</h1>
  <p class="products-intro">
    Browse our complete catalog of premium 18/10 stainless steel tableware. 
    All products support OEM/ODM with custom logo and packaging.
  </p>

  <!-- 分类筛选 -->
  <div class="category-filter">
    <button class="filter-btn active" onclick="filterProducts('all')">All Products</button>
    <button class="filter-btn" onclick="filterProducts('cutlery')">Cutlery Sets</button>
    <button class="filter-btn" onclick="filterProducts('flatware')">Flatware</button>
    <button class="filter-btn" onclick="filterProducts('serving')">Serving</button>
    <button class="filter-btn" onclick="filterProducts('hotel')">Hotel & Restaurant</button>
  </div>

  <!-- 产品网格 -->
  <div class="product-grid" id="productGrid">
    
    <!-- 产品1 -->
    <div class="product-card" data-category="cutlery">
      <img src="https://via.placeholder.com/400x300?text=24pc+Cutlery+Set" alt="24-Piece Cutlery Set" class="product-image">
      <div class="product-info">
        <h3>24-Piece Stainless Steel Cutlery Set</h3>
        <div class="product-meta">
          <span class="product-price">$12.50/set</span>
          <span class="product-moq">MOQ: 1000 sets</span>
        </div>
        <p class="product-desc">18/10 stainless steel, mirror polish finish. Includes 6 dinner knives, 6 forks, 6 spoons, 6 teaspoons.</p>
        <div class="product-tags">
          <span class="tag">18/10 SS</span>
          <span class="tag">Mirror Polish</span>
          <span class="tag">FDA</span>
        </div>
        <div class="product-actions">
          <a href="/contact?product=24pc-cutlery" class="btn btn-primary">Inquire Now</a>
          <a href="/products/24pc-cutlery-set/" class="btn btn-secondary">Details</a>
        </div>
      </div>
    </div>

    <!-- 产品2 -->
    <div class="product-card" data-category="flatware">
      <img src="https://via.placeholder.com/400x300?text=Dinner+Fork" alt="Dinner Fork" class="product-image">
      <div class="product-info">
        <h3>Premium Dinner Fork</h3>
        <div class="product-meta">
          <span class="product-price">$0.85/pc</span>
          <span class="product-moq">MOQ: 3000 pcs</span>
        </div>
        <p class="product-desc">Heavy-duty 18/10 stainless steel dinner fork. Length: 20.5cm. Weight: 65g. Satin or mirror finish.</p>
        <div class="product-tags">
          <span class="tag">18/10 SS</span>
          <span class="tag">65g</span>
          <span class="tag">LFGB</span>
        </div>
        <div class="product-actions">
          <a href="/contact?product=dinner-fork" class="btn btn-primary">Inquire Now</a>
          <a href="/products/dinner-fork.md/" class="btn btn-secondary">Details</a>
        </div>
      </div>
    </div>

    <!-- 产品3 -->
    <div class="product-card" data-category="serving">
      <img src="https://via.placeholder.com/400x300?text=Serving+Spoon" alt="Serving Spoon" class="product-image">
      <div class="product-info">
        <h3>Large Serving Spoon</h3>
        <div class="product-meta">
          <span class="product-price">$1.20/pc</span>
          <span class="product-moq">MOQ: 2000 pcs</span>
        </div>
        <p class="product-desc">Professional serving spoon for buffet and restaurant use. Length: 28cm. Dishwasher safe.</p>
        <div class="product-tags">
          <span class="tag">28cm</span>
          <span class="tag">Hotel Grade</span>
          <span class="tag">Dishwasher Safe</span>
        </div>
        <div class="product-actions">
          <a href="/contact?product=serving-spoon" class="btn btn-primary">Inquire Now</a>
          <a href="#" class="btn btn-secondary">Details</a>
        </div>
      </div>
    </div>

    <!-- 产品4 -->
    <div class="product-card" data-category="hotel">
      <img src="https://via.placeholder.com/400x300?text=Hotel+Bulk" alt="Hotel Bulk Set" class="product-image">
      <div class="product-info">
        <h3>Hotel Bulk Flatware Set (500pc)</h3>
        <div class="product-meta">
          <span class="product-price">$8.50/pc</span>
          <span class="product-moq">MOQ: 500 pcs</span>
        </div>
        <p class="product-desc">Complete hotel restaurant flatware. Heavy gauge 18/0 or 18/10. Custom logo engraving available.</p>
        <div class="product-tags">
          <span class="tag">18/0 or 18/10</span>
          <span class="tag">Logo Engraving</span>
          <span class="tag">Bulk Pack</span>
        </div>
        <div class="product-actions">
          <a href="/contact?product=hotel-bulk" class="btn btn-primary">Inquire Now</a>
          <a href="#" class="btn btn-secondary">Details</a>
        </div>
      </div>
    </div>

    <!-- 产品5 -->
    <div class="product-card" data-category="cutlery">
      <img src="https://via.placeholder.com/400x300?text=16pc+Gift+Set" alt="16pc Gift Set" class="product-image">
      <div class="product-info">
        <h3>16-Piece Gift Box Set</h3>
        <div class="product-meta">
          <span class="product-price">$9.80/set</span>
          <span class="product-moq">MOQ: 1500 sets</span>
        </div>
        <p class="product-desc">Elegant gift packaging for retail. 4-place setting with premium color box. Perfect for Amazon/eBay sellers.</p>
        <div class="product-tags">
          <span class="tag">Gift Box</span>
          <span class="tag">Retail Ready</span>
          <span class="tag">Amazon FBA</span>
        </div>
        <div class="product-actions">
          <a href="/contact?product=gift-set" class="btn btn-primary">Inquire Now</a>
          <a href="#" class="btn btn-secondary">Details</a>
        </div>
      </div>
    </div>

    <!-- 产品6 -->
    <div class="product-card" data-category="flatware">
      <img src="https://via.placeholder.com/400x300?text=Steak+Knife" alt="Steak Knife" class="product-image">
      <div class="product-info">
        <h3>Serrated Steak Knife</h3>
        <div class="product-meta">
          <span class="product-price">$1.50/pc</span>
          <span class="product-moq">MOQ: 2500 pcs</span>
        </div>
        <p class="product-desc">Sharp serrated edge steak knife. 23.5cm length. Hollow handle design. Restaurant quality.</p>
        <div class="product-tags">
          <span class="tag">Serrated</span>
          <span class="tag">23.5cm</span>
          <span class="tag">Restaurant</span>
        </div>
        <div class="product-actions">
          <a href="/contact?product=steak-knife" class="btn btn-primary">Inquire Now</a>
          <a href="#" class="btn btn-secondary">Details</a>
        </div>
      </div>
    </div>

  </div>

  <!-- 底部询盘 -->
  <div class="cta-bottom">
    <h2>Can't Find What You Need?</h2>
    <p>We support full OEM/ODM service. Send us your design, sample, or idea. We'll produce exactly what you want.</p>
    <a href="/contact" class="cta-button">Request Custom Quote</a>
    <a href="https://wa.me/8613822066349" class="cta-button secondary" target="_blank">Chat on WhatsApp</a>
  </div>
</div>

<script>
function filterProducts(category) {
  // 更新按钮状态
  document.querySelectorAll('.filter-btn').forEach(btn => {
    btn.classList.remove('active');
  });
  event.target.classList.add('active');

  // 筛选产品
  const cards = document.querySelectorAll('.product-card');
  cards.forEach(card => {
    if (category === 'all' || card.dataset.category === category) {
      card.style.display = 'block';
    } else {
      card.style.display = 'none';
    }
  });
}
</script>
