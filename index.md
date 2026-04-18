---
layout: home
title: 毛刚的个人博客
---

<!-- 自定义布局样式 -->
<style>
  /* 全局布局重置 */
  .home-container {
    width: 95%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px 0;
    display: grid;
    /* 调整布局比例：左侧25% + 中间70%，去掉右侧重复菜单 */
    grid-template-columns: 25% 70%;
    gap: 5%;
    font-family: "Microsoft YaHei", sans-serif;
  }

  /* 左侧栏：博客标题+个人介绍 */
  .left-column {
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 20px;
    background: #f9f9f9;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  }
  .blog-title {
    font-size: 18px;
    font-weight: bold;
    color: #333;
    text-align: center;
    padding-bottom: 15px;
    border-bottom: 1px solid #eee;
    margin-bottom: 20px;
  }
  .personal-intro {
    font-size: 15px;
    color: #666;
    line-height: 1.6;
    text-align: center;
  }
  .personal-intro a {
    color: #4299e1;
    text-decoration: none;
  }
  .personal-intro a:hover {
    text-decoration: underline;
  }

  /* 中间栏：图片展示区（占比更大，更美观） */
  .middle-column {
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 20px;
    background: #fff;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 450px;
  }
  .img-container {
    text-align: center;
  }
  .img-container img {
    max-width: 100%;
    max-height: 400px;
    border-radius: 8px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  }
  .img-desc {
    margin-top: 15px;
    color: #777;
    font-size: 14px;
  }

  /* 底部动画栏 */
  .animation-bar {
    width: 95%;
    max-width: 1200px;
    margin: 20px auto 40px;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 20px;
    background: #fff;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    text-align: center;
  }
  /* 可爱的浮动小球动画 */
  .cute-animation {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;
    margin-top: 10px;
  }
  .ball {
    width: 30px;
    height: 30px;
    border-radius: 50%;
    animation: bounce 2s infinite ease-in-out;
  }
  .ball1 { background: #ff9a9e; animation-delay: 0s; }
  .ball2 { background: #fad0c4; animation-delay: 0.3s; }
  .ball3 { background: #f6d365; animation-delay: 0.6s; }
  .ball4 { background: #84fab0; animation-delay: 0.9s; }
  .ball5 { background: #8fd3f4; animation-delay: 1.2s; }
  @keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-20px); }
  }

  /* 移动端适配（布局自动调整） */
  @media (max-width: 768px) {
    .home-container {
      grid-template-columns: 1fr;
      gap: 20px;
    }
  }
</style>

<!-- 修正后的布局：左+中两列，去掉右侧重复菜单 -->
<div class="home-container">
  <!-- 左侧栏：博客标题+个人介绍（保留） -->
  <div class="left-column">
    <div class="blog-title">右边是我！</div>
    <div class="personal-intro">
      这里是我个人的一些介绍<br>
      <a href="/photos/aboutme.md">点击查看完整个人介绍 →</a>
    </div>
  </div>

  <!-- 中间栏：图片展示区（占比更大，更协调） -->
  <div class="middle-column">
    <div class="img-container">
      <!-- 你的图片地址，不用改 -->
      <img src="https://picsum.photos/600/400" alt="我的图片">
      <div class="img-desc">这是我</div>
    </div>
  </div>
</div>

<!-- 底部动画栏（保留可爱动画） -->
<div class="animation-bar">
  这一排显示一些动画
  <div class="cute-animation">
    <div class="ball ball1"></div>
    <div class="ball ball2"></div>
    <div class="ball ball3"></div>
    <div class="ball ball4"></div>
    <div class="ball ball5"></div>
  </div>
</div>