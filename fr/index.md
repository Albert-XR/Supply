---
layout: home
lang: fr
permalink: /fr/
title: Fabricant de couverts en acier inoxydable & fournisseur OEM
description: "DINGYONG, fabricant de couverts en acier inoxydable basé à Guangdong (Chine) : ménagères, couverts et coffrets cadeaux pour importateurs, grossistes, hôtels et restaurants — OEM/ODM avec logo et emballage personnalisés."
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
  display: flex;
  flex-direction: column;
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
  display: flex;
  flex-direction: column;
  flex: 1;
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
  margin-top: auto;
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

/* FAQ 常见问题 */
.faq-list {
  max-width: 800px;
  margin: 0 auto;
}

.faq-item {
  background: white;
  border: 1px solid #e8e8e8;
  border-radius: 8px;
  margin-bottom: 12px;
  transition: box-shadow 0.3s, border-color 0.3s;
}

.faq-item[open] {
  border-color: #e94560;
  box-shadow: 0 4px 15px rgba(0,0,0,0.08);
}

.faq-item summary {
  padding: 16px 48px 16px 20px;
  cursor: pointer;
  font-weight: bold;
  color: #1a1a2e;
  list-style: none;
  position: relative;
  font-size: 0.98em;
}

.faq-item summary::-webkit-details-marker { display: none; }

.faq-item summary::after {
  content: '+';
  position: absolute;
  right: 20px;
  top: 50%;
  transform: translateY(-50%);
  font-size: 1.5em;
  font-weight: normal;
  color: #e94560;
  line-height: 1;
  transition: transform 0.3s;
}

.faq-item[open] summary::after {
  transform: translateY(-50%) rotate(45deg);
}

.faq-answer {
  padding: 0 20px 16px;
  color: #555;
  line-height: 1.7;
  font-size: 0.92em;
}
</style>

<!-- FAQ 结构化数据（与下方可见 Q&A 逐字一致） -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Fournissez-vous des échantillons gratuits ?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Oui. Nous fournissons gratuitement des échantillons de nos modèles existants — vous ne payez que le transport. Des échantillons personnalisés avec votre logo peuvent également être réalisés ; contactez-nous et nous confirmerons les modalités pour votre projet."
      }
    },
    {
      "@type": "Question",
      "name": "Proposez-vous l'OEM/ODM, le logo et l'emballage personnalisés ?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Oui. Nous prenons en charge la gravure laser du logo, les couleurs PVD personnalisées, les moules sur mesure et les coffrets cadeaux adaptés. Notre équipe de design interne vous accompagne du dessin au produit fini."
      }
    },
    {
      "@type": "Question",
      "name": "Comment garantissez-vous la qualité des produits ?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Chaque commande passe par la confirmation d'échantillon et une inspection avant expédition. Des tests en laboratoire indépendant (type SGS) peuvent être organisés à la demande, et les audits d'usine ou inspections par visioconférence sont les bienvenus."
      }
    }
  ]
}
</script>

<!-- 首屏横幅 -->
<div class="hero">
  <h1>JIEYANG DINGYONG HARDWARE &amp; PLASTIC PRODUCTS CO., LTD</h1>
  <p class="hero-subtitle">Votre partenaire de confiance pour les solutions de couverts OEM/ODM</p>
  <div class="hero-badges">
    <span>✓ Contrôle qualité avant expédition sur chaque commande</span>
    <span>✓ Tests en laboratoire indépendant à la demande</span>
    <span>✓ Plus de 12 ans d'expérience à l'export</span>
  </div>
  <a href="/fr/produits/" class="cta-button">Voir les produits</a>
  <a href="/fr/contact/" class="cta-button secondary">Demander un devis</a>
</div>

<!-- 核心数据 -->
<div class="stats-bar">
  <div class="stat-item">
    <strong>600+</strong>
    <span>Modèles de produits</span>
  </div>
  <div class="stat-item">
    <strong>40+</strong>
    <span>Pays d'exportation</span>
  </div>
  <div class="stat-item">
    <strong>10M+</strong>
    <span>Pièces produites par mois</span>
  </div>
  <div class="stat-item">
    <strong>200+</strong>
    <span>Employés</span>
  </div>
</div>

<!-- 产品分类 -->
<section>
  <h2>Nos gammes de produits</h2>
  <div class="category-grid">

    <div class="category-card">
      <img src="/assets/images/home/goldbox-400.jpg" alt="Ménagère dorée en coffret cadeau avec manches gravés" loading="lazy">
      <div class="category-info">
        <h3>Ménagères et coffrets</h3>
        <p>Ménagères 24/72 pièces en coffret, finitions miroir et dorée — pour la vente au détail, les hôtels et les restaurants</p>
        <a href="/fr/produits/">Voir les produits →</a>
      </div>
    </div>

    <div class="category-card">
      <img src="/assets/images/home/portugal-400.jpg" alt="Couverts série Portugal avec revêtement titane multicolore" loading="lazy">
      <div class="category-info">
        <h3>Couverts</h3>
        <p>Couteaux, fourchettes et cuillères en finition miroir, satinée ou titane PVD multicolore — série Portugal et designs sur mesure</p>
        <a href="/fr/produits/">Voir les produits →</a>
      </div>
    </div>

    <div class="category-card">
      <img src="/assets/images/home/kitchen-400.jpg" alt="Set anti-brûlure de cuisine" loading="lazy">
      <div class="category-info">
        <h3>Accessoires de cuisine</h3>
        <p>Pinces anti-brûlure, maniques et demi-moufles en silicone, designs brevetés, matériaux résistants à la chaleur pour contact alimentaire</p>
        <a href="/fr/produits/">Voir les produits →</a>
      </div>
    </div>

    <div class="category-card">
      <img src="/assets/images/home/christmas-400.jpg" alt="Coffret cadeau de cuillères à dessert thème Noël" loading="lazy">
      <div class="category-info">
        <h3>Coffrets cadeaux de fêtes</h3>
        <p>Coffrets de cuillères et fourchettes thème Noël et fêtes, figurines amusantes et boîtes festives, parfaits pour la vente saisonnière</p>
        <a href="/fr/produits/">Voir les produits →</a>
      </div>
    </div>

  </div>
</section>

<!-- 为什么选择我们 -->
<section>
  <h2>Pourquoi choisir DINGYONG</h2>
  <div class="features-grid">
    <div class="feature">
      <h4>🏭 Vente directe d'usine</h4>
      <p>Site de production de 5 000 m², moules sur mesure, finitions (PVD/miroir/satin) et marquage de votre marque.</p>
    </div>
    <div class="feature">
      <h4>🔬 Qualité garantie</h4>
      <p>Contrôle qualité interne rigoureux avec inspection avant expédition sur chaque commande.</p>
    </div>
    <div class="feature">
      <h4>🚢 Production réactive</h4>
      <p>Planification flexible et délais optimisés pour un lancement rapide sur votre marché.</p>
    </div>
    <div class="feature">
      <h4>🎨 Présence mondiale</h4>
      <p>Une expérience éprouvée auprès de clients en Europe, Amériques, Moyen-Orient et Asie du Sud-Est — plus de 40 pays.</p>
    </div>
  </div>
</section>

<!-- 采购指南（内链博客，英文）-->
<section>
  <h2>Guides d'achat</h2>
  <p style="text-align:center;color:#666;font-size:0.9em;margin-bottom:20px;">Nos guides d'achat détaillés sont disponibles en anglais :</p>
  <div class="features-grid">
    {% for post in site.posts limit:3 %}
    <div class="feature">
      <h4 style="margin-bottom:8px;">
        <a href="{{ post.url }}" style="color:#1a1a2e;text-decoration:none;">{{ post.title }}</a>
      </h4>
      <p style="color:#666;font-size:0.9em;line-height:1.6;margin-bottom:10px;">{{ post.description | truncate: 130 }}</p>
      <a href="{{ post.url }}" style="color:#e94560;font-weight:bold;font-size:0.9em;">Lire le guide (EN) →</a>
    </div>
    {% endfor %}
  </div>
</section>

<!-- 服务市场（内链市场着陆页，英文）-->
<section>
  <h2>Marchés que nous servons</h2>
  <div class="features-grid">
    <div class="feature">
      <h4>Pakistan</h4>
      <p>Fourniture de couverts en acier inoxydable pour importateurs et grossistes à Karachi, Lahore et dans tout le Pakistan.</p>
      <a href="/markets/pakistan/" style="color:#e94560;font-weight:bold;font-size:0.9em;">Pour les acheteurs pakistanais (EN) →</a>
    </div>
    <div class="feature">
      <h4>Afrique de l'Ouest</h4>
      <p>Couverts et ménagères en gros pour les importateurs du Ghana, du Mali, du Togo et des pays voisins d'Afrique de l'Ouest.</p>
      <a href="/markets/west-africa/" style="color:#e94560;font-weight:bold;font-size:0.9em;">Pour les acheteurs ouest-africains (EN) →</a>
    </div>
  </div>
</section>

<!-- 常见问题 -->
<section>
  <h2>Questions fréquentes</h2>
  <div class="faq-list">

    <details class="faq-item">
      <summary>Fournissez-vous des échantillons gratuits ?</summary>
      <div class="faq-answer">
        Oui. Nous fournissons gratuitement des échantillons de nos modèles existants — vous ne payez que le transport. Des échantillons personnalisés avec votre logo peuvent également être réalisés ; contactez-nous et nous confirmerons les modalités pour votre projet.
      </div>
    </details>

    <details class="faq-item">
      <summary>Proposez-vous l'OEM/ODM, le logo et l'emballage personnalisés ?</summary>
      <div class="faq-answer">
        Oui. Nous prenons en charge la gravure laser du logo, les couleurs PVD personnalisées, les moules sur mesure et les coffrets cadeaux adaptés. Notre équipe de design interne vous accompagne du dessin au produit fini.
      </div>
    </details>

    <details class="faq-item">
      <summary>Comment garantissez-vous la qualité des produits ?</summary>
      <div class="faq-answer">
        Chaque commande passe par la confirmation d'échantillon et une inspection avant expédition. Des tests en laboratoire indépendant (type SGS) peuvent être organisés à la demande, et les audits d'usine ou inspections par visioconférence sont les bienvenus.
      </div>
    </details>

  </div>
</section>
