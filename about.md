---
layout: page
title: About Us
permalink: /about/
---

<style>
/* About 页面整体布局 */
.about-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 40px 20px;
}

/* 标题区域 */
.about-header {
  text-align: center;
  margin-bottom: 50px;
}

.about-header h1 {
  font-size: 2.2em;
  color: #1a1a2e;
  margin-bottom: 10px;
}

.about-header .subtitle {
  color: #666;
  font-size: 1.1em;
}

/* 主内容区 - 左右布局 */
.about-main {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
  align-items: start;
  margin-bottom: 60px;
}

/* 左侧文字内容 */
.about-content h2 {
  color: #1a1a2e;
  font-size: 1.5em;
  margin-bottom: 20px;
  margin-top: 30px;
}

.about-content h2:first-child {
  margin-top: 0;
}

.about-content p {
  color: #555;
  line-height: 1.8;
  margin-bottom: 15px;
}

/* 右侧视频区域 */
.about-video {
  position: sticky;
  top: 20px;
}

.video-wrapper {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 比例 */
  height: 0;
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 0 8px 30px rgba(0,0,0,0.1);
}

.video-wrapper iframe,
.video-wrapper video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: none;
}

/* 视频封面图（无视频时显示） */
.video-placeholder {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
  padding: 20px;
}

.video-placeholder .play-icon {
  width: 80px;
  height: 80px;
  background: rgba(255,255,255,0.2);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 20px;
  cursor: pointer;
  transition: background 0.3s;
}

.video-placeholder .play-icon:hover {
  background: rgba(255,255,255,0.3);
}

.video-placeholder .play-icon svg {
  width: 30px;
  height: 30px;
  fill: white;
  margin-left: 5px;
}

.video-placeholder h3 {
  font-size: 1.3em;
  margin-bottom: 10px;
}

.video-placeholder p {
  font-size: 0.9em;
  opacity: 0.8;
}

/* 数据统计 */
.stats-section {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 30px;
  margin: 60px 0;
  text-align: center;
}

.stat-item {
  padding: 30px;
  background: #f8f9fa;
  border-radius: 12px;
}

.stat-number {
  font-size: 2.5em;
  font-weight: bold;
  color: #e94560;
  margin-bottom: 8px;
}

.stat-label {
  color: #666;
  font-size: 0.9em;
}

/* 时间线 */
.timeline-section {
  margin: 60px 0;
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

/* 响应式 */
@media (max-width: 768px) {
  .about-main {
    grid-template-columns: 1fr;
  }
  
  .about-video {
    position: relative;
    order: -1;
  }
  
  .stats-section {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 480px) {
  .stats-section {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="about-container">

  <!-- 标题 -->
  <div class="about-header">
    <h1>About Ding-Yong Products</h1>
    <p class="subtitle">Professional Stainless Steel Tableware Manufacturer Since 2010</p>
  </div>

  <!-- 主内容：左文右视频 -->
  <div class="about-main">
    
    <!-- 左侧：公司介绍 -->
    <div class="about-content">
      <h2>Who We Are</h2>
      <p>
        Ding-Yong Products Co., Ltd is a leading manufacturer specializing in premium 
        18/10 stainless steel cutlery, flatware, and kitchen utensils. Based in 
        Guangdong, China, we have been serving global B2B buyers for over 15 years.
      </p>
      <p>
        Our 5,000㎡ production facility houses 200+ skilled workers and advanced 
        CNC polishing machines, enabling us to produce 500,000+ pieces monthly. 
        We are committed to delivering restaurant-quality tableware at competitive 
        factory-direct prices.
      </p>
      <p>
        From small custom orders to large hotel chain contracts, we provide flexible 
        OEM/ODM solutions tailored to your market needs.
      </p>

      <h2>Our Strengths</h2>
      <p>
        ✓ <strong>Factory Direct</strong> — No middlemen, competitive pricing<br>
        ✓ <strong>Quality Assured</strong> — ISO9001, FDA, LFGB, SGS certified<br>
        ✓ <strong>Custom Capacity</strong> — Logo engraving, custom packaging, PVD colors<br>
        ✓ <strong>Fast Delivery</strong> — 35-50 days lead time, flexible MOQ
      </p>
    </div>

    <!-- 右侧：工厂视频 -->
    <div class="about-video">
      <<div class="video-container" style="position: relative; width: 100%; aspect-ratio: 16/9; border-radius: 12px; overflow: hidden;">
        
        <!-- 方案 1：YouTube 嵌入（推荐，替换 VIDEO_ID） -->
        <iframe 
          id="factory-video"
          src="https://www.youtube.com/embed/rxGmVh_LP3A?modestbranding=1&controls=1&showinfo=0&rel=0&iv_load_policy=3" 
          title="Ding-Yong Factory Tour"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
          allowfullscreen
          style="width: 100%; height: 100%; border: none;">
        </iframe>

        <!-- 遮罩层：隐藏标题、logo 等 -->
        <<div class="video-overlay" style="
            position: absolute;
            top: 0; left: 0; right: 0; height: 60px;
            background: linear-gradient(to bottom, rgba(0,0,0,0.8) 0%, transparent 100%);
            z-index: 10;
            pointer-events: none;
        "></div>

        <!-- 自定义播放键（初始显示，点击后隐藏） -->
        <<div id="custom-play" style="
            position: absolute;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            width: 80px; height: 80px;
            background: rgba(220, 38, 38, 0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            z-index: 20;
            transition: opacity 0.3s;
        ">
            <<svg width="32" height="32" viewBox="0 0 24 24" fill="white">
                <polygon points="8,5 8,19 19,12"></polygon>
            </svg>
        </div>
    </div>
    
    <<script>
        document.getElementById('custom-play').addEventListener('click', function() {
            var iframe = document.getElementById('factory-video');
            // 通过 postMessage 触发播放（需要启用 JS API）
            iframe.contentWindow.postMessage('{"event":"command","func":"playVideo","args":""}', '*');
            this.style.opacity = '0';
            this.style.pointerEvents = 'none';
        });
    </script>
      
      <!-- 视频说明 -->
      <div style="margin-top: 15px; text-align: center; color: #666; font-size: 0.85em;">
        <p>🎬 Watch how your tableware is crafted from raw steel to finished products</p>
      </div>
    </div>

  </div>

  <!-- 数据统计 -->
  <div class="stats-section">
    <div class="stat-item">
      <div class="stat-number">15+</div>
      <div class="stat-label">Years Experience</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">5,000㎡</div>
      <div class="stat-label">Factory Area</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">200+</div>
      <div class="stat-label">Workers</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">500K+</div>
      <div class="stat-label">Monthly Output</div>
    </div>
  </div>

  <!-- 发展历程 -->
  <div class="timeline-section">
    <h2>Our Journey</h2>
    <div class="timeline">
      <div class="timeline-item">
        <div class="timeline-year">2010</div>
        <div class="timeline-text">Founded as a small family workshop with 10 workers, focusing on local market stainless steel flatware.</div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2013</div>
        <div class="timeline-text">Expanded to 50 workers, obtained ISO9001 certification, began exporting to Southeast Asia.</div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2016</div>
        <div class="timeline-text">Moved to new 5,000㎡ facility, installed CNC polishing lines, reached 200 workers capacity.</div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2019</div>
        <div class="timeline-text">Achieved FDA and LFGB certifications, entered European and North American markets.</div>
      </div>
      <div class="timeline-item">
        <div class="timeline-year">2024</div>
        <div class="timeline-text">Launched PVD color and custom engraving services, serving 40+ countries worldwide.</div>
      </div>
    </div>
  </div>

</div>
