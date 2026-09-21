---
layout: page
title: About Us
permalink: /about/
---

<!-- LocalBusiness Schema (About 页) -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "@id": "https://www.ding-yong.com/about/#localbusiness",
  "name": "Ding-Yong Products Co., Ltd",
  "alternateName": "DINGYONG",
  "url": "https://www.ding-yong.com/about/",
  "logo": "https://www.ding-yong.com/siteicon.png",
  "image": "https://www.ding-yong.com/siteicon.png",
  "description": "Stainless steel cutlery and flatware manufacturer in Guangdong, China. OEM/ODM services for hotels, restaurants, and retail brands.",
  "telephone": "+86-150-1337-1880",
  "email": "sales@ding-yong.com",
  "foundingDate": "2014",
  "priceRange": "$$",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "No. 2, 1st Floor, Maifeng Commercial Building, Chating Road, Xixi Village, Xichang Town, Jiedong District",
    "addressLocality": "Jieyang City",
    "addressRegion": "Guangdong Province",
    "addressCountry": "CN"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": 23.55,
    "longitude": 116.37
  },
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"],
      "opens": "08:30",
      "closes": "18:00"
    }
  ],
  "parentOrganization": {
    "@type": "Organization",
    "name": "Ding-Yong Products Co., Ltd",
    "url": "https://www.ding-yong.com/"
  }
}
</script>

<!-- VideoObject Schema (工厂视频) -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "VideoObject",
  "name": "Ding-Yong Factory Tour",
  "description": "Watch how your stainless steel tableware is crafted from raw steel to finished products at our 4,000 m² facility in Guangdong, China.",
  "thumbnailUrl": "https://i.ytimg.com/vi/rxGmVh_LP3A/maxresdefault.jpg",
  "uploadDate": "2024-01-01",
  "duration": "PT2M30S",
  "contentUrl": "https://www.youtube.com/watch?v=rxGmVh_LP3A",
  "embedUrl": "https://www.youtube.com/embed/rxGmVh_LP3A",
  "publisher": {
    "@type": "Organization",
    "name": "Ding-Yong Products Co., Ltd",
    "logo": {
      "@type": "ImageObject",
      "url": "https://www.ding-yong.com/siteicon.png"
    }
  }
}
</script>

<style>
/* Hero 横幅 */
.about-hero img {
  width: 100%;
  display: block;
  border-radius: 0 0 16px 16px;
}

/* 数字统计条 */
.stats-band {
  background: #1a1a2e;
  border-radius: 14px;
  display: flex;
  gap: 10px;
  padding: 26px 20px;
  margin: 40px auto;
  max-width: 1200px;
}

.stat-cell {
  flex: 1;
  text-align: center;
}

.stat-cell .num {
  font-size: 2em;
  font-weight: bold;
  color: #fff;
  line-height: 1.2;
  white-space: nowrap;
}

.stat-cell .num em {
  font-style: normal;
  color: #e94560;
}

.stat-cell .lbl {
  color: #aab0c0;
  font-size: 0.85em;
  margin-top: 6px;
}

/* 通用小节 */
.about-section {
  max-width: 1200px;
  margin: 70px auto;
  padding: 0 0;
}

.about-section > h2 {
  text-align: center;
  font-size: 1.8em;
  color: #1a1a2e;
  margin-bottom: 12px;
}

.section-subtitle {
  text-align: center;
  color: #666;
  margin-bottom: 35px;
}

/* 我们是谁：左文右图 */
.who-grid {
  display: grid;
  grid-template-columns: 1.1fr 1fr;
  gap: 45px;
  align-items: center;
}

.who-grid p {
  color: #555;
  line-height: 1.8;
  margin-bottom: 15px;
}

.who-grid .strengths {
  margin-top: 20px;
  line-height: 2;
}

.who-img img {
  width: 100%;
  border-radius: 12px;
  display: block;
  box-shadow: 0 8px 30px rgba(0,0,0,0.12);
}

/* 工厂视频 + 生产流程 */
.factory-grid {
  display: grid;
  grid-template-columns: 1.2fr 1fr;
  gap: 40px;
  align-items: center;
}

.video-box {
  position: relative;
  width: 100%;
  aspect-ratio: 16/9;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 8px 30px rgba(0,0,0,0.12);
}

.video-box iframe {
  position: absolute;
  top: 0; left: 0;
  width: 100%; height: 100%;
  border: none;
}

.process-list {
  display: flex;
  flex-direction: column;
  gap: 14px;
}

.process-item {
  display: flex;
  gap: 14px;
  align-items: flex-start;
  background: #f8f9fa;
  border-radius: 10px;
  padding: 14px 16px;
}

.process-item .step-no {
  min-width: 34px;
  height: 34px;
  background: #e94560;
  color: #fff;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  font-size: 0.95em;
}

.process-item h4 {
  margin: 0 0 3px;
  font-size: 1em;
  color: #1a1a2e;
}

.process-item p {
  margin: 0;
  color: #666;
  font-size: 0.9em;
  line-height: 1.5;
}

/* 证书墙 */
.cert-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
}

.cert-card {
  background: #f8f9fa;
  border-radius: 12px;
  padding: 28px 18px;
  text-align: center;
  transition: transform 0.3s;
}

.cert-card:hover {
  transform: translateY(-4px);
}

.cert-card .cert-icon {
  width: 58px;
  height: 58px;
  margin: 0 auto 14px;
  background: #fcebeb;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.cert-card .cert-icon svg {
  width: 28px;
  height: 28px;
  fill: #e94560;
}

.cert-card h4 {
  margin: 0 0 6px;
  color: #1a1a2e;
  font-size: 1.05em;
}

.cert-card p {
  margin: 0;
  color: #666;
  font-size: 0.85em;
  line-height: 1.5;
}

/* 时间线 */
.timeline-section {
  margin: 70px 0;
}

.timeline-section h2 {
  text-align: center;
  font-size: 1.8em;
  color: #1a1a2e;
  margin-bottom: 40px;
}

.timeline {
  position: relative;
  padding-left: 30px;
  max-width: 860px;
  margin: 0 auto;
}

.timeline::before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  width: 2px;
  background: #e94560;
}

.timeline-item {
  position: relative;
  padding-bottom: 30px;
}

.timeline-item::before {
  content: '';
  position: absolute;
  left: -34px;
  top: 5px;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #e94560;
  border: 2px solid white;
  box-shadow: 0 0 0 2px #e94560;
}

.timeline-year {
  font-weight: bold;
  color: #e94560;
  font-size: 1.1em;
  margin-bottom: 5px;
}

.timeline-text {
  color: #555;
  line-height: 1.6;
}

/* 展会图库 */
.tradeshow-section {
  margin: 70px 0;
}

.tradeshow-section h2 {
  text-align: center;
  font-size: 1.8em;
  color: #1a1a2e;
  margin-bottom: 15px;
}

.tradeshow-section .section-subtitle {
  margin-bottom: 0;
}

.tradeshow-row-title {
  text-align: center;
  color: #555;
  font-size: 1.05em;
  font-weight: 600;
  margin: 25px 0 12px;
}

.tradeshow-row-title:first-of-type {
  margin-top: 0;
}

.tradeshow-row {
  display: flex;
  gap: 12px;
  margin-bottom: 12px;
}

.tradeshow-row img {
  flex: 1;
  min-width: 0;
  width: 100%;
  height: 240px;
  object-fit: cover;
  border-radius: 10px;
  display: block;
  transition: transform 0.3s, box-shadow 0.3s;
}

.tradeshow-row img:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

/* CTA 收口 */
.cta-band {
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  border-radius: 14px;
  text-align: center;
  padding: 50px 30px;
  margin: 70px auto 10px;
}

.cta-band h2 {
  color: #fff;
  font-size: 1.7em;
  margin: 0 0 10px;
}

.cta-band p {
  color: #aab0c0;
  margin: 0 0 26px;
}

.cta-band .cta-btn {
  display: inline-block;
  background: #e94560;
  color: #fff;
  padding: 14px 38px;
  border-radius: 30px;
  font-weight: bold;
  text-decoration: none;
  font-size: 1.05em;
  transition: background 0.3s;
}

.cta-band .cta-btn:hover {
  background: #d13a54;
}

.cta-band .cta-contact {
  margin-top: 18px;
  font-size: 0.9em;
}

.cta-band .cta-contact a {
  color: #aab0c0;
  text-decoration: none;
}

.cta-band .cta-contact a:hover {
  color: #fff;
}

/* 响应式 */
@media (max-width: 768px) {
  .stats-band {
    flex-wrap: wrap;
    gap: 20px;
    padding: 22px 16px;
  }

  .stat-cell {
    flex: 1 1 40%;
  }

  .who-grid,
  .factory-grid {
    grid-template-columns: 1fr;
    gap: 30px;
  }

  .cert-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .tradeshow-row {
    flex-wrap: wrap;
  }

  .tradeshow-row img {
    flex: 1 1 45%;
    height: 150px;
  }

  .about-section {
    margin: 50px auto;
  }
}

@media (max-width: 480px) {
  .stat-cell {
    flex: 1 1 40%;
  }

  .stat-cell .num {
    font-size: 1.5em;
  }
}
</style>

<!-- Hero 横幅 -->
<div class="about-hero">
  <img src="/assets/images/about/hero-banner.jpg" alt="Dingyong - stainless steel cutlery manufacturer in Jieyang, Guangdong, China. OEM/ODM, wholesale, private label and export.">
</div>

<!-- 数字统计条 -->
<div class="stats-band">
  <div class="stat-cell">
    <div class="num">12<em>+</em></div>
    <div class="lbl">Years Experience</div>
  </div>
  <div class="stat-cell">
    <div class="num">4,000<em>+</em></div>
    <div class="lbl">㎡ Factory Area</div>
  </div>
  <div class="stat-cell">
    <div class="num">50<em>+</em></div>
    <div class="lbl">Skilled Workers</div>
  </div>
  <div class="stat-cell">
    <div class="num">10M<em>+</em></div>
    <div class="lbl">Pieces Monthly Output</div>
  </div>
</div>

<!-- 我们是谁 -->
<div class="about-section">
  <h2>Who We Are</h2>
  <p class="section-subtitle">A trusted cutlery partner from Jieyang, Guangdong — the heartland of China's stainless steel tableware industry.</p>
  <div class="who-grid">
    <div>
      <p>
        Ding-Yong Products Co., Ltd is a manufacturer specializing in 410
        stainless steel cutlery, flatware, and kitchen utensils. Based in Jieyang,
        Guangdong, we have been serving global B2B buyers for over a decade under
        our own registered brand DINGYONG.
      </p>
      <p>
        Our 4,000+㎡ production facility houses 50+ skilled workers and advanced CNC
        polishing machines, enabling us to produce 10 million+ pieces monthly. From
        small custom orders to large hotel chain contracts, we provide flexible
        OEM/ODM solutions tailored to your market.
      </p>
      <p class="strengths">
        ✓ <strong>Factory Direct</strong> — No middlemen, competitive pricing<br>
        ✓ <strong>Quality Assured</strong> — FDA, LFGB, SGS, ISO9001 certified<br>
        ✓ <strong>Custom Capacity</strong> — Logo engraving, custom packaging, PVD colors<br>
        ✓ <strong>Fast Delivery</strong> — efficient production scheduling and on-time shipping
      </p>
    </div>
    <div class="who-img">
      <img src="/assets/images/tradeshows/tradeshow-04.jpg" alt="Dingyong exhibition stand showcasing stainless steel cutlery sets" loading="lazy">
    </div>
  </div>
</div>

<!-- 工厂视频 + 生产流程 -->
<div class="about-section">
  <h2>Inside Our Factory</h2>
  <p class="section-subtitle">See how your tableware is crafted — from raw steel to finished products.</p>
  <div class="factory-grid">
    <div class="video-box">
      <iframe
        src="https://www.youtube.com/embed/rxGmVh_LP3A?modestbranding=1&controls=1&showinfo=0&rel=0&iv_load_policy=3"
        title="Ding-Yong Factory Tour"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen>
      </iframe>
    </div>
    <div class="process-list">
      <div class="process-item">
        <div class="step-no">1</div>
        <div>
          <h4>Stamping &amp; Forming</h4>
          <p>High-precision presses shape stainless steel blanks into knife, fork and spoon profiles.</p>
        </div>
      </div>
      <div class="process-item">
        <div class="step-no">2</div>
        <div>
          <h4>Polishing</h4>
          <p>Multi-stage CNC and hand polishing deliver the signature mirror finish.</p>
        </div>
      </div>
      <div class="process-item">
        <div class="step-no">3</div>
        <div>
          <h4>Quality Inspection</h4>
          <p>Every batch is checked for finish, edge and food-contact safety before packing.</p>
        </div>
      </div>
      <div class="process-item">
        <div class="step-no">4</div>
        <div>
          <h4>Packing &amp; Export</h4>
          <p>Custom gift boxes, color boxes and export cartons, shipped worldwide.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- 证书墙 -->
<div class="about-section">
  <h2>Certifications &amp; Quality</h2>
  <p class="section-subtitle">Our products passed third-party laboratory testing — safe for food contact, trusted by importers worldwide.</p>
  <div class="cert-grid">
    <div class="cert-card">
      <div class="cert-icon"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 4.9 5.4.8-3.9 3.8.9 5.4L12 14.4 7.2 16.9l.9-5.4L4.2 7.7l5.4-.8L12 2z"/></svg></div>
      <h4>FDA</h4>
      <p>Food-contact material compliance for the US market</p>
    </div>
    <div class="cert-card">
      <div class="cert-icon"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 4.9 5.4.8-3.9 3.8.9 5.4L12 14.4 7.2 16.9l.9-5.4L4.2 7.7l5.4-.8L12 2z"/></svg></div>
      <h4>LFGB</h4>
      <p>German food safety testing — stricter than EU standard</p>
    </div>
    <div class="cert-card">
      <div class="cert-icon"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 4.9 5.4.8-3.9 3.8.9 5.4L12 14.4 7.2 16.9l.9-5.4L4.2 7.7l5.4-.8L12 2z"/></svg></div>
      <h4>SGS</h4>
      <p>Third-party quality inspection and audit reports</p>
    </div>
    <div class="cert-card">
      <div class="cert-icon"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 4.9 5.4.8-3.9 3.8.9 5.4L12 14.4 7.2 16.9l.9-5.4L4.2 7.7l5.4-.8L12 2z"/></svg></div>
      <h4>ISO9001</h4>
      <p>Quality management system across the whole factory</p>
    </div>
  </div>
</div>

<!-- 发展历程 -->
<div class="timeline-section">
  <h2>Our Journey</h2>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-year">2014</div>
      <div class="timeline-text">Entered the stainless steel tableware industry and began manufacturing cutlery and flatware in Jieyang, Guangdong.</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2016</div>
      <div class="timeline-text">Registered our own trademark "DINGYONG", building a dedicated brand identity for our product lines.</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2021</div>
      <div class="timeline-text">Products passed third-party laboratory testing and obtained food-contact safety certifications, including FDA, LFGB and SGS.</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2023</div>
      <div class="timeline-text">Joined Alibaba International Station, opening direct wholesale channels to global B2B buyers.</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2024</div>
      <div class="timeline-text">Expanded our factory to a 4,000+㎡ production facility with upgraded equipment and capacity.</div>
    </div>
  </div>
</div>

<!-- 展会图库 -->
<div class="tradeshow-section">
  <h2>Trade Shows &amp; Exhibitions</h2>
  <p class="section-subtitle">Meet us in person at international trade fairs — real booths, real conversations, real partnerships.</p>

  <div class="tradeshow-row-title">Our Booths</div>
  <div class="tradeshow-row">
    <img src="/assets/images/tradeshows/tradeshow-01.jpg" alt="Dingyong stainless steel cutlery booth at trade fair" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-03.jpg" alt="Stainless steel tableware display at trade show" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-04.jpg" alt="Dingyong exhibition stand with cutlery sets and stainless steel products" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-05.jpg" alt="Dingyong branded booth showing flatware collections" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-06.jpg" alt="Product showcase at stainless steel industry exhibition" loading="lazy">
  </div>

  <div class="tradeshow-row-title">Buyers &amp; Business Talks</div>
  <div class="tradeshow-row">
    <img src="/assets/images/tradeshows/tradeshow-02.jpg" alt="Discussing cutlery collections with overseas buyers at exhibition" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-08.jpg" alt="Buyers reviewing stainless steel flatware samples" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-11.jpg" alt="Visitors at Dingyong trade show stand" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-12.jpg" alt="Buyers examining cutlery sets at exhibition booth" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-14.jpg" alt="Busy booth with buyers from Latin America at tableware fair" loading="lazy">
  </div>

  <div class="tradeshow-row-title">Moments with Clients</div>
  <div class="tradeshow-row">
    <img src="/assets/images/tradeshows/tradeshow-07.jpg" alt="Group photo with international customers at trade fair" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-09.jpg" alt="Team with international clients at cutlery exhibition" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-10.jpg" alt="Happy customers taking selfie at Dingyong booth" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-13.jpg" alt="Team with clients at Canton Fair booth" loading="lazy">
  </div>
</div>

<!-- CTA 收口 -->
<div class="cta-band">
  <h2>Ready to Start Your Order?</h2>
  <p>Get a factory-direct quote, request free samples, or discuss your OEM/ODM project with our team.</p>
  <a class="cta-btn" href="https://wa.me/8615013371880" target="_blank" rel="noopener">Get a Quote on WhatsApp</a>
  <p class="cta-contact">
    Or email us at <a href="mailto:sales@ding-yong.com">sales@ding-yong.com</a> — we reply within 24 hours.
  </p>
</div>
