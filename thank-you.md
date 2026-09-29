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
  // 询盘成功事件（真正有商业价值的转化信号）
  // 国家/数量/来源产品由 contact.md 在提交前写入 sessionStorage（Web3Forms 整页 POST
  // 跳转，URL 带不过来；sessionStorage 在同源跳转链路上保留）。
  if (typeof gtag === 'function') {
    var ctx = {};
    try { ctx = JSON.parse(sessionStorage.getItem('dy_inquiry_ctx') || '{}') || {}; } catch (e) {}
    gtag('event', 'inquiry_submitted', {
      inquiry_country: ctx.country || 'unknown',
      inquiry_quantity: ctx.quantity || 'unknown',
      product_context: ctx.product || '',
      inquiry_referrer: document.referrer || 'direct'
    });
    if (typeof clarity === 'function') clarity('event', 'inquiry_submitted');
    try { sessionStorage.removeItem('dy_inquiry_ctx'); } catch (e) {}
  }
</script>
{% endif %}
