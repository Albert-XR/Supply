---
layout: page
lang: fr
permalink: /fr/a-propos/
title: À propos de nous
description: "DINGYONG est un fabricant de couverts et de ménagères en acier inoxydable à Guangdong (Chine) — une usine de 5 000 m² produisant couverts, ménagères et accessoires de cuisine pour importateurs, hôtels et marques de retail depuis 2014."
---

<!-- LocalBusiness Schema (About 页，结构化数据保持英文与英文版一致) -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "@id": "https://www.ding-yong.com/about/#localbusiness",
  "name": "Jieyang Dingyong Hardware & Plastic Products Co., Ltd",
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
    "name": "Jieyang Dingyong Hardware & Plastic Products Co., Ltd",
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
  "description": "Watch how your stainless steel tableware is crafted from raw steel to finished products at our 5,000 m² facility in Guangdong, China.",
  "thumbnailUrl": "https://i.ytimg.com/vi/rxGmVh_LP3A/maxresdefault.jpg",
  "uploadDate": "2024-01-01",
  "duration": "PT2M30S",
  "contentUrl": "https://www.youtube.com/watch?v=rxGmVh_LP3A",
  "embedUrl": "https://www.youtube.com/embed/rxGmVh_LP3A",
  "publisher": {
    "@type": "Organization",
    "name": "Jieyang Dingyong Hardware & Plastic Products Co., Ltd",
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

/* 工厂实景图片墙：两行反向匀速滚动 */
.factory-strip {
  position: relative;
  margin: 0 0 46px;
  overflow: hidden;
}

/* 两端半透明白纱：照片轮廓仍可见，模拟画布外的延续 */
.factory-strip::before,
.factory-strip::after {
  content: '';
  position: absolute;
  top: 0;
  bottom: 0;
  width: clamp(72px, 11vw, 160px);
  z-index: 2;
  pointer-events: none;
}

.factory-strip::before {
  left: 0;
  background: linear-gradient(90deg, #fff 12%, rgba(255,255,255,0.72) 52%, rgba(255,255,255,0) 100%);
}

.factory-strip::after {
  right: 0;
  background: linear-gradient(270deg, #fff 12%, rgba(255,255,255,0.72) 52%, rgba(255,255,255,0) 100%);
}

.factory-row {
  overflow: hidden;
  margin-bottom: 26px;
}

.factory-row:last-child {
  margin-bottom: 0;
}

/* 轨道内含两套相同照片，位移到 -50% 时首尾正好重合，循环无缝 */
.factory-track {
  display: flex;
  width: max-content;
  will-change: transform;
  animation: factory-marquee 62s linear infinite;
}

@keyframes factory-marquee {
  from {
    transform: translate3d(0, 0, 0);
  }
  to {
    transform: translate3d(-50%, 0, 0);
  }
}

/* 第二行反向滚 */
.factory-row--reverse .factory-track {
  animation-direction: reverse;
  animation-duration: 74s;
}

.factory-track img {
  flex: 0 0 auto;
  width: clamp(200px, 19vw, 260px);
  height: 200px;
  margin-right: 18px;
  object-fit: cover;
  border-radius: 10px;
  display: block;
  background: #eef0f3;
}

/* 悬停暂停，方便看清某张照片 */
.factory-strip:hover .factory-track {
  animation-play-state: paused;
}

/* 尊重系统的「减少动态效果」设置：停住动画，改回手指滑动 */
@media (prefers-reduced-motion: reduce) {
  .factory-track {
    animation: none;
  }

  .factory-row {
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
  }

  .factory-strip::before,
  .factory-strip::after {
    display: none;
  }
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

/* 产品合规 */
.compliance-panel {
  background: #f8f9fa;
  border-left: 4px solid #1a1a2e;
  border-radius: 12px;
  padding: 30px 32px;
}

.compliance-head {
  display: flex;
  gap: 16px;
  align-items: center;
  margin-bottom: 22px;
}

.compliance-head .compliance-icon {
  width: 52px;
  height: 52px;
  flex-shrink: 0;
  background: #fcebeb;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.compliance-head .compliance-icon svg {
  width: 26px;
  height: 26px;
  fill: #e94560;
}

.compliance-head h3 {
  margin: 0;
  color: #1a1a2e;
  font-size: 1.15em;
}

.compliance-num {
  margin: 4px 0 0;
  color: #e94560;
  font-size: 0.92em;
  font-weight: 600;
}

.compliance-body {
  display: grid;
  grid-template-columns: minmax(0, 400px) minmax(0, 1fr);
  gap: 36px;
  align-items: start;
}

.compliance-doc {
  margin: 0;
}

.compliance-doc img {
  width: 100%;
  display: block;
  border-radius: 8px;
  border: 1px solid #e5e7eb;
  box-shadow: 0 6px 20px rgba(0,0,0,0.09);
}

.compliance-doc figcaption {
  margin-top: 10px;
  font-size: 0.78em;
  color: #8a8f98;
  line-height: 1.55;
}

.compliance-facts {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 16px 20px;
  margin: 0;
}

.compliance-facts dt {
  color: #888;
  font-size: 0.8em;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  margin-bottom: 3px;
}

.compliance-facts dd {
  margin: 0;
  color: #333;
  font-size: 0.95em;
  line-height: 1.55;
}

.compliance-scope {
  margin: 28px 0 0;
  padding-top: 18px;
  border-top: 1px solid #e5e7eb;
  color: #666;
  font-size: 0.9em;
  line-height: 1.7;
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

.tradeshow-note {
  text-align: center;
  margin: 26px 0 0;
  font-size: 0.98em;
}

.tradeshow-note a {
  color: #c8102e;
  font-weight: 600;
  text-decoration: none;
}

.tradeshow-note a:hover {
  text-decoration: underline;
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

  .factory-strip {
    margin-bottom: 34px;
  }

  .factory-strip::before,
  .factory-strip::after {
    width: 46px;
  }

  .factory-row {
    margin-bottom: 14px;
  }

  .factory-track img {
    width: 56vw;
    max-width: 300px;
    height: 172px;
    margin-right: 14px;
  }

  .cert-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .compliance-panel {
    padding: 24px 20px;
  }

  .compliance-body {
    grid-template-columns: 1fr;
    gap: 26px;
  }

  .compliance-facts {
    grid-template-columns: 1fr;
    gap: 14px;
  }

  .compliance-scope {
    margin-top: 22px;
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
  <img src="/assets/images/about/hero-banner.jpg" alt="Dingyong, fabricant de couverts en acier inoxydable à Jieyang, Guangdong, Chine. OEM/ODM, vente en gros, marque propre et export.">
</div>

<!-- 数字统计条 -->
<div class="stats-band">
  <div class="stat-cell">
    <div class="num">12<em>+</em></div>
    <div class="lbl">Années d'expérience</div>
  </div>
  <div class="stat-cell">
    <div class="num">5 000<em>+</em></div>
    <div class="lbl">m² d'usine</div>
  </div>
  <div class="stat-cell">
    <div class="num">200<em>+</em></div>
    <div class="lbl">Employés</div>
  </div>
  <div class="stat-cell">
    <div class="num">10M<em>+</em></div>
    <div class="lbl">Pièces produites par mois</div>
  </div>
</div>

<!-- 我们是谁 -->
<div class="about-section">
  <h2>Qui sommes-nous</h2>
  <p class="section-subtitle">Un partenaire couverts de confiance, basé à Jieyang (Guangdong) — le berceau chinois de l'acier inoxydable pour la table.</p>
  <div class="who-grid">
    <div>
      <p>
        Jieyang Dingyong Hardware &amp; Plastic Products Co., Ltd est un fabricant
        spécialisé dans les couverts, ménagères et accessoires de cuisine en acier
        inoxydable. Basés à Jieyang (Guangdong), nous servons des acheteurs B2B du
        monde entier depuis plus de dix ans, sous notre propre marque enregistrée
        DINGYONG.
      </p>
      <p>
        Notre site de production de plus de 5 000 m² réunit 200 employés et des
        machines de polissage CNC avancées, nous permettant de produire plus de
        10 millions de pièces par mois. Des petites commandes personnalisées aux
        contrats de grandes chaînes hôtelières, nous offrons des solutions OEM/ODM
        flexibles, adaptées à votre marché.
      </p>
      <p class="strengths">
        ✓ <strong>Vente directe d'usine</strong> — Sans intermédiaires, à des prix compétitifs<br>
        ✓ <strong>Qualité garantie</strong> — Inspection avant expédition sur chaque commande, tests en laboratoire indépendant disponibles<br>
        ✓ <strong>Capacité de personnalisation</strong> — Gravure de logo, emballage personnalisé, couleurs PVD<br>
        ✓ <strong>Livraison rapide</strong> — Stock disponible, avec un planning flexible pour les commandes personnalisées
      </p>
    </div>
    <div class="who-img">
      <img src="/assets/images/tradeshows/tradeshow-04.jpg" alt="Stand Dingyong présentant des ménagères en acier inoxydable" loading="lazy">
    </div>
  </div>
</div>

<!-- 工厂视频 + 生产流程 -->
<div class="about-section">
  <h2>Au cœur de notre usine</h2>
  <p class="section-subtitle">Découvrez comment vos couverts sont fabriqués — de l'acier brut au produit fini.</p>

  <div class="factory-strip">
    <div class="factory-row">
      <div class="factory-track">
        <!-- 上行 9 张（原料 → 模具 → 通道 → 压头 → 车间 → 成品仓） -->
        <img src="/assets/images/about/factory/factory-coil.jpg" alt="Rouleaux d'acier inoxydable dans la zone des matières premières" decoding="async">
        <img src="/assets/images/about/factory/factory-die.jpg" alt="Presse à emboutir avec moule progressif et système d'alimentation" decoding="async">
        <img src="/assets/images/about/factory/factory-corridor.jpg" alt="Allée entre les rangées de machines de l'atelier" decoding="async">
        <img src="/assets/images/about/factory/factory-press-head.jpg" alt="Tête de presse et outillage avec circuits de lubrification" decoding="async">
        <img src="/assets/images/about/factory/factory-shopfloor.jpg" alt="Vue d'ensemble de l'atelier d'emboutissage" decoding="async">
        <img src="/assets/images/about/factory/factory-cartons.jpg" alt="Cartons emballés sur palettes dans la zone des produits finis" decoding="async">
        <img src="/assets/images/about/factory/factory-wheel.jpg" alt="Volant et transmission d'une presse mécanique" decoding="async">
        <img src="/assets/images/about/factory/factory-operator.jpg" alt="Opérateur chargeant des pièces sur une presse" decoding="async">
        <img src="/assets/images/about/factory/factory-press.jpg" alt="Presse mécanique formant les ébauches de couverts" decoding="async">
        <!-- 复制一整套：轨道滚到 -50% 时首尾重合，形成无缝循环 -->
        <img src="/assets/images/about/factory/factory-coil.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-die.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-corridor.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-press-head.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-shopfloor.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-cartons.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-wheel.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-operator.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-press.jpg" alt="" aria-hidden="true" decoding="async">
      </div>
    </div>
    <div class="factory-row factory-row--reverse">
      <div class="factory-track">
        <!-- 下行另外 9 张：同一车间、不同机位，与上行不重复一张 -->
        <img src="/assets/images/about/factory/factory-b-coil.jpg" alt="Rouleaux d'acier inoxydable stockés dans la cour extérieure" decoding="async">
        <img src="/assets/images/about/factory/factory-b-machinist.jpg" alt="Opérateur réglant une presse à emboutir" decoding="async">
        <img src="/assets/images/about/factory/factory-b-workshop.jpg" alt="Rangées de presses à emboutir dans l'atelier" decoding="async">
        <img src="/assets/images/about/factory/factory-b-tooling.jpg" alt="Outillage de transfert et alimentation sécurisée" decoding="async">
        <img src="/assets/images/about/factory/factory-b-aisle.jpg" alt="Passerelle longeant les lignes de presses" decoding="async">
        <img src="/assets/images/about/factory/factory-b-press.jpg" alt="Postes de presses bleues dans l'atelier d'emboutissage" decoding="async">
        <img src="/assets/images/about/factory/factory-b-feed.jpg" alt="Dérouleur alimentant une ligne de presse en bande d'acier" decoding="async">
        <img src="/assets/images/about/factory/factory-b-workbench.jpg" alt="Établis et chariots de matière dans l'atelier" decoding="async">
        <img src="/assets/images/about/factory/factory-b-floor.jpg" alt="Atelier d'emboutissage lumineux avec rangées de machines" decoding="async">
        <!-- 复制一整套：轨道滚到 -50% 时首尾重合，形成无缝循环 -->
        <img src="/assets/images/about/factory/factory-b-coil.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-b-machinist.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-b-workshop.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-b-tooling.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-b-aisle.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-b-press.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-b-feed.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-b-workbench.jpg" alt="" aria-hidden="true" decoding="async">
        <img src="/assets/images/about/factory/factory-b-floor.jpg" alt="" aria-hidden="true" decoding="async">
      </div>
    </div>
  </div>

  <div class="factory-grid">
    <div class="video-box">
      <iframe
        src="https://www.youtube.com/embed/rxGmVh_LP3A?modestbranding=1&controls=1&showinfo=0&rel=0&iv_load_policy=3"
        title="Visite de l'usine Ding-Yong"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen>
      </iframe>
    </div>
    <div class="process-list">
      <div class="process-item">
        <div class="step-no">1</div>
        <div>
          <h4>Emboutissage &amp; formage</h4>
          <p>Des presses de haute précision découpent et forment les ébauches d'acier inoxydable en couteaux, fourchettes et cuillères.</p>
        </div>
      </div>
      <div class="process-item">
        <div class="step-no">2</div>
        <div>
          <h4>Polissage</h4>
          <p>Un polissage CNC en plusieurs étapes, complété à la main, donne la finition miroir signature de la maison.</p>
        </div>
      </div>
      <div class="process-item">
        <div class="step-no">3</div>
        <div>
          <h4>Contrôle qualité</h4>
          <p>Chaque lot est vérifié : finition, arêtes et sécurité au contact alimentaire, avant l'emballage.</p>
        </div>
      </div>
      <div class="process-item">
        <div class="step-no">4</div>
        <div>
          <h4>Emballage &amp; export</h4>
          <p>Coffrets cadeaux sur mesure, boîtes couleur et cartons d'export, expédiés dans le monde entier.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- 质量保障 -->
<div class="about-section">
  <h2>Assurance qualité</h2>
  <p class="section-subtitle">Chaque commande suit un processus qualité structuré — de la confirmation d'échantillon à l'inspection avant expédition.</p>
  <div class="cert-grid">
    <div class="cert-card">
      <div class="cert-icon"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 4.9 5.4.8-3.9 3.8.9 5.4L12 14.4 7.2 16.9l.9-5.4L4.2 7.7l5.4-.8L12 2z"/></svg></div>
      <h4>Confirmation d'échantillon</h4>
      <p>Validation des échantillons pré-production avant le lancement en série</p>
    </div>
    <div class="cert-card">
      <div class="cert-icon"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 4.9 5.4.8-3.9 3.8.9 5.4L12 14.4 7.2 16.9l.9-5.4L4.2 7.7l5.4-.8L12 2z"/></svg></div>
      <h4>Inspection avant expédition</h4>
      <p>Chaque commande est contrôlée (finition, fonction, emballage) avant départ</p>
    </div>
    <div class="cert-card">
      <div class="cert-icon"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 4.9 5.4.8-3.9 3.8.9 5.4L12 14.4 7.2 16.9l.9-5.4L4.2 7.7l5.4-.8L12 2z"/></svg></div>
      <h4>Tests en laboratoire indépendant</h4>
      <p>SGS ou autres laboratoires indépendants, organisés à la demande</p>
    </div>
    <div class="cert-card">
      <div class="cert-icon"><svg viewBox="0 0 24 24"><path d="M12 2l2.4 4.9 5.4.8-3.9 3.8.9 5.4L12 14.4 7.2 16.9l.9-5.4L4.2 7.7l5.4-.8L12 2z"/></svg></div>
      <h4>Audit d'usine bienvenu</h4>
      <p>Visitez notre usine à Jieyang ou inspectez la production en visioconférence. <a href="/visit-our-factory/">Itinéraires &amp; organisation de la visite (EN) &rarr;</a></p>
    </div>
  </div>
</div>

<!-- 产品合规 -->
<div class="about-section">
  <h2>Conformité des produits</h2>
  <p class="section-subtitle">Une conformité documentée là où le marché l'exige — et une transparence totale là où elle ne s'applique pas.</p>
  <div class="compliance-panel">
    <div class="compliance-body">
      <figure class="compliance-doc">
        <img src="/assets/images/about/ru-declaration-gostr.jpg" alt="Déclaration nationale russe de conformité, numéro d'enregistrement РОСС RU Д-CN.РА01.В.29537/26, valide jusqu'au 24 août 2031" loading="lazy">
        <figcaption>Extrait du registre d'État (Rosaccreditation) — numéro d'enregistrement, statut et validité.</figcaption>
      </figure>
      <div class="compliance-info">
    <div class="compliance-head">
      <div class="compliance-icon"><svg viewBox="0 0 24 24"><path d="M12 1L3 5v6c0 5.6 3.8 10.7 9 12 5.2-1.3 9-6.4 9-12V5l-9-4zm-1.1 15.2L6.8 12l1.4-1.4 2.7 2.7 5.4-5.4 1.4 1.4-6.8 6.9z"/></svg></div>
      <div>
        <h3>Déclaration nationale russe de conformité</h3>
        <p class="compliance-num">N° РОСС RU Д-CN.РА01.В.29537/26</p>
      </div>
    </div>
    <dl class="compliance-facts">
      <div>
        <dt>Norme</dt>
        <dd>GOST R 51687-2021 — vaisselle et ustensiles de cuisine en acier inoxydable, conditions techniques générales</dd>
      </div>
      <div>
        <dt>Enregistrée le</dt>
        <dd>26 août 2026</dd>
      </div>
      <div>
        <dt>Valable jusqu'au</dt>
        <dd>24 août 2031</dd>
      </div>
      <div>
        <dt>Fabricant déclaré</dt>
        <dd>Jieyang Dingyong Hardware &amp; Plastic Products Co., Ltd</dd>
      </div>
      <div>
        <dt>Titulaire de la déclaration</dt>
        <dd>Représentant autorisé dans la Fédération de Russie</dd>
      </div>
      <div>
        <dt>Laboratoire d'essais</dt>
        <dd>Laboratoire accrédité, accréditation N° RA.RU.21ОМ79</dd>
      </div>
        </dl>
      </div>
    </div>
    <p class="compliance-scope">
      <strong>Portée :</strong> cette déclaration est enregistrée auprès du système national de conformité de la Fédération
      de Russie (GOST R) et est valable pour le marché russe. Elle ne constitue pas une approbation à l'échelle de
      l'Union économique eurasienne (UEE) et ne s'étend pas aux autres destinations. Pour la FDA, la LFGB ou toute
      autre exigence propre à un marché, nous organisons les tests avec un laboratoire indépendant avant expédition —
      indiquez-nous votre marché cible et nous confirmerons la documentation nécessaire.
    </p>
  </div>
</div>

<!-- 发展历程 -->
<div class="timeline-section">
  <h2>Notre parcours</h2>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-year">2014</div>
      <div class="timeline-text">Entrée dans l'industrie de l'acier inoxydable pour la table et début de la fabrication de couverts à Jieyang (Guangdong).</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2016</div>
      <div class="timeline-text">Enregistrement de notre propre marque « DINGYONG », avec une identité de marque dédiée à nos gammes de produits.</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2021</div>
      <div class="timeline-text">Standardisation de notre processus qualité — confirmation d'échantillon et inspection avant expédition sur chaque commande.</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2023</div>
      <div class="timeline-text">Adhésion à Alibaba Station Internationale, ouverture de canaux de vente en gros en direct vers les acheteurs B2B mondiaux.</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2024</div>
      <div class="timeline-text">Agrandissement de l'usine à plus de 5 000 m² avec des équipements et une capacité modernisés.</div>
    </div>
    <div class="timeline-item">
      <div class="timeline-year">2026</div>
      <div class="timeline-text">Enregistrement de notre vaisselle en acier inoxydable sous une Déclaration nationale russe de conformité GOST R 51687-2021, ajoutant un accès documenté au marché de la Fédération de Russie.</div>
    </div>
  </div>
</div>

<!-- 展会图库 -->
<div class="tradeshow-section">
  <h2>Salons &amp; expositions</h2>
  <p class="section-subtitle">Rencontrez-nous en personne lors des salons internationaux — de vrais stands, de vraies conversations, de vrais partenariats.</p>

  <div class="tradeshow-row-title">Nos stands</div>
  <div class="tradeshow-row">
    <img src="/assets/images/tradeshows/tradeshow-01.jpg" alt="Stand Dingyong de couverts en acier inoxydable au salon" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-03.jpg" alt="Présentation de vaisselle en acier inoxydable au salon" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-04.jpg" alt="Stand Dingyong avec ménagères et produits en acier inoxydable" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-05.jpg" alt="Stand Dingyong présentant les collections de couverts" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-06.jpg" alt="Vitrine produits au salon de l'acier inoxydable" loading="lazy">
  </div>

  <div class="tradeshow-row-title">Acheteurs &amp; négociations</div>
  <div class="tradeshow-row">
    <img src="/assets/images/tradeshows/tradeshow-02.jpg" alt="Discussion sur les collections de couverts avec des acheteurs étrangers au salon" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-08.jpg" alt="Acheteurs examinant des échantillons de couverts en acier inoxydable" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-11.jpg" alt="Visiteurs sur le stand Dingyong" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-12.jpg" alt="Acheteurs examinant des ménagères au stand du salon" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-14.jpg" alt="Stand animé avec des acheteurs d'Amérique latine au salon de la vaisselle" loading="lazy">
  </div>

  <div class="tradeshow-row-title">Moments avec nos clients</div>
  <div class="tradeshow-row">
    <img src="/assets/images/tradeshows/tradeshow-07.jpg" alt="Photo de groupe avec des clients internationaux au salon" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-09.jpg" alt="L'équipe avec des clients internationaux au salon des couverts" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-10.jpg" alt="Clients heureux prenant un selfie au stand Dingyong" loading="lazy">
    <img src="/assets/images/tradeshows/tradeshow-13.jpg" alt="L'équipe avec des clients au stand de la Canton Fair" loading="lazy">
  </div>

  <p class="tradeshow-note">
    <a href="/jinhan-fair-2026/">Jinhan Fair 2026, Guangzhou — stand 7B01 : photos, vidéo et retours des acheteurs (EN) &rarr;</a>
  </p>
</div>

<!-- CTA 收口 -->
<div class="cta-band">
  <h2>Prêt à lancer votre commande ?</h2>
  <p>Obtenez un devis direct usine, demandez des échantillons gratuits ou parlez de votre projet OEM/ODM avec notre équipe.</p>
  <a class="cta-btn" href="https://wa.me/8615013371880" target="_blank" rel="noopener">Obtenir un devis sur WhatsApp</a>
  <p class="cta-contact">
    Ou écrivez-nous à <a href="mailto:sales@ding-yong.com">sales@ding-yong.com</a> — nous répondons sous 24 heures.
  </p>
</div>
