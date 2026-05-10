---
layout: page
title: Contact Us
permalink: /contact/
---

<style>
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

/* 右侧：表单 */
.contact-form {
  background: #f8f9fa;
  padding: 30px;
  border-radius: 12px;
}
.contact-form h2 { margin-bottom: 20px; color: #1a1a2e; }
.form-group { margin-bottom: 20px; }
.form-group label {
  display: block;
  margin-bottom: 8px;
  font-weight: bold;
  color: #333;
  font-size: 0.9em;
}
.form-group input,
.form-group textarea,
.form-group select {
  width: 100%;
  padding: 12px;
  border: 1px solid #ddd;
  border-radius: 6px;
  font-size: 1em;
  font-family: inherit;
}
.form-group input:focus,
.form-group textarea:focus,
.form-group select:focus {
  outline: none;
  border-color: #e94560;
}
.form-group textarea {
  resize: vertical;
  min-height: 120px;
}
.required { color: #e94560; }

.submit-btn {
  width: 100%;
  padding: 14px;
  background: #e94560;
  color: white;
  border: none;
  border-radius: 6px;
  font-size: 1em;
  font-weight: bold;
  cursor: pointer;
  transition: opacity 0.2s;
}
.submit-btn:hover { opacity: 0.9; }

/* 响应式 */
@media (max-width: 768px) {
  .contact-grid { grid-template-columns: 1fr; }
}

/* 成功提示 */
.success-msg {
  display: none;
  background: #d4edda;
  color: #155724;
  padding: 15px;
  border-radius: 6px;
  margin-bottom: 20px;
}
</style>

<div class="contact-page">
  <h1>Contact Us</h1>
  <p class="contact-intro">Get in touch for quotes, samples, or factory visits. We reply within 24 hours.</p>

  <div class="contact-grid">
    <!-- 左侧联系信息 -->
    <div class="contact-info">
      <h2>Get In Touch</h2>
      
      <div class="info-item">
        <div class="info-icon">📧</div>
        <div class="info-content">
          <h4>Email</h4>
          <p><a href="mailto:sales@ding-yong.com">sales@ding-yong.com</a></p>
          <p style="font-size: 0.85em; color: #888; margin-top: 5px;">For quotes & general inquiries</p>
        </div>
      </div>

      <div class="info-item">
        <div class="info-icon">📱</div>
        <div class="info-content">
          <h4>WhatsApp / WeChat</h4>
          <p><a href="https://wa.me/8613822066349" target="_blank">+86 138-2206-6349</a></p>
          <p style="font-size: 0.85em; color: #888; margin-top: 5px;">Fast response for urgent matters</p>
        </div>
      </div>

      <div class="info-item">
        <div class="info-icon">🏭</div>
        <div class="info-content">
          <h4>Factory Address</h4>
          <p>Ding-Yong Industrial Park, No. 168 Yongxing Road</p>
          <p>Chaozhou City, Guangdong Province, China 521000</p>
        </div>
      </div>

      <div class="info-item">
        <div class="info-icon">🕐</div>
        <div class="info-content">
          <h4>Working Hours</h4>
          <p>Monday - Saturday: 8:30 AM - 6:00 PM (GMT+8)</p>
          <p>Sunday: Closed</p>
        </div>
      </div>

      <div style="margin-top: 30px; padding: 20px; background: #fff3cd; border-radius: 10px; border-left: 4px solid #ffc107;">
        <strong>💡 Quick Tip</strong>
        <p style="margin: 5px 0 0 0; font-size: 0.9em; color: #666;">For fastest quote, include: product name, quantity, destination country, and any custom requirements.</p>
      </div>
    </div>

    <!-- 替换整个表单区域 -->

<div class="contact-form">
  <h2>How to Inquire</h2>
  
  <div style="background: #e8f4fd; padding: 20px; border-radius: 10px; margin-bottom: 20px; border-left: 4px solid #2196F3;">
    <p style="margin: 0; font-size: 0.95em;">
      <strong>💡 Recommended:</strong> For fastest response, send inquiry via WhatsApp or email with:
    </p>
    <ul style="margin: 10px 0 0 20px; font-size: 0.9em; color: #555;">
      <li>Product name or photo</li>
      <li>Target quantity</li>
      <li>Destination country</li>
      <li>Any custom requirements</li>
    </ul>
  </div>

  <div style="text-align: center; padding: 30px 20px;">
    <div style="margin-bottom: 25px;">
      <div style="font-size: 2.5em; margin-bottom: 10px;">📧</div>
      <h4 style="margin: 5px 0;">Email Us</h4>
      <a href="mailto:sales@ding-yong.com" style="color: #e94560; font-size: 1.1em; text-decoration: none;">
        sales@ding-yong.com
      </a>
      <p style="font-size: 0.85em; color: #888; margin-top: 5px;">Reply within 24 hours</p>
    </div>

    <div style="margin-bottom: 25px;">
      <div style="font-size: 2.5em; margin-bottom: 10px;">💬</div>
      <h4 style="margin: 5px 0;">WhatsApp</h4>
      <a href="https://wa.me/8613822066349" target="_blank" style="color: #e94560; font-size: 1.1em; text-decoration: none;">
        +86 138-2206-6349
      </a>
      <p style="font-size: 0.85em; color: #888; margin-top: 5px;">Fastest response</p>
    </div>

    <div>
      <div style="font-size: 2.5em; margin-bottom: 10px;">🕐</div>
      <h4 style="margin: 5px 0;">Working Hours</h4>
      <p style="color: #555; font-size: 0.95em;">
        Mon-Sat: 8:30 AM - 6:00 PM (GMT+8)<br>
        <span style="color: #888;">Sunday: Closed</span>
      </p>
    </div>
  </div>

  <a href="https://wa.me/8613822066349" target="_blank" class="submit-btn" style="display: block; text-align: center; text-decoration: none; margin-top: 10px;">
    Chat on WhatsApp Now
  </a>
</div>
  </div>

  <!-- 底部CTA -->
  <div style="background: #1a1a2e; color: white; padding: 40px 30px; text-align: center; border-radius: 12px; margin-top: 40px;">
    <h3 style="margin-bottom: 10px;">Prefer Direct Chat?</h3>
    <p style="opacity: 0.9; margin-bottom: 20px;">Click below to start a WhatsApp conversation with our sales team.</p>
    <a href="https://wa.me/8613822066349" target="_blank" class="cta-button">Chat on WhatsApp</a>
  </div>
</div>

<script>
// 简单的表单提交反馈（实际提交由Formspree处理）
document.getElementById('inquiryForm').addEventListener('submit', function(e) {
  // 如果Formspree配置正确，会自动跳转或显示成功页
  // 这里仅做本地提示
  setTimeout(function() {
    document.getElementById('successMsg').style.display = 'block';
  }, 500);
});
</script>
