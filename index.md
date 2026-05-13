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
  margin: 0 -20px 30px -20px;    /* 突破 .container 的 padding */
  width: calc(100% + 40px);       /* 补偿负 margin */
  position: relative;
  left: -20px;                    /* 对齐 */
  box-sizing: border-box;
}
/* 大屏幕：一行显示 */
.hero h1 {
  font-size: clamp(1.0em, 2.2vw, 1.6em);  /* 自适应字体大小 */
  margin-bottom: 15px;
  white-space: nowrap;                      /* 强制不换行 */
  overflow: hidden;
  text-overflow: ellipsis;          /* 如果还是超出，显示省略号 */
}
/* 中等屏幕：缩小字体 */
@media (max-width: 1024px) {
  .hero h1 {
    font-size: 1.3em;
  }
}
/* 小屏幕：允许换行 */
@media (max-width: 768px) {
  .hero h1 {
    font-size: 1.1em;
    white-space: normal;    /* 允许换行 */
    word-break: keep-all;   /* 保持单词完整 */
    overflow: visible;
  }
}
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
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
  margin: 30px 0;
}

.category-card {
  border: 1px solid #e8e8e8;
  border-radius: 12px;
  overflow: hidden;
  transition: box-shadow 0.3s, transform 0.3s;
  background: white;
}

.category-card:hover {
  box-shadow: 0 8px 25px rgba(0,0,0,0.1);
  transform: translateY(-5px);
}

.category-card img {
  width: 100%;
  aspect-ratio: 16/9;
  object-fit: cover;
  display: block;
}

.category-info {
  padding: 15px;
}

.category-info h3 {
  font-size: 1em;
  margin-bottom: 6px;
  color: #1a1a2e;
}

.category-info p {
  color: #666;
  font-size: 0.85em;
  line-height: 1.4;
  margin-bottom: 10px;
}

.category-info a {
  color: #e94560;
  text-decoration: none;
  font-weight: bold;
  font-size: 0.9em;
}

/* 响应式：平板2列 */
@media (max-width: 1024px) {
  .category-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

/* 响应式：手机1列 */
@media (max-width: 600px) {
  .category-grid {
    grid-template-columns: 1fr;
  }
}

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
      <img src="/assets/images/home/portugal-400.jpg" alt="Portugal Series Cutlery">
      <div class="category-info">
        <h3>Cutlery Sets</h3>
        <p>24pc/72pc dinnerware sets, Portugal Series, multi-colour titanium plated</p>
        <a href="/products">View Products →</a>
      </div>
    </div>

    <div class="category-card">
      <img src="/assets/images/home/christmas-400.jpg" alt="Christmas Flatware">
      <div class="category-info">
        <h3>Flatware</h3>
        <p>Christmas dessert spoons, patterned handles, gift-giving preferred</p>
        <a href="/products">View Products →</a>
      </div>
    </div>

    <div class="category-card">
      <img src="/assets/images/home/kitchen-400.jpg" alt="Kitchen Anti-scalding Set">
      <div class="category-info">
        <h3>Serving Utensils</h3>
        <p>Kitchen anti-scalding set, patented product, beautiful and practical</p>
        <a href="/products">View Products →</a>
      </div>
    </div>

    <div class="category-card">
      <img src="/assets/images/home/goldbox-400.jpg" alt="Gold Box with Handle">
      <div class="category-info">
        <h3>Hotel & Restaurant</h3>
        <p>Gold gift box with handle, exquisite packaging, thickened material</p>
        <a href="/products">View Products →</a>
      </div>
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
