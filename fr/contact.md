---
layout: page
lang: fr
permalink: /fr/contact/
title: Contactez-nous
description: "Contactez DINGYONG pour la vente en gros de couverts en acier inoxydable, l'OEM/ODM et les demandes de logo personnalisé. WhatsApp +86 15013371880 ou email sales@ding-yong.com — nous répondons à chaque demande."
---

<style>
.contact-page h1 { text-align: center; margin-bottom: 10px; }
.contact-intro { text-align: center; color: #666; margin-bottom: 40px; }

.contact-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
  margin-bottom: 50px;
}

.contact-info h2 { margin-bottom: 20px; color: #1a1a2e; }

.info-item {
  display: flex;
  align-items: flex-start;
  margin-bottom: 25px;
  padding: 20px;
  background: #f8f9fa;
  border-radius: 10px;
}

.info-icon {
  font-size: 1.8em;
  margin-right: 15px;
  width: 50px;
  height: 50px;
  background: #e94560;
  color: white;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.info-content h4 { margin: 0 0 5px 0; color: #1a1a2e; }
.info-content p { margin: 0; color: #555; font-size: 0.95em; }
.info-content a { color: #e94560; text-decoration: none; }

.inquiry-guide {
  background: #f8f9fa;
  padding: 30px;
  border-radius: 12px;
}

.inquiry-guide h2 { margin-bottom: 20px; color: #1a1a2e; }

.tip-box {
  background: #e8f4fd;
  padding: 20px;
  border-radius: 10px;
  margin-bottom: 25px;
  border-left: 4px solid #2196F3;
}

.tip-box p { margin: 0; font-size: 0.95em; }
.tip-box ul { margin: 10px 0 0 20px; font-size: 0.9em; color: #555; }

.contact-method {
  text-align: center;
  padding: 25px 20px;
  background: white;
  border-radius: 10px;
  margin-bottom: 20px;
  border: 1px solid #e0e0e0;
}

.contact-method .method-icon {
  font-size: 2.5em;
  margin-bottom: 10px;
}

.contact-method h4 { margin: 5px 0; color: #1a1a2e; }
.contact-method a {
  color: #e94560;
  font-size: 1.1em;
  text-decoration: none;
  font-weight: bold;
}
.contact-method p {
  font-size: 0.85em;
  color: #888;
  margin-top: 5px;
}

.whatsapp-btn {
  display: block;
  width: 100%;
  padding: 16px;
  background: #25D366;
  color: white;
  text-align: center;
  border-radius: 8px;
  text-decoration: none;
  font-size: 1.1em;
  font-weight: bold;
  margin-top: 10px;
}

.inquiry-template {
  background: white;
  padding: 25px;
  border-radius: 10px;
  margin-top: 25px;
  border: 1px solid #e0e0e0;
}

.inquiry-template h4 {
  margin: 0 0 15px 0;
  color: #1a1a2e;
}

.inquiry-template pre {
  background: #f5f5f5;
  padding: 15px;
  border-radius: 6px;
  font-size: 0.85em;
  line-height: 1.6;
  color: #555;
  overflow-x: auto;
  white-space: pre-wrap;
  word-wrap: break-word;
}

.copy-btn {
  display: inline-block;
  margin-top: 10px;
  padding: 8px 16px;
  background: #e94560;
  color: white;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-size: 0.9em;
}

.contact-form {
  background: white;
  padding: 25px;
  border-radius: 12px;
  border: 1px solid #e0e0e0;
  margin-bottom: 25px;
}
.contact-form h3 { margin: 0 0 18px 0; color: #1a1a2e; }
.contact-form input,
.contact-form select,
.contact-form textarea {
  width: 100%;
  padding: 12px 14px;
  border: 1px solid #ddd;
  border-radius: 6px;
  font-size: 0.95em;
  font-family: inherit;
  margin-bottom: 14px;
  box-sizing: border-box;
  background: #fff;
  color: #333;
}
.contact-form input:focus,
.contact-form select:focus,
.contact-form textarea:focus {
  outline: none;
  border-color: #e94560;
}
.cform-row { display: flex; gap: 14px; }
.cform-row > * { flex: 1; }
.submit-btn {
  width: 100%;
  padding: 14px;
  background: #e94560;
  color: white;
  border: none;
  border-radius: 6px;
  font-size: 1.05em;
  font-weight: bold;
  cursor: pointer;
}
.submit-btn:hover { background: #d1334d; }

@media (max-width: 768px) {
  .cform-row { flex-direction: column; gap: 0; }
}

@media (max-width: 768px) {
  .contact-grid { grid-template-columns: 1fr; }
}

.cta-bottom {
  background: #1a1a2e;
  color: white;
  padding: 50px 30px;
  text-align: center;
  border-radius: 12px;
  margin-top: 40px;
}

.cta-bottom h3 { margin-bottom: 10px; }
.cta-bottom p { opacity: 0.9; margin-bottom: 20px; }

.cta-button {
  display: inline-block;
  background: #e94560;
  color: white;
  padding: 14px 32px;
  border-radius: 6px;
  text-decoration: none;
  font-weight: bold;
  margin: 5px;
}

.cta-button.secondary {
  background: transparent;
  border: 2px solid white;
}

/* 表单上方提示语 */
.guide-text {
  color: #555;
  margin: 0 0 18px 0;
  font-size: 0.95em;
  line-height: 1.5;
}

/* 邮件模板（全宽 section） */
.inquiry-template-full {
  background: #f8f9fa;
  padding: 30px;
  border-radius: 12px;
  margin-top: 30px;
}
.inquiry-template-full h3 {
  color: #1a1a2e;
  margin: 0 0 8px 0;
}
.inquiry-template-full > p {
  color: #666;
  font-size: 0.9em;
  margin: 0 0 15px 0;
}
/* 模板 pre 必须换行，否则长行在手机上撑破布局（存量 bug，英文版同步修） */
.inquiry-template-full pre {
  background: #f5f5f5;
  padding: 15px;
  border-radius: 6px;
  font-size: 0.85em;
  line-height: 1.6;
  color: #555;
  overflow-x: auto;
  white-space: pre-wrap;
  word-wrap: break-word;
}
</style>

<div class="contact-page">
<h1>Contactez-nous</h1>
<p class="contact-intro">Contactez-nous pour des devis, des échantillons ou une visite d'usine. Nous répondons sous 24 heures.</p>

<div class="contact-grid">

<div class="contact-info">
<h2>Restons en contact</h2>

<div class="info-item">
<div class="info-icon">&#9993;</div>
<div class="info-content">
<h4>Email</h4>
<p><a href="mailto:sales@ding-yong.com">sales@ding-yong.com</a></p>
<p style="font-size: 0.85em; color: #888; margin-top: 5px;">Pour les devis et demandes générales</p>
</div>
</div>

<div class="info-item">
<div class="info-icon">&#128241;</div>
<div class="info-content">
<h4>WhatsApp / WeChat</h4>
<p><a href="https://wa.me/8615013371880" target="_blank">+86 150-1337-1880</a></p>
<p style="font-size: 0.85em; color: #888; margin-top: 5px;">La réponse la plus rapide pour les demandes urgentes</p>
</div>
</div>

<div class="info-item">
<div class="info-icon">&#127981;</div>
<div class="info-content">
<h4>Adresse de l'usine</h4>
<p>No. 2, 1st Floor, Maifeng Commercial Building, Chating Road, Xixi Village, Xichang Town, Jiedong District, Jieyang City, Guangdong Province, China</p>
<p style="font-size: 0.85em; margin-top: 6px;"><a href="/visit-our-factory/">Vous nous rendez visite ? Itinéraires &amp; service de navette (EN) &rarr;</a></p>
</div>
</div>

<div class="info-item">
<div class="info-icon">&#128336;</div>
<div class="info-content">
<h4>Horaires de travail</h4>
<p>Lundi - Samedi : 8h30 - 18h00 (GMT+8)</p>
<p>Dimanche : fermé</p>
</div>
</div>

</div>

<div class="inquiry-guide">
<h2>Envoyez-nous votre demande</h2>
<p class="guide-text">Nous répondons sous 24 heures. Pour une réponse plus rapide, précisez le produit visé, la quantité et le pays de destination.</p>

<div class="contact-form">
<form action="https://api.web3forms.com/submit" method="POST">
  <input type="hidden" name="access_key" value="{{ site.web3forms_access_key }}">
  <input type="hidden" name="subject" value="New Website Inquiry from FR Contact Page">
  <input type="hidden" name="redirect" id="form-redirect" value="">
  <script>document.getElementById('form-redirect').value = window.location.origin + '/thank-you/';</script>
  <input type="checkbox" name="botcheck" class="hidden" style="display:none;" tabindex="-1" autocomplete="off">
  <div class="cform-row">
    <input type="text" name="name" placeholder="Votre nom *" required>
    <input type="email" name="email" placeholder="Adresse email *" required>
  </div>
  <div class="cform-row">
    <input type="text" name="company" placeholder="Société (facultatif)">
    <input type="text" name="country" placeholder="Pays / Région">
  </div>
  <div class="cform-row">
    <select name="quantity" required>
      <option value="">Quantité visée *</option>
      <option value="Samples first">D'abord des échantillons</option>
      <option value="Not sure yet">Pas encore sûr — merci de conseiller</option>
      <option value="Under 1,000 pcs">Moins de 1 000 pièces</option>
      <option value="1,000 - 5,000 pcs">1 000 - 5 000 pièces</option>
      <option value="5,000 - 10,000 pcs">5 000 - 10 000 pièces</option>
      <option value="10,000+ pcs">Plus de 10 000 pièces</option>
    </select>
  </div>
  <textarea name="message" rows="4" placeholder="Parlez-nous de vos besoins (produit, matériau, finition, emballage, logo...)"></textarea>
  <button type="submit" class="submit-btn">Envoyer la demande</button>
</form>
</div>

<a href="https://wa.me/8615013371880" target="_blank" class="whatsapp-btn">&#128172; Discuter sur WhatsApp</a>

</div>

</div>

<div class="inquiry-template-full">
<h3>&#128203; Modèle d'email à copier-coller</h3>
<p>Vous préférez l'email ? Copiez ce modèle et envoyez-le à <a href="mailto:sales@ding-yong.com">sales@ding-yong.com</a> :</p>
<pre id="templateText">Bonjour,

Je suis intéressé(e) par vos produits en acier inoxydable pour la table. Voici le détail de ma demande :

Produit visé : [ex. Ménagère 24 pièces en coffret / Série Portugal / OEM sur mesure]
Quantité : [ex. 3 000 lots]
Pays de destination : [ex. Mali / Togo / France]

Exigences :
- Matériau : [410 / 18/0 / 304]
- Finition : [Poli miroir / Satiné / Doré]
- Emballage : [Boîte couleur / Blister / Personnalisé]
- Logo : [Gravure laser / Aucun]
- Livraison : [FOB / CIF / DDP]

Merci de m'envoyer votre meilleure offre et votre catalogue.

Cordialement,
[Votre nom]
[Votre société]
[Votre WhatsApp/Email]</pre>
<button class="copy-btn" onclick="copyTemplate()">&#128203; Copier le modèle</button>
</div>

</div>

<script>
// 询盘表单埋点
// 说明：Web3Forms 是整页 POST 跳转（跳到 api.web3forms.com 再 302 回 /thank-you/），
// 所以「提交成功」的信号由 thank-you.md 负责。这里只记录「开始填写」和「点了提交」，
// 并把国家/数量/来源产品写进 sessionStorage，供感谢页读取做归因。
document.addEventListener('DOMContentLoaded', function () {
  var form = document.querySelector('.contact-form form');
  if (!form) return;

  var started = false;
  form.addEventListener('input', function () {
    if (started) return;
    started = true;
    if (typeof gtag === 'function') gtag('event', 'form_start', { form_name: 'inquiry_fr' });
  });

  form.addEventListener('submit', function () {
    if (typeof gtag === 'function') {
      gtag('event', 'form_submit', { form_name: 'inquiry_fr', transport_type: 'beacon' });
    }
    try {
      var q = form.querySelector('[name="quantity"]');
      var c = form.querySelector('[name="country"]');
      sessionStorage.setItem('dy_inquiry_ctx', JSON.stringify({
        quantity: q ? q.value : '',
        country: c ? c.value : '',
        product: new URLSearchParams(location.search).get('product') || ''
      }));
    } catch (err) { /* 隐私模式等场景下静默失败，不阻断提交 */ }
  });
});

function copyTemplate() {
  var text = document.getElementById('templateText').innerText;
  navigator.clipboard.writeText(text).then(function () {
    if (typeof gtag === 'function') gtag('event', 'template_copy', { page_path: location.pathname });
    var btn = document.querySelector('.copy-btn');
    btn.textContent = '\u2705 Copié !';
    setTimeout(function () {
      btn.textContent = '\uD83D\uDCCB Copier le modèle';
    }, 2000);
  });
}
</script>
