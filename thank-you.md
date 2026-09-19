---
layout: page
title: Thank You
permalink: /thank-you/
sitemap: false
---

<style>
.thanks-box { text-align: center; padding: 60px 20px; max-width: 640px; margin: 0 auto; }
.thanks-icon { font-size: 4em; margin-bottom: 10px; }
.thanks-box h1 { color: #1a1a2e; margin-bottom: 10px; }
.thanks-box p { color: #555; font-size: 1.05em; line-height: 1.7; }
.thanks-actions { margin-top: 30px; display: flex; gap: 14px; justify-content: center; flex-wrap: wrap; }
.thanks-btn { display: inline-block; padding: 13px 28px; border-radius: 6px; text-decoration: none; font-weight: bold; }
.thanks-btn.primary { background: #e94560; color: #fff; }
.thanks-btn.whatsapp { background: #25D366; color: #fff; }
</style>

<div class="thanks-box">
  <div class="thanks-icon">&#9989;</div>
  <h1>Thank You!</h1>
  <p>Your inquiry has been received. Our sales team will reply within <strong>24 hours</strong> (Mon&ndash;Sat).</p>
  <p>For urgent matters, reach us directly on WhatsApp.</p>
  <div class="thanks-actions">
    <a class="thanks-btn whatsapp" href="https://wa.me/8615013371880" target="_blank">&#128172; Chat on WhatsApp</a>
    <a class="thanks-btn primary" href="/products/">Continue Browsing Products</a>
  </div>
</div>

{% if site.google_analytics_key and site.google_analytics_key != "" %}
<script>
  if (typeof gtag === 'function') {
    gtag('event', 'inquiry_submitted', {
      'event_category': 'engagement',
      'event_label': document.referrer || 'direct'
    });
  }
</script>
{% endif %}
