---
layout: page
title: Contact Us
permalink: /contact/
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
</style>

<div class="contact-page">
<h1>Contact Us</h1>
<p class="contact-intro">Get in touch for quotes, samples, or factory visits. We reply within 24 hours.</p>

<div class="contact-grid">

<div class="contact-info">
<h2>Get In Touch</h2>

<div class="info-item">
<div class="info-icon">&#9993;</div>
<div class="info-content">
<h4>Email</h4>
<p><a href="mailto:sales@ding-yong.com">sales@ding-yong.com</a></p>
<p style="font-size: 0.85em; color: #888; margin-top: 5px;">For quotes & general inquiries</p>
</div>
</div>

<div class="info-item">
<div class="info-icon">&#128241;</div>
<div class="info-content">
<h4>WhatsApp / WeChat</h4>
<p><a href="https://wa.me/8613822066349" target="_blank">+86 138-2206-6349</a></p>
<p style="font-size: 0.85em; color: #888; margin-top: 5px;">Fastest response for urgent matters</p>
</div>
</div>

<div class="info-item">
<div class="info-icon">&#127981;</div>
<div class="info-content">
<h4>Factory Address</h4>
<p>No. 2, 1st Floor, Maifeng Commercial Building, Chating Road, Xixi Village, Xichang Town, Jiedong District, Jieyang City, Guangdong Province, China</p>
</div>
</div>

<div class="info-item">
<div class="info-icon">&#128336;</div>
<div class="info-content">
<h4>Working Hours</h4>
<p>Monday - Saturday: 8:30 AM - 6:00 PM (GMT+8)</p>
<p>Sunday: Closed</p>
</div>
</div>

</div>

<div class="inquiry-guide">
<h2>How to Inquire</h2>

<div class="contact-form">
<h3>&#128221; Send Us an Inquiry</h3>
<form action="https://api.web3forms.com/submit" method="POST">
  <input type="hidden" name="access_key" value="{{ site.web3forms_access_key }}">
  <input type="hidden" name="subject" value="New Website Inquiry from Contact Page">
  <input type="hidden" name="redirect" id="form-redirect" value="">
  <script>document.getElementById('form-redirect').value = window.location.origin + '/thank-you/';</script>
  <input type="checkbox" name="botcheck" class="hidden" style="display:none;" tabindex="-1" autocomplete="off">
  <div class="cform-row">
    <input type="text" name="name" placeholder="Your Name *" required>
    <input type="email" name="email" placeholder="Email Address *" required>
  </div>
  <div class="cform-row">
    <input type="text" name="company" placeholder="Company (optional)">
    <input type="text" name="country" placeholder="Country / Region">
  </div>
  <div class="cform-row">
    <select name="quantity" required>
      <option value="">Target Quantity *</option>
      <option value="Samples first">Samples first</option>
      <option value="Under 1,000 pcs">Under 1,000 pcs</option>
      <option value="1,000 - 5,000 pcs">1,000 - 5,000 pcs</option>
      <option value="5,000 - 10,000 pcs">5,000 - 10,000 pcs</option>
      <option value="10,000+ pcs">10,000+ pcs</option>
    </select>
  </div>
  <textarea name="message" rows="4" placeholder="Tell us about your needs (product, material, finish, packaging, logo...)"></textarea>
  <button type="submit" class="submit-btn">Submit Inquiry</button>
</form>
</div>

<div class="tip-box">
<p><strong>&#128161; Recommended:</strong> For fastest response, include:</p>
<ul>
<li>Product name or photo</li>
<li>Target quantity</li>
<li>Destination country</li>
<li>Any custom requirements (logo, packaging, etc.)</li>
</ul>
</div>

<div class="contact-method">
<div class="method-icon">&#9993;</div>
<h4>Email Us</h4>
<p><a href="mailto:sales@ding-yong.com">sales@ding-yong.com</a></p>
<p>Reply within 24 hours</p>
</div>

<div class="contact-method">
<div class="method-icon">&#128172;</div>
<h4>WhatsApp</h4>
<p><a href="https://wa.me/8613822066349" target="_blank">+86 138-2206-6349</a></p>
<p>Fastest response</p>
</div>

<a href="https://wa.me/8613822066349" target="_blank" class="whatsapp-btn">&#128172; Chat on WhatsApp Now</a>

<div class="inquiry-template">
<h4>&#128203; Copy-Paste Inquiry Template</h4>
<pre id="templateText">Dear Sales Team,

I am interested in your stainless steel tableware products. Please find my inquiry details below:

Product Interest: [e.g., 410 Stainless Steel Knife Fork Spoon Set / Diamond Bottle Tableware Set / Custom OEM]
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
[Your WhatsApp/Email]</pre>
<button class="copy-btn" onclick="copyTemplate()">&#128203; Copy Template</button>
</div>

</div>

</div>

</div>

<script>
function copyTemplate() {
  var text = document.getElementById('templateText').innerText;
  navigator.clipboard.writeText(text).then(function() {
    var btn = document.querySelector('.copy-btn');
    btn.textContent = '&#10004; Copied!';
    setTimeout(function() {
      btn.textContent = '&#128203; Copy Template';
    }, 2000);
  });
}
</script>
