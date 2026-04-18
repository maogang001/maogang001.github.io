<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>毛刚的个人博客 | 笔记 & 日志 & 思考</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    :root {
      --bg: #f8f9fa;
      --card: #ffffff;
      --text: #2d3748;
      --subtext: #718096;
      --accent: #4299e1;
      --border: #e2e8f0;
      --hover: #f7fafc;
    }

    body {
      font-family: "Inter", system-ui, -apple-system, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.8;
      padding: 0;
      margin: 0;
    }

    /* 导航栏 */
    nav {
      background: var(--card);
      border-bottom: 1px solid var(--border);
      padding: 16px 0;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav-container {
      max-width: 900px;
      margin: 0 auto;
      padding: 0 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 20px;
      font-weight: 700;
      color: var(--accent);
      text-decoration: none;
    }

    .nav-links a {
      color: var(--subtext);
      text-decoration: none;
      margin-left: 24px;
      font-weight: 500;
      transition: 0.2s;
    }

    .nav-links a:hover {
      color: var(--accent);
    }

    /* 主体内容 */
    .container {
      max-width: 900px;
      margin: 40px auto;
      padding: 0 20px;
    }

    /* 首页头部 */
    .hero {
      text-align: center;
      margin-bottom: 60px;
      padding: 40px 0;
    }

    .hero h1 {
      font-size: 36px;
      margin-bottom: 16px;
      color: var(--text);
    }

    .hero p {
      font-size: 18px;
      color: var(--subtext);
      max-width: 600px;
      margin: 0 auto;
    }

    /* 文章卡片 */
    .post-card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 12px;
      padding: 24px;
      margin-bottom: 20px;
      transition: all 0.2s ease;
    }

    .post-card:hover {
      transform: translateY(-2px);
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
      border-color: var(--accent);
    }

    .post-date {
      color: var(--accent);
      font-size: 14px;
      font-weight: 600;
      margin-bottom: 8px;
    }

    .post-title {
      font-size: 22px;
      font-weight: 600;
      margin-bottom: 12px;
      color: var(--text);
      text-decoration: none;
      display: block;
    }

    .post-title:hover {
      color: var(--accent);
    }

    .post-excerpt {
      color: var(--subtext);
      font-size: 16px;
      margin-bottom: 16px;
    }

    .post-tags {
      display: flex;
      gap: 8px;
      flex-wrap: wrap;
    }

    .post-tag {
      background: rgba(66, 153, 225, 0.1);
      color: var(--accent);
      padding: 4px 12px;
      border-radius: 20px;
      font-size: 12px;
    }

    /* 页脚 */
    footer {
      text-align: center;
      padding: 40px 0;
      color: var(--subtext);
      border-top: 1px solid var(--border);
      margin-top: 80px;
    }

    /* 移动端适配 */
    @media (max-width: 600px) {
      .hero h1 {
        font-size: 28px;
      }
      .post-title {
        font-size: 20px;
      }
      .nav-links a {
        margin-left: 16px;
        font-size: 14px;
      }
    }
  </style>
</head>
<body>
  <!-- 导航栏 -->
  <nav>
    <div class="nav-container">
      <a href="/" class="logo">毛刚的博客</a>
      <div class="nav-links">
        <a href="/">首页</a>
        <a href="#about">关于我</a>
      </div>
    </div>
  </nav>

  <!-- 主体内容 -->
  <div class="container">
    <!-- 首页头部 -->
    <div class="hero">
      <h1>我的笔记与日志</h1>
      <p>记录学习、工作、生活中的所有思考与收获 📝</p>
    </div>

    <!-- 文章列表 -->
    <div class="post-card">
      <div class="post-date">2025-12-29</div>
      <a href="#" class="post-title">我的第一篇博客</a>
      <div class="post-excerpt">
        这是我在 GitHub 上发布的第一篇笔记，以后会在这里记录技术学习、日常思考和生活日志～
      </div>
      <div class="post-tags">
        <span class="post-tag">日常日志</span>
        <span class="post-tag">随笔</span>
      </div>
    </div>

    <div class="post-card">
      <div class="post-date">2025-12-28</div>
      <a href="#" class="post-title">前端学习笔记：Markdown 常用语法</a>
      <div class="post-excerpt">
        整理了写博客常用的 Markdown 语法，包括标题、列表、链接、图片、代码块等，写笔记超方便！
      </div>
      <div class="post-tags">
        <span class="post-tag">技术笔记</span>
        <span class="post-tag">前端</span>
      </div>
    </div>

    <!-- 关于我 -->
    <div id="about" class="post-card" style="margin-top: 40px;">
      <h2 style="margin-bottom: 16px; color: var(--text);">关于我</h2>
      <p style="color: var(--subtext);">
        你好，我是毛刚！<br>
        这里是我的个人博客，专注于记录学习笔记、技术文章和生活思考。<br>
        坚持记录，持续成长～
      </p>
    </div>
  </div>

  <!-- 页脚 -->
  <footer>
    © 2025 毛刚的个人博客 | 搭建于 GitHub Pages
  </footer>
</body>
</html>
