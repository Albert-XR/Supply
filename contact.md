---
layout: page
title: Contact Us
permalink: /contact/
---

&lt;style&gt;
.contact-page h1 { text-align: center; margin-bottom: 10px; }
.contact-intro { text-align: center; color: #666; margin-bottom: 40px; }

/* 联系信息卡片 */
.contact-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
  margin-bottom: 50px;
}

/* 左侧：联系信息 */
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

/* 右侧：询盘引导 */
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
  transition: opacity 0.2s;
}
.whatsapp-btn:hover { opacity: 0.9; }

/* 询盘模板 */
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
.copy-btn:hover { opacity: 0.9; }

/* 响应式 */
@media (max-width: 768px) {
  .contact-grid { grid-template-columns: 1fr; }
}

/* 页脚CTA */
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
&lt;/style&gt;

&lt;div class="contact-page"&gt;
  &lt;h1&gt;Contact Us&lt;/h1&gt;
  &lt;p class="contact-intro"&gt;Get in touch for quotes, samples, or factory visits. We reply within 24 hours.&lt;/p&gt;

  &lt;div class="contact-grid"&gt;
    &lt;!-- 左侧联系信息 --&gt;
    &lt;div class="contact-info"&gt;
      &lt;h2&gt;Get In Touch&lt;/h2&gt;
      
      &lt;div class="info-item"&gt;
        &lt;div class="info-icon"&gt;📧&lt;/div&gt;
        &lt;div class="info-content"&gt;
          &lt;h4&gt;Email&lt;/h4&gt;
          &lt;p&gt;&lt;a href="mailto:sales@ding-yong.com"&gt;sales@ding-yong.com&lt;/a&gt;&lt;/p&gt;
          &lt;p style="font-size: 0.85em; color: #888; margin-top: 5px;"&gt;For quotes & general inquiries&lt;/p&gt;
        &lt;/div&gt;
      &lt;/div&gt;

      &lt;div class="info-item"&gt;
        &lt;div class="info-icon"&gt;📱&lt;/div&gt;
        &lt;div class="info-content"&gt;
          &lt;h4&gt;WhatsApp / WeChat&lt;/h4&gt;
          &lt;p&gt;&lt;a href="https://wa.me/8613822066349" target="_blank"&gt;+86 138-2206-6349&lt;/a&gt;&lt;/p&gt;
          &lt;p style="font-size: 0.85em; color: #888; margin-top: 5px;"&gt;Fastest response for urgent matters&lt;/p&gt;
        &lt;/div&gt;
      &lt;/div&gt;

      &lt;div class="info-item"&gt;
        &lt;div class="info-icon"&gt;🏭&lt;/div&gt;
        &lt;div class="info-content"&gt;
          &lt;h4&gt;Factory Address&lt;/h4&gt;
          &lt;p&gt;Ding-Yong Industrial Park, No. 168 Yongxing Road&lt;/p&gt;
          &lt;p&gt;Chaozhou City, Guangdong Province, China 521000&lt;/p&gt;
        &lt;/div&gt;
      &lt;/div&gt;

      &lt;div class="info-item"&gt;
        &lt;div class="info-icon"&gt;🕐&lt;/div&gt;
        &lt;div class="info-content"&gt;
          &lt;h4&gt;Working Hours&lt;/h4&gt;
          &lt;p&gt;Monday - Saturday: 8:30 AM - 6:00 PM (GMT+8)&lt;/p&gt;
          &lt;p&gt;Sunday: Closed&lt;/p&gt;
        &lt;/div&gt;
      &lt;/div&gt;
    &lt;/div&gt;

    &lt;!-- 右侧：询盘引导 --&gt;
    &lt;div class="inquiry-guide"&gt;
      &lt;h2&gt;How to Inquire&lt;/h2&gt;
      
      &lt;div class="tip-box"&gt;
        &lt;p&gt;&lt;strong&gt;💡 Recommended:&lt;/strong&gt; For fastest response, include:&lt;/p&gt;
        &lt;ul&gt;
          &lt;li&gt;Product name or photo&lt;/li&gt;
          &lt;li&gt;Target quantity&lt;/li&gt;
          &lt;li&gt;Destination country&lt;/li&gt;
          &lt;li&gt;Any custom requirements (logo, packaging, etc.)&lt;/li&gt;
        &lt;/ul&gt;
      &lt;/div&gt;

      &lt;div class="contact-method"&gt;
        &lt;div class="method-icon"&gt;📧&lt;/div&gt;
        &lt;h4&gt;Email Us&lt;/h4&gt;
        &lt;a href="mailto:sales@ding-yong.com"&gt;sales@ding-yong.com&lt;/a&gt;
        &lt;p&gt;Reply within 24 hours&lt;/p&gt;
      &lt;/div&gt;

      &lt;div class="contact-method"&gt;
        &lt;div class="method-icon"&gt;💬&lt;/div&gt;
        &lt;h4&gt;WhatsApp&lt;/h4&gt;
        &lt;a href="https://wa.me/8613822066349" target="_blank"&gt;+86 138-2206-6349&lt;/a&gt;
        &lt;p&gt;Fastest response&lt;/p&gt;
      &lt;/div&gt;

      &lt;a href="https://wa.me/8613822066349" target="_blank" class="whatsapp-btn"&gt;
        💬 Chat on WhatsApp Now
      &lt;/a&gt;

      &lt;!-- 询盘模板 --&gt;
      &lt;div class="inquiry-template"&gt;
        &lt;h4&gt;📋 Copy-Paste Inquiry Template&lt;/h4&gt;
        &lt;pre id="templateText"&gt;Dear Sales Team,

I am interested in your stainless steel tableware products. Please find my inquiry details below:

Product Interest: [e.g., 24pc Cutlery Set / Dinner Fork / Custom OEM]
Quantity: [e.g., 3,000 sets]
Destination Country: [e.g., USA / Germany / Japan]
Target Price: [optional]

Requirements:
- Material: [18/10 or 18/0]
- Finish: [Mirror Polish / Satin / Gold Plated]
- Packaging: [Color Box / Blister / Custom]
- Logo: [Laser Engraving / None]
- Delivery: [FOB / CIF / DDP]

Please send your best quotation and catalog.

Best regards,
[Your Name]
[Your Company]
[Your WhatsApp/Email]&lt;/pre&gt;
        &lt;button class="copy-btn" onclick="copyTemplate()"&gt;📋 Copy Template&lt;/button&gt;
      &lt;/div&gt;
    &lt;/div&gt;
  &lt;/div&gt;

  &lt;!-- 底部CTA --&gt;
  &lt;div class="cta-bottom"&gt;
    &lt;h3&gt;Prefer to Visit Our Factory?&lt;/h3&gt;
    &lt;p&gt;We welcome factory audits and video inspections. Schedule a visit today.&lt;/p&gt;
    &lt;a href="mailto:sales@ding-yong.com?subject=Factory Visit Request" class="cta-button"&gt;Schedule Factory Visit&lt;/a&gt;
    &lt;a href="https://wa.me/8613822066349" class="cta-button secondary" target="_blank"&gt;Video Call on WhatsApp&lt;/a&gt;
  &lt;/div&gt;
&lt;/div&gt;

&lt;script&gt;
function copyTemplate() {
  var text = document.getElementById('templateText').innerText;
  navigator.clipboard.writeText(text).then(function() {
    var btn = document.querySelector('.copy-btn');
    btn.textContent = '✅ Copied!';
    setTimeout(function() {
      btn.textContent = '📋 Copy Template';
    }, 2000);
  });
}
&lt;/script&gt;
