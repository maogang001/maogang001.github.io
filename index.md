---
layout: none
title: 毛刚的个人博客
---

<!-- 全局样式：包含动画、布局、隐藏冗余文字 -->
<style>
  /* 全局重置 */
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Microsoft YaHei", sans-serif;
  }
  body {
    background: #fff;
    padding: 20px;
  }

  /* 🔥 关键：隐藏左上角意外显示的文本（如<!DOCTYPE html>） */
  body > :first-child {
    display: none !important;
  }

  /* 顶部动画栏（恢复小球动画） */
  .top-animation-bar {
    width: 95%;
    max-width: 1200px;
    margin: 0 auto 20px;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 20px;
    background: #fff;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    text-align: center;
  }
  .cute-animation {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;
  }
  .ball {
    width: 30px;
    height: 30px;
    border-radius: 50%;
    animation: bounce 2s infinite ease-in-out;
  }
  /* 小球颜色+延迟（完整保留） */
  .ball1 { background: #ff9a9e; animation-delay: 0s; }
  .ball2 { background: #fad0c4; animation-delay: 0.3s; }
  .ball3 { background: #f6d365; animation-delay: 0.6s; }
  .ball4 { background: #84fab0; animation-delay: 0.9s; }
  .ball5 { background: #8fd3f4; animation-delay: 1.2s; }
  .ball6 { background: #f6d365; animation-delay: 1.5s; }
  .ball7 { background: #84fab0; animation-delay: 1.8s; }
  .ball8 { background: #8fd3f4; animation-delay: 2.1s; }
  .ball9 { background: #f6d365; animation-delay: 2.4s; }
  .ball10 { background: #84fab0; animation-delay: 2.7s; }
  .ball11 { background: #8fd3f4; animation-delay: 3.0s; }
  .ball12 { background: #8fd3f4; animation-delay: 3.3s; }
  .ball13 { background: #f6d365; animation-delay: 3.6s; }
  .ball14 { background: #84fab0; animation-delay: 4.2s; }
  .ball15 { background: #8fd3f4; animation-delay: 4.5s; }
  /* 小球弹跳动画（完整保留） */
  @keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-20px); }
  }

  /* 三列布局容器 */
  .home-container {
    width: 95%;
    max-width: 1200px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 20% 55% 20%;
    gap: 2%;
  }

  /* 左侧栏 */
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
  .nav-item {
    padding: 15px 20px;
    border-bottom: 1px solid #eee;
    text-align: center;
  }
  .nav-item:last-child {
    border-bottom: none;
  }
  .nav-item a {
    font-size: 16px;
    color: #333;
    text-decoration: none;
    transition: all 0.2s;
  }
  .nav-item a:hover {
    color: #4299e1;
    font-weight: bold;
  }
  .visit-count {
    text-align: center;
    margin-top: 20px;
    font-size: 15px;
    color: #666;
  }
  .visit-count span {
    font-size: 20px;
    font-weight: bold;
    color: #4299e1;
  }

  /* 中间栏：图片全屏填充 */
  .middle-column {
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    background: #fff;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    overflow: hidden;
    min-height: 400px;
  }
  .middle-column img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  /* 右侧栏 */
  .right-column {
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    padding: 10px 0;
    background: #f9f9f9;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  }

  /* 页脚 */
  .footer {
    width: 95%;
    max-width: 1200px;
    margin: 20px auto 0;
    padding: 20px 0;
    border-top: 1px solid #eee;
    text-align: center;
    line-height: 2;
    color: #666;
  }
</style>

<!-- 顶部动画栏（恢复小球，完整保留） -->
<div class="top-animation-bar">
  <div class="cute-animation">
    <div class="ball ball1"></div>
    <div class="ball ball2"></div>
    <div class="ball ball3"></div>
    <div class="ball ball4"></div>
    <div class="ball ball5"></div>
    <div class="ball ball6"></div>
    <div class="ball ball7"></div>
    <div class="ball ball8"></div>
    <div class="ball ball9"></div>
    <div class="ball ball10"></div>
    <div class="ball ball11"></div>
    <div class="ball ball12"></div>
    <div class="ball ball13"></div>
    <div class="ball ball14"></div>
    <div class="ball ball15"></div>
  </div>
</div>

<!-- 三列布局 -->
<div class="home-container">
  <!-- 左侧栏 -->
  <div class="left-column">
    <div class="blog-title">基础导航</div>
    <div class="nav-item"><a href="/life">我的生活记录</a></div>
    <div class="nav-item"><a href="/diary">我的日记</a></div>
    <div class="nav-item"><a href="/tech-notes">我的技术笔记</a></div>
    <hr style="margin: 20px 0; border: none; border-top: 1px solid #eee;">
    <div class="blog-title">访问量</div>
    <div class="visit-count">
      访问<br>
      <span>
        <script src="https://busuanzi.ibruce.info/busuanzi/2.3/busuanzi.pure.mini.js"></script>
        <span id="busuanzi_value_site_pv"></span>
      </span><br>次
    </div>
  </div>

  <!-- 中间栏：图片 -->
  <div class="middle-column">
    <img src="./photos/007.jpg" alt="我的图片">
  </div>

  <!-- 右侧栏 -->
  <div class="right-column">
    <div class="blog-title">高级导航</div>
    <div class="nav-item"><a href="/life">我的生活记录</a></div>
    <div class="nav-item"><a href="/diary">我的日记</a></div>
    <div class="nav-item"><a href="/tech-notes">我的技术笔记</a></div>
    <div class="nav-item"><a href="/share">我的日常分享</a></div>
    <div class="nav-item"><a href="/collection">我的收藏</a></div>
    <div class="nav-item"><a href="/aboutme">关于俺</a></div>
  </div>
</div>

<!-- 页脚 -->
<div class="footer">
  知不足而奋进，望远山而行---<br>
  学习的敌人是自己的满足，<br>
  要认真学习一点东西，必须从不自满开始。<br>
  —— 毛泽东
</div>