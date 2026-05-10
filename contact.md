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

    <!-- 右侧表单 -->
    <div class="contact-form">
      <h2>Send Inquiry</h2>
      
      <!-- 使用Formspree（免费，50条/月） -->
      <!-- 注册 https://formspree.io 获取你的form ID，替换下面的action -->
      <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" id="inquiryForm">
        
        <div class="success-msg" id="successMsg">
          ✅ Thank you! Your inquiry has been sent. We'll reply within 24 hours.
        </div>

        <div class="form-group">
          <label>Your Name <span class="required">*</span></label>
          <input type="text" name="name" required placeholder="John Smith">
        </div>

        <div class="form-group">
          <label>Email <span class="required">*</span></label>
          <input type="email" name="email" required placeholder="john@yourcompany.com">
        </div>

        <div class="form-group">
          <label>Company Name</label>
          <input type="text" name="company" placeholder="Your Company Ltd.">
        </div>

        <div class="form-group">
          <label>WhatsApp / Phone</label>
          <input type="tel" name="phone" placeholder="+1 234 567 8900">
        </div>

        <div class="form-group">
          <label>Product Interest <span class="required">*</span></label>
          <select name="product" required>
            <option value="">Select a product category</option>
            <option value="cutlery-sets">Cutlery Sets</option>
            <option value="flatware">Flatware (Forks, Knives, Spoons)</option>
            <option value="serving">Serving Utensils</option>
            <option value="hotel">Hotel & Restaurant Supplies</option>
            <option value="custom">Custom OEM/ODM</option>
          </select>
        </div>

        <div class="form-group">
          <label>Estimated Quantity</label>
          <select name="quantity">
            <option value="">Select quantity range</option>
            <option value="1000-3000">1,000 - 3,000 pcs</option>
            <option value="3000-5000">3,000 - 5,000 pcs</option>
            <option value="5000-10000">5,000 - 10,000 pcs</option>
            <option value="10000+">10,000+ pcs</option>
          </select>
        </div>

        <div class="form-group">
          <label>Destination Country</label>
          <input type="text" name="country" placeholder="e.g., USA, Germany, Japan">
        </div>

        <div class="form-group">
          <label>Message / Requirements <span class="required">*</span></label>
          <textarea name="message" required placeholder="Please describe your needs: product specifications, packaging requirements, target price, delivery timeline, etc."></textarea>
        </div>

        <button type="submit" class="submit-btn">Send Inquiry</button>
      </form>

      <p style="text-align: center; margin-top: 15px; font-size: 0.85em; color: #888;">
        🔒 Your information is secure and will never be shared.
      </p>
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
