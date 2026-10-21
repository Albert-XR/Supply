---
layout: page
title: Meet Us at Jinhan Fair 2026 — Booth 7B01
permalink: /jinhan-fair-2026/
description: "DINGYONG is exhibiting at the 54th Jinhan Fair for Home & Gifts — October 21–27, 2026, PWTC Expo, Guangzhou, Booth No. 7B01. Visit our booth to see our latest stainless steel cutlery and discuss OEM/ODM programmes."
image: /assets/images/exhibition/jinhan-fair-2026-og.jpg
---

<style>
.exhibition-page { max-width: 720px; margin: 0 auto; text-align: center; }

.exhibition-page h1 { margin: 0 0 16px; }

.ex-kicker {
  display: inline-block;
  background: #c8102e;
  color: #fff;
  font-size: 0.76em;
  font-weight: bold;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  padding: 7px 18px;
  border-radius: 20px;
  margin-bottom: 20px;
}

.ex-lede {
  font-size: 1.02em;
  line-height: 1.75;
  color: #555;
  text-align: left;
  max-width: 640px;
  margin: 0 auto 34px;
}
.ex-lede strong { color: #1a1a2e; }

.ex-invitation { margin: 0 auto 14px; max-width: 560px; }

.ex-invitation a {
  display: block;
  border: 1px solid #e4e4e4;
  border-radius: 10px;
  overflow: hidden;
  line-height: 0;
  box-shadow: 0 6px 22px rgba(0, 0, 0, 0.09);
  transition: box-shadow 0.3s, transform 0.3s;
}
.ex-invitation a:hover {
  box-shadow: 0 12px 32px rgba(0, 0, 0, 0.16);
  transform: translateY(-3px);
}
.ex-invitation img { width: 100%; height: auto; display: block; }

.ex-download {
  font-size: 0.9em;
  color: #777;
  margin: 0 0 36px;
}
.ex-download a { color: #c8102e; font-weight: bold; text-decoration: none; }
.ex-download a:hover { text-decoration: underline; }

.ex-meet {
  border-top: 1px solid #ececec;
  padding-top: 26px;
  font-size: 0.97em;
  line-height: 1.75;
  color: #555;
}
.ex-meet a { color: #c8102e; font-weight: bold; text-decoration: none; }
.ex-meet a:hover { text-decoration: underline; }

/* 现场实拍：一条视频 + 一组图片 */
.ex-gallery {
  border-top: 1px solid #ececec;
  padding-top: 28px;
  margin-top: 38px;
}
.ex-gallery h2 {
  font-size: 1.2em;
  margin: 0 0 8px;
  color: #1a1a2e;
}
.ex-gallery-note {
  font-size: 0.93em;
  line-height: 1.7;
  color: #777;
  max-width: 560px;
  margin: 0 auto 24px;
}
.ex-video { margin: 0; flex: 0 0 auto; }
.ex-video video {
  display: block;
  width: auto;
  height: auto;
  max-width: 100%;
  max-height: 460px;
  margin: 0 auto;
  border-radius: 10px;
  background: #000;
  box-shadow: 0 6px 22px rgba(0, 0, 0, 0.12);
}

.ex-live {
  display: flex;
  gap: 26px;
  align-items: flex-start;
  text-align: left;
  margin: 0 0 32px;
}
.ex-live-text { flex: 1 1 auto; min-width: 0; }
.ex-live-text h3 {
  font-size: 1.02em;
  margin: 0 0 12px;
  color: #1a1a2e;
}
.ex-live-text ul {
  list-style: none;
  padding: 0;
  margin: 0 0 14px;
  font-size: 0.92em;
  line-height: 1.65;
  color: #555;
}
.ex-live-text li {
  position: relative;
  padding-left: 20px;
  margin-bottom: 10px;
}
.ex-live-text li::before {
  content: "✓";
  position: absolute;
  left: 0;
  top: 0;
  color: #c8102e;
  font-weight: bold;
}
.ex-live-close {
  font-size: 0.88em;
  line-height: 1.65;
  color: #888;
  margin: 0;
}
.ex-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 14px;
}
.ex-grid figure { margin: 0; }
.ex-grid img {
  display: block;
  width: 100%;
  height: auto;
  border-radius: 8px;
}
.ex-grid .ex-wide { grid-column: 1 / -1; }
.ex-video figcaption,
.ex-grid figcaption {
  font-size: 0.84em;
  line-height: 1.6;
  color: #888;
  margin-top: 9px;
}
@media (max-width: 520px) {
  .ex-live { flex-direction: column; align-items: center; gap: 18px; }
  .ex-live .ex-video video { max-height: 400px; }
  .ex-live-text ul { font-size: 0.9em; }
}

/* 灯箱：点击邀请函后在页内放大，点任意处 / × / Esc 关闭 */
.ex-lightbox {
  position: fixed;
  top: 0; left: 0; right: 0; bottom: 0;
  background: rgba(0, 0, 0, 0.92);
  z-index: 10000;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 26px 16px 40px;
  overflow-y: auto;
  -webkit-overflow-scrolling: touch;
  cursor: zoom-out;
}
.ex-lightbox[hidden] { display: none; }
.ex-lightbox img {
  width: 100%;
  max-width: 760px;
  height: auto;
  border-radius: 6px;
  cursor: default;
}
.ex-lb-close {
  position: fixed;
  top: 12px;
  right: 14px;
  width: 46px;
  height: 46px;
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
  border-radius: 50%;
  background: #fff;
  color: #1a1a2e;
  font-family: inherit;
  font-size: 1.7em;
  line-height: 1;
  padding: 0 0 4px;
  cursor: pointer;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.35);
}
.ex-lb-close:hover { background: #f0f0f0; }
.ex-lb-hint {
  color: rgba(255, 255, 255, 0.7);
  font-size: 0.85em;
  margin: 16px 0 0;
}
body.ex-lb-open { overflow: hidden; }
</style>

<div class="exhibition-page">

  <span class="ex-kicker">54th Jinhan Fair for Home &amp; Gifts</span>

  <h1>Meet Us at Booth No. 7B01</h1>

  <p class="ex-lede">
    DINGYONG is exhibiting at the 54th Jinhan Fair for Home &amp; Gifts in Guangzhou, from
    <strong>October 21 to 27, 2026</strong>, at <strong>PWTC Expo</strong>. You are warmly invited to
    visit <strong>Booth No. 7B01</strong> — our latest stainless steel cutlery is on display, and our
    team is on hand to go through finishes, packaging and OEM/ODM programmes. Open daily through
    October 27.
  </p>

  <figure class="ex-invitation">
    <a class="ex-zoom" href="/assets/images/exhibition/jinhan-fair-2026-invitation.jpg"
       target="_blank" rel="noopener"
       data-ga-event="invitation_view" data-ga-location="exhibition_page">
      <img src="/assets/images/exhibition/jinhan-fair-2026-invitation.jpg"
           width="1240" height="2100"
           alt="DINGYONG invitation to the 54th Jinhan Fair for Home &amp; Gifts — October 21–27, 2026, PWTC Expo Guangzhou, Booth No. 7B01">
    </a>
  </figure>

  <!-- 灯箱：放大查看，点任意处 / × / Esc 关闭 -->
  <div class="ex-lightbox" id="exLightbox" role="dialog" aria-modal="true" aria-label="Invitation" hidden>
    <button type="button" class="ex-lb-close" aria-label="Close">&times;</button>
    <img src="/assets/images/exhibition/jinhan-fair-2026-invitation.jpg"
         alt="DINGYONG invitation to the 54th Jinhan Fair for Home &amp; Gifts, Booth No. 7B01">
    <p class="ex-lb-hint">Click anywhere or press Esc to close</p>
  </div>

  <p class="ex-download">
    Click the invitation to open it full size, or
    <a href="/assets/images/exhibition/jinhan-fair-2026-invitation.jpg"
       download="DINGYONG-Jinhan-Fair-2026-Invitation.jpg"
       data-ga-event="invitation_download" data-ga-location="exhibition_page">download the JPG</a>
    to save or forward to your team.
  </p>

  <section class="ex-gallery" aria-labelledby="exGalleryTitle">
    <h2 id="exGalleryTitle">From the booth</h2>
    <p class="ex-gallery-note">
      Everything on the shelves is out in the open — no glass between you and the pieces. That is
      deliberate: thickness, weight and finish are the three things a catalogue photo cannot show,
      and the only way to judge them is to pick a piece up.
    </p>

    <div class="ex-live">
      <figure class="ex-video">
        <video controls playsinline preload="none"
               poster="/assets/images/exhibition/jinhan-fair-2026-walkthrough-poster.jpg"
               width="720" height="1280">
          <source src="/assets/videos/jinhan-fair-2026-walkthrough.mp4" type="video/mp4">
          Your browser does not support embedded video.
          <a href="/assets/videos/jinhan-fair-2026-walkthrough.mp4">Download the walkthrough (MP4)</a>.
        </video>
        <figcaption>A short walk past the flatware wall.</figcaption>
      </figure>

      <div class="ex-live-text">
        <h3>What to look at on a sample</h3>
        <ul>
          <li><strong>The back of the bowl</strong> — polish should carry into the curve, not stop at the edge.</li>
          <li><strong>The rim</strong> — rolled and even, so it does not feel sharp on the lip after a year of dishwashing.</li>
          <li><strong>The weight at the handle</strong> — hold it by the tip. If it feels light, the balance is wrong and it will sit on the plate.</li>
          <li><strong>Where the handle meets the bowl</strong> — on plated pieces, this is where the finish shows wear first.</li>
        </ul>
        <p class="ex-live-close">Ten seconds, four checks. None of them show in a photo — which is why we bring the pieces to the fair.</p>
      </div>
    </div>

    <div class="ex-grid">
      <figure class="ex-wide">
        <img src="/assets/images/exhibition/jinhan-fair-2026-booth.jpg"
             width="1024" height="560" loading="lazy"
             alt="The DINGYONG booth at Jinhan Fair 2026 — gold display shelving filled with stainless steel flatware, gift boxes and decorative containers, with two meeting tables in front">
        <figcaption>Booth 7B01, set up the day before the doors opened.</figcaption>
      </figure>

      <figure class="ex-wide">
        <img src="/assets/images/exhibition/jinhan-fair-2026-flatware-wall.jpg"
             width="1024" height="768" loading="lazy"
             alt="Close view of the flatware wall at the DINGYONG booth — rows of stainless steel spoons, forks and knives arranged on gold shelving">
        <figcaption>The flatware wall — every handle pattern we currently run.</figcaption>
      </figure>

      <figure>
        <img src="/assets/images/exhibition/jinhan-fair-2026-spoon-silver.jpg"
             width="800" height="1000" loading="lazy"
             alt="Mirror-polished stainless steel spoon held up against the display shelving at the DINGYONG booth">
        <figcaption>Mirror polish, silver finish.</figcaption>
      </figure>

      <figure>
        <img src="/assets/images/exhibition/jinhan-fair-2026-spoon-gold.jpg"
             width="800" height="1000" loading="lazy"
             alt="Gold PVD-finished stainless steel spoon held up against the display shelving at the DINGYONG booth">
        <figcaption>Same spoon, gold PVD finish.</figcaption>
      </figure>
    </div>
  </section>

  <p class="ex-meet">
    Would you like to fix a time with us in advance? Message us on
    <a href="https://wa.me/8615013371880" target="_blank" rel="noopener">WhatsApp +86 150 1337 1880</a>
    or <a href="/contact/?product=jinhan-fair-2026">send an enquiry</a> — we will be ready for you at the booth.
  </p>

</div>

<script>
// 邀请函灯箱：有 JS 时在页内放大（不再跳转到浏览器图片页），无 JS 时降级为原链接行为
(function () {
  var lb = document.getElementById('exLightbox');
  var trigger = document.querySelector('.ex-zoom');
  if (!lb || !trigger) return;

  function open() {
    lb.hidden = false;
    document.body.classList.add('ex-lb-open');
  }
  function close() {
    lb.hidden = true;
    document.body.classList.remove('ex-lb-open');
  }

  trigger.addEventListener('click', function (e) {
    e.preventDefault();
    open();
  });

  lb.addEventListener('click', function (e) {
    if (e.target.closest('img')) return;   // 点图片本身不关闭
    close();
  });

  document.addEventListener('keydown', function (e) {
    if (e.key === 'Escape' && !lb.hidden) close();
  });
})();

// 现场视频：只记第一次播放，避免拖动进度条重复计数
(function () {
  var v = document.querySelector('.ex-video video');
  if (!v) return;
  v.addEventListener('play', function () {
    if (v.getAttribute('data-tracked')) return;
    v.setAttribute('data-tracked', '1');
    if (typeof gtag === 'function') {
      gtag('event', 'booth_video_play', { link_location: 'exhibition_page' });
    }
  });
})();
</script>
