---
layout: archive
title: "My Fishing Adventures"
permalink: /fishes/
author_profile: true
---

{% include base_path %}

<style>
/* 轮播图容器 */
.fish-carousel {
  position: relative;
  max-width: 800px;
  margin: 2em auto;
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 8px 32px rgba(0,0,0,0.1);
  overflow: hidden;
}

/* 轮播图片容器 */
.carousel-container {
  position: relative;
  width: 100%;
  height: 700px;
  overflow: hidden;
}

/* 图片样式 */
.carousel-slide {
  display: none;
  width: 100%;
  height: 100%;
  position: relative;
}

.carousel-slide.active {
  display: block;
}

.carousel-slide img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* 图片描述 */
.slide-caption {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: linear-gradient(transparent, rgba(0,0,0,0.7));
  color: white;
  padding: 20px;
  text-align: center;
}

.slide-caption h3 {
  margin: 0;
  font-size: 1.2em;
  font-weight: bold;
}

.slide-caption p {
  margin: 5px 0 0 0;
  font-size: 0.9em;
  opacity: 0.9;
}

/* 导航按钮 */
.carousel-nav {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(255,255,255,0.8);
  border: none;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  cursor: pointer;
  font-size: 18px;
  color: #333;
  transition: all 0.3s ease;
  z-index: 10;
}

.carousel-nav:hover {
  background: rgba(255,255,255,0.95);
  transform: translateY(-50%) scale(1.1);
}

.carousel-prev {
  left: 15px;
}

.carousel-next {
  right: 15px;
}

/* 指示点 */
.carousel-indicators {
  text-align: center;
  padding: 20px;
  background: #f8f9fa;
}

.indicator {
  display: inline-block;
  width: 12px;
  height: 12px;
  margin: 0 5px;
  border-radius: 50%;
  background: #ccc;
  cursor: pointer;
  transition: all 0.3s ease;
}

.indicator.active {
  background: #007bff;
  transform: scale(1.2);
}

.indicator:hover {
  background: #666;
}

/* 统计信息 */
.fishing-stats {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
  margin: 2em 0;
  text-align: center;
}

.stat-card {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
}

.stat-number {
  font-size: 2em;
  font-weight: bold;
  margin-bottom: 5px;
}

.stat-label {
  font-size: 0.9em;
  opacity: 0.9;
}

/* 响应式 */
@media (max-width: 768px) {
  .fish-carousel {
    margin: 1em;
  }
  
  .carousel-container {
    height: 700px;
  }
  
  .carousel-nav {
    width: 40px;
    height: 40px;
    font-size: 16px;
  }
  
  .slide-caption {
    padding: 15px;
  }
  
  .slide-caption h3 {
    font-size: 1em;
  }
}
</style>

## 🎣 Welcome to My Fishing Gallery


<!-- 钓鱼统计 -->
<!-- <div class="fishing-stats">
  <div class="stat-card">
    <div class="stat-number">23</div>
    <div class="stat-label">Total Fish Caught</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">8</div>
    <div class="stat-label">Different Species</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">15</div>
    <div class="stat-label">Fishing Trips</div>
  </div>
  <div class="stat-card">
    <div class="stat-number">2.3kg</div>
    <div class="stat-label">Biggest Catch</div>
  </div>
</div> -->

<!-- 鱼类轮播图 -->
<div class="fish-carousel">
  <div class="carousel-container">
    <button class="carousel-nav carousel-prev" onclick="changeSlide(-1)">‹</button>
    <button class="carousel-nav carousel-next" onclick="changeSlide(1)">›</button>
    
    <div class="carousel-slide active">
      <img src="/images/fish1.png" alt="Squirrel Fish at Singapore">
      <div class="slide-caption">
        <h3> Squirrel Fish</h3>
        <p>Santosa • May 2025 • 0.4kg</p>
      </div>
    </div>
    
    <div class="carousel-slide">
      <img src="/images/fish2.png" alt="Snapper at Singapore">
      <div class="slide-caption">
        <h3>Snapper</h3>
        <p>Santosa • May 2025 • 0.5kg</p>
      </div>
    </div>
    
    <div class="carousel-slide">
      <img src="/images/fish3.png" alt="Small Fish at Jeju">
      <div class="slide-caption">
        <h3>I don't know him</h3>
        <p>Jeju • October 2024 • 0.2kg</p>
      </div>
    </div>
    
    <div class="carousel-slide">
      <img src="/images/fish8.png" alt="鳜鱼 from local river">
      <div class="slide-caption">
        <h3>Aucha Perch</h3>
        <p>Local River • June 2025 • 0.5kg</p>
      </div>
    </div>
    
    <div class="carousel-slide">
      <img src="/images/fish9.png" alt="Catfish">
      <div class="slide-caption">
        <h3>😸 Catfish</h3>
        <p>Local Pond • July 2025 • 1.7kg</p>
      </div>
    </div>
  </div>
  
  <div class="carousel-indicators">
    <span class="indicator active" onclick="currentSlide(1)"></span>
    <span class="indicator" onclick="currentSlide(2)"></span>
    <span class="indicator" onclick="currentSlide(3)"></span>
    <span class="indicator" onclick="currentSlide(4)"></span>
    <span class="indicator" onclick="currentSlide(5)"></span>
  </div>
</div>

<script>
let slideIndex = 1;
const slides = document.querySelectorAll('.carousel-slide');
const indicators = document.querySelectorAll('.indicator');

function showSlide(n) {
  if (n > slides.length) { slideIndex = 1 }
  if (n < 1) { slideIndex = slides.length }
  
  // 隐藏所有幻灯片
  slides.forEach(slide => slide.classList.remove('active'));
  indicators.forEach(indicator => indicator.classList.remove('active'));
  
  // 显示当前幻灯片
  slides[slideIndex - 1].classList.add('active');
  indicators[slideIndex - 1].classList.add('active');
}

function changeSlide(n) {
  slideIndex += n;
  showSlide(slideIndex);
}

function currentSlide(n) {
  slideIndex = n;
  showSlide(slideIndex);
}

// 自动轮播（可选）
setInterval(() => {
  slideIndex++;
  showSlide(slideIndex);
}, 50000); // 每5秒切换一次
</script>

---

<!-- ## 🎯 Fishing Techniques & Equipment

### Favorite Techniques
- **Fly Fishing** - 适合山溪和河流
- **Spinning** - 万能技法，适合各种环境
- **Trolling** - 深海和大湖作业
- **Bottom Fishing** - 钓大型底栖鱼类

### My Tackle Box
- **Rods:** 7ft Medium Action Spinning Rod, 9ft Fly Rod
- **Reels:** Shimano Stradic CI4+, Orvis Clearwater
- **Lines:** Braided PE Line, Fluorocarbon Leader
- **Baits:** Soft plastics, Spoons, Dry flies

---

## 📍 Favorite Fishing Spots

1. **Lake Michigan** - 最佳Bass钓点
2. **Rocky Mountain Streams** - 野生Trout的天堂
3. **Pacific Coastline** - Salmon季节必去
4. **Local Farm Ponds** - 练手的好地方

---

## 🏆 Personal Records

| Species | Weight | Length | Location | Date |
|---------|--------|--------|----------|------|
| Pacific Salmon | 2.3kg | 65cm | Pacific Coast | May 2024 |
| Large Mouth Bass | 1.8kg | 45cm | Lake Michigan | Mar 2024 |
| Northern Pike | 1.5kg | 52cm | Northern Lake | Jun 2024 |
| Rainbow Trout | 1.2kg | 38cm | Mountain Stream | Apr 2024 | -->

---

*"The charm of fishing is that it is the pursuit of what is elusive but attainable, a perpetual series of occasions for hope." - John Buchan*