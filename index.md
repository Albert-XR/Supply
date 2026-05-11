---
layout: home
title: Home
---

<style>
/* 基础样式 */
.hero {
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  color: white;
  padding: 60px 20px;
  text-align: center;
  margin: -20px -20px 30px -20px;
}
.hero h1 { font-size: 2.2em; margin-bottom: 15px; }
.hero-subtitle { font-size: 1.1em; opacity: 0.9; margin-bottom: 20px; }
.hero-badges { margin: 20px 0; }
.hero-badges span {
  background: rgba(255,255,255,0.15);
  padding: 6px 14px;
  border-radius: 20px;
  margin: 0 5px;
  font-size: 0.85em;
  display: inline-block;
  margin-bottom: 8px;
}
.cta-button {
  display: inline-block;
  background: #e94560;
  color: white;
  padding: 12px 28px;
  border-radius: 6px;
  text-decoration: none;
  margin: 8px;
  font-weight: bold;
}
.cta-button.secondary {
  background: transparent;
  border: 2px solid white;
}

.stats-bar {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(130px, 1fr));
  gap: 20px;
  padding: 40px 20px;
  background: #f8f9fa;
  text-align: center;
  margin-bottom: 30px;
}
.stat-item strong {
  display: block;
  font-size: 2em;
  color: #e94560;
}
.stat-item span { color: #666; font-size: 0.9em; }

section { padding: 30px 20px; max-width: 1100px; margin: 0 auto; }
h2 { text-align: center; margin-bottom: 25px; }

.category-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  margin: 25px 0;
}
.category-card {
  border: 1px solid #e0e0e0;
  border-radius: 10px;
  padding: 15px;
  text-align: center;
}
.category-card img {
  width: 100%;
  height: 150px;
  object-fit: cover;
  border-radius: 6px;
  margin-bottom: 12px;
  background: #f0f0f0;
}
.category-card h3 { margin: 10px 0 5px 0; }
.category-card p { font-size: 0.9em; color: #666; margin-bottom: 10px; }
.category-card a { color: #e94560; text-decoration: none; font-weight: bold; }

.features-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
  margin: 25px 0;
}
.feature {
  padding: 20px;
  background: #f8f9fa;
  border-radius: 8px;
}
.feature h4 { margin-top: 0; color: #1a1a2e; }

.cta-section {
  background: #1a1a2e;
  color: white;
  padding: 50px 20px;
  text-align: center;
  margin: 30px 0;
}
.cta-section h2 { margin-top: 0; }
.contact-mini { opacity: 0.8; margin-top: 15px; font-size: 0.9em; }

img { max-width: 100%; height: auto; }
</style>

<!-- 首屏横幅 -->
<div class="hero">
  <h1>JIEYANG DINGYONG HARDWARE & PLASTIC PRODUCTS CO., LTD</h1>
  <p class="hero-subtitle">Your Strategic Partner for OEM/ODM Cutlery Solutions</p>
  <div class="hero-badges">
    <span>✓ ISO9001 & BSCI Certified</span>
    <span>✓ FDA & LFGB Approved</span>
    <span>✓ 15+ Years Export Experience</span>
  </div>
  <a href="/products" class="cta-button">Browse Products</a>
  <a href="/contact" class="cta-button secondary">Request Quote</a>
</div>

<!-- 核心数据 -->
<div class="stats-bar">
  <div class="stat-item">
    <strong>600+</strong>
    <span>Product Designs</span>
  </div>
  <div class="stat-item">
    <strong>40+</strong>
    <span>Export Countries</span>
  </div>
  <div class="stat-item">
    <strong>5M+</strong>
    <span>Pieces Annual Output</span>
  </div>
  <div class="stat-item">
    <strong>200+</strong>
    <span>Factory Workers</span>
  </div>
</div>

<!-- 产品分类 -->
<section>
  <h2>Our Product Categories</h2>
  <div class="category-grid">
    <div class="category-card">
      <img src="/assets/images/products/cutlery-set.jpg" alt="Cutlery Sets">
      <h3>Cutlery Sets</h3>
      <p>16pc/24pc/72pc dinnerware sets, 18/10 stainless steel</p>
      <a href="/products">View Products →</a>
    </div>
    <div class="category-card">
      <img src="/assets/images/products/flatware_small.jpg" alt="Flatware">
      <h3>Flatware</h3>
      <p>Dinner forks, knives, spoons. Custom designs available</p>
      <a href="/products">View Products →</a>
    </div>
    <div class="category-card">
      <img src="/assets/images/products/cutlery-set_small.jpg" alt="Serving Utensils">
      <h3>Serving Utensils</h3>
      <p>Serving spoons, ladles, tongs for hotels & restaurants</p>
      <a href="/products">View Products →</a>
    </div>
    <div class="category-card">
      <img src="/assets/images/products/serving_small.jpg" alt="Hotel Supplies">
      <h3>Hotel & Restaurant</h3>
      <p>Bulk orders, custom logo engraving, premium packaging</p>
      <a href="/products">View Products →</a>
    </div>
  </div>
</section>

<!-- 为什么选择我们 -->
<section>
  <h2>Why Choose Us</h2>
  <div class="features-grid">
    <div class="feature">
      <h4>🏭 Factory Direct</h4>
      <p>5,000㎡ production facility, full support for bespoke molds, finishes (PVD/Mirror/Satin), and branding.</p>
    </div>
    <div class="feature">
      <h4>🔬 Quality Assured</h4>
      <p>Rigorous in-house QC protocols to meet international standards (EU/FDA/LFGB).</p>
    </div>
    <div class="feature">
      <h4>🚢 Agile Production</h4>
      <p>Flexible MOQs and optimized lead times for rapid market entry.</p>
    </div>
    <div class="feature">
      <h4>🎨 Global Footprint</h4>
      <p>Proven experience serving clients across Europe, the Americas, Middle East and Southeast Asia etc. 40+ countries.</p>
    </div>
  </div>
</section>

<!-- 询盘引导 -->
<div class="cta-section">
  <h2>Ready to Source Premium Tableware?</h2>
  <p>Tell us your target product, quantity, and destination country.</p>
  <a href="/contact" class="cta-button">Get Free Quote</a>
  <a href="https://wa.me/8617718828885" class="cta-button secondary" target="_blank">Chat on WhatsApp</a>
  <p class="contact-mini">📧 sales@ding-yong.com | 📱 +86 17718828885</p>
</div>
