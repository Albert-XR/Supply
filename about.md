---
layout: page
title: About Us
permalink: /about/
---

<style>
.about-page h1 { text-align: center; margin-bottom: 10px; }
.about-subtitle { text-align: center; color: #666; margin-bottom: 40px; }

/* 公司介绍 */
.company-intro {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
  align-items: center;
  margin-bottom: 50px;
}
.company-intro img {
  width: 100%;
  border-radius: 12px;
  height: 300px;
  object-fit: cover;
}
.company-intro h2 { margin-bottom: 15px; color: #1a1a2e; }
.company-intro p { color: #555; line-height: 1.8; margin-bottom: 15px; }

/* 时间线 */
.timeline {
  position: relative;
  padding-left: 30px;
  margin: 30px 0;
}
.timeline::before {
  content: '';
  position: absolute;
  left: 8px;
  top: 0;
  bottom: 0;
  width: 2px;
  background: #e94560;
}
.timeline-item {
  position: relative;
  margin-bottom: 25px;
  padding-left: 20px;
}
.timeline-item::before {
  content: '';
  position: absolute;
  left: -26px;
  top: 5px;
  width: 12px;
  height: 12px;
  background: #e94560;
  border-radius: 50%;
}
.timeline-item strong {
  color: #e94560;
  display: block;
  margin-bottom: 5px;
}

/* 数据展示 */
.stats-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
  margin: 40px 0;
  text-align: center;
}
.stat-box {
  background: #f8f9fa;
  padding: 30px 20px;
  border-radius: 10px;
}
.stat-box strong {
  display: block;
  font-size: 2.2em;
  color: #e94560;
  margin-bottom: 5px;
}
.stat-box span { color: #666; font-size: 0.9em; }

/* 认证 */
.cert-section {
  text-align: center;
  margin: 50px 0;
}
.cert-grid {
  display: flex;
  justify-content: center;
  gap: 40px;
  flex-wrap: wrap;
  margin-top: 30px;
}
.cert-item {
  width: 120px;
  height: 120px;
  background: #f8f9fa;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 0.85em;
  color: #666;
  font-weight: bold;
}

/* 团队/设备 */
.equipment-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
  margin: 30px 0;
}
.equip-card {
  text-align: center;
  padding: 20px;
  background: #f8f9fa;
  border-radius: 10px;
}
.equip-card h4 { margin: 10px 0 5px; color: #1a1a2e; }
.equip-card p { font-size: 0.85em; color: #666; }

/* 响应式 */
@media (max-width: 768px) {
  .company-intro { grid-template-columns: 1fr; }
  .stats-grid { grid-template-columns: repeat(2, 1fr); }
}
</style>

<div class="about-page">
  <h1>About Ding-Yong Products</h1>
  <p class="about-subtitle">Professional Stainless Steel Tableware Manufacturer Since 2010</p>

  <!-- 公司介绍 -->
  <div class="company-intro">
    <div>
      <h2>Who We Are</h2>
      <p>Ding-Yong Products Co., Ltd is a leading manufacturer specializing in premium 18/10 stainless steel cutlery, flatware, and kitchen utensils. Based in Guangdong, China, we have been serving global B2B buyers for over 15 years.</p>
      <p>Our 5,000㎡ production facility houses 200+ skilled workers and advanced CNC polishing machines, enabling us to produce 500,000+ pieces monthly. We are committed to delivering restaurant-quality tableware at competitive factory-direct prices.</p>
      <p>From small custom orders to large hotel chain contracts, we provide flexible OEM/ODM solutions tailored to your market needs.</p>
    </div>
    <img src="https://via.placeholder.com/600x400?text=Factory+Building" alt="Factory Building">
  </div>

  <!-- 核心数据 -->
  <div class="stats-grid">
    <div class="stat-box">
      <strong>15+</strong>
      <span>Years Experience</span>
    </div>
    <div class="stat-box">
      <strong>5,000㎡</strong>
      <span>Factory Area</span>
    </div>
    <div class="stat-box">
      <strong>200+</strong>
      <span>Workers</span>
    </div>
    <div class="stat-box">
      <strong>500K+</strong>
      <span>Monthly Output</span>
    </div>
  </div>

  <!-- 发展历程 -->
  <section>
    <h2 style="text-align: center; margin-bottom: 30px;">Our Journey</h2>
    <div class="timeline">
      <div class="timeline-item">
        <strong>2010</strong>
        Founded as a small family workshop with 10 workers, focusing on local market stainless steel flatware.
      </div>
      <div class="timeline-item">
        <strong>2013</strong>
        Expanded to 50 workers, obtained ISO9001 certification, began exporting to Southeast Asia.
      </div>
      <div class="timeline-item">
        <strong>2016</strong>
        Moved to new 5,000㎡ facility, installed CNC polishing lines, reached 200 workers capacity.
      </div>
      <div class="timeline-item">
        <strong>2019</strong>
        Achieved FDA and LFGB certifications, entered European and North American markets.
      </div>
      <div class="timeline-item">
        <strong>2023</strong>
        Launched OEM/ODM design center, serving Amazon FBA sellers and hotel chains globally.
      </div>
      <div class="timeline-item">
        <strong>2026</strong>
        Annual export volume exceeded 5 million pieces, covering 50+ countries worldwide.
      </div>
    </div>
  </section>

  <!-- 生产设备 -->
  <section>
    <h2 style="text-align: center; margin-bottom: 30px;">Production Capability</h2>
    <div class="equipment-grid">
      <div class="equip-card">
        <h4>🔧 CNC Polishing</h4>
        <p>12 automated polishing lines for mirror/satin finish</p>
      </div>
      <div class="equip-card">
        <h4>⚡ Electroplating</h4>
        <p>Dust-free workshop for gold/rose gold/black PVD coating</p>
      </div>
      <div class="equip-card">
        <h4>🔦 Laser Engraving</h4>
        <p>Precision logo engraving, 0.1mm accuracy</p>
      </div>
      <div class="equip-card">
        <h4>📦 Auto Packaging</h4>
        <p>Color box, blister, gift box assembly lines</p>
      </div>
    </div>
  </section>

  <!-- 质量认证 -->
  <div class="cert-section">
    <h2>Quality Certifications</h2>
    <p style="color: #666; margin-bottom: 20px;">All products meet international food safety standards</p>
    <div class="cert-grid">
      <div class="cert-item">ISO<br>9001</div>
      <div class="cert-item">FDA<br>Approved</div>
      <div class="cert-item">LFGB<br>Certified</div>
      <div class="cert-item">SGS<br>Tested</div>
      <div class="cert-item">BSCI<br>Audit</div>
    </div>
  </div>

  <!-- CTA -->
  <div style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%); color: white; padding: 50px 30px; text-align: center; border-radius: 12px; margin: 50px 0;">
    <h2 style="margin-bottom: 15px;">Visit Our Factory</h2>
    <p style="opacity: 0.9; margin-bottom: 25px;">We welcome factory audits and video inspections. Schedule a visit or virtual tour today.</p>
    <a href="/contact" class="cta-button">Schedule Factory Visit</a>
    <a href="https://wa.me/8613822066349" class="cta-button secondary" target="_blank">Video Call on WhatsApp</a>
  </div>
</div>
