---
layout: page
permalink: /publications/
title: Publications
---

<style>
/* 整体背景色 */
body {
  background-color: #f0f5fa;  /* 非常淡的蓝色背景 */
}

/* 摘要部分样式 */
.summary-section {
  background: rgba(255, 255, 255, 0.9);
  padding: 30px;
  border-radius: 16px;
  margin-bottom: 40px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.05);
  font-size: 1em;
}

/* 摘要统计部分样式 */
.summary-stats {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin: 20px 0;
}

.stat-item {
  background: #fff;
  padding: 15px 25px;
  border-radius: 12px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
  transition: all 0.3s ease;
}

.stat-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.1);
}

.stat-number {
  font-size: 2.5em;
  font-weight: 700;
  background: linear-gradient(135deg, #2196F3, #00BCD4);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin-bottom: 5px;
}

.stat-label {
  font-size: 0.9em;
  color: #666;
}

/* 论文标签及按钮样式 */
.paper-tag {
  display: inline-flex;
  align-items: center;
  padding: 6px 12px;
  margin: 4px;
  font-size: 0.85em;
  font-weight: 500;
  border-radius: 20px;
  transition: all 0.3s ease;
  cursor: default;
}

.tag-method {
  background: linear-gradient(135deg, rgba(33,150,243,0.1), rgba(33,150,243,0.2));
  color: #2196F3;
  border: 1px solid rgba(33,150,243,0.3);
}

.tag-application {
  background: linear-gradient(135deg, rgba(76,175,80,0.1), rgba(76,175,80,0.2));
  color: #4CAF50;
  border: 1px solid rgba(76,175,80,0.3);
}

.custom-link—paper,
.custom-link—code,
.custom-link—project {
  display: inline-block;
  padding: 5px 10px;
  border-radius: 6px;
  text-decoration: none;
  margin: 0 5px;
  transition: all 0.3s ease;
  font-size: 0.85em;
}

.custom-link—paper {
  color: #2196F3;
  background: rgba(33,150,243,0.1);
  border: 1px solid rgba(33,150,243,0.2);
}

.custom-link—code {
  color: #4CAF50;
  background: rgba(76,175,80,0.1);
  border: 1px solid rgba(76,175,80,0.2);
}

.custom-link—project {
  color: #FF9800;
  background: rgba(255,152,0,0.1);
  border: 1px solid rgba(255,152,0,0.2);
}

.custom-link—paper:hover {
  background: rgba(33,150,243,0.2);
  border: 1px solid rgba(33,150,243,0.4);
  transform: translateY(-1px);
}

.custom-link—code:hover {
  background: rgba(76,175,80,0.2);
  border: 1px solid rgba(76,175,80,0.4);
  transform: translateY(-1px);
}

.custom-link—project:hover {
  background: rgba(255,152,0,0.2);
  border: 1px solid rgba(255,152,0,0.4);
  transform: translateY(-1px);
}

/* 研究标签容器 */
.research-tags-container {
  margin: 25px 0;
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  justify-content: flex-start;
}

.research-tag {
  display: inline-flex;
  align-items: center;
  padding: 8px 16px;
  margin: 5px;
  font-size: 0.9em;
  font-weight: 500;
  border-radius: 25px;
  transition: all 0.4s ease;
  position: relative;
  overflow: hidden;
}

.tag-tech {
  background: linear-gradient(135deg, #00695c10, #00695c20);
  color: #00695c;
  border: 1.5px solid #00695c40;
}

.tag-focus {
  background: linear-gradient(135deg, #bf360c10, #bf360c20);
  color: #bf360c;
  border: 1.5px solid #bf360c40;
}

/* 表格与图片容器样式 */
.year-section { margin: 50px 0; }
.year-divider {
  display: flex;
  align-items: center;
  margin: 40px 0;
}
.year-2025 { color: #4169E1; }

.publication-item {
  display: flex;
  /* 新增：允许子项在空间不足时换行 */
  flex-wrap: wrap;
  align-items: center;
  background-color: #fff;
  margin-bottom: 30px;
  border-radius: 16px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.05);
  transition: all 0.3s ease;
  overflow: hidden;
}

.publication-item:hover {
  transform: translateY(-5px); /* 鼠标悬停时上浮 */
  box-shadow: 0 8px 25px rgba(0,0,0,0.1); /* 增强阴影 */
}

.publication-item .image-wrapper {
  /* 允许在换行时保持35%基准并可收缩 */
  flex: 1 1 35%;
  padding: 20px;
  text-align: center;
}

.publication-item .image-wrapper img {
  width: 100%;
  max-width: 100%;
  border-radius: 12px;
}

.publication-item .text-wrapper {
  /* 允许在换行时保持55%基准并可收缩 */
  flex: 1 1 55%;
  padding: 20px;
  overflow-wrap: break-word;
  min-width: 0;
  /* 强制在单词或长串字符处断行，避免超出容器 */
  word-break: break-word;
}

/* 新增作者和会议信息样式 */
.pub-authors {
  font-size: 0.9em; /* 减小作者列表字体大小 */
  margin-bottom: 5px; /* 增加作者列表下方间距 */
}

.pub-venue {
  font-style: italic;
  margin-top: 5px; /* 增加会议信息上方间距 */
}
</style>

<!-- 摘要部分 -->
<div class="summary-section">
  <h1>Publications</h1>
  My research focuses on low-level vision, AI-generated content (AIGC), and multimodal large language models (MLLM).
  <br><br>
  I aim to develop robust solutions for image restoration in real complex environments, explore AIGC applications for real-world scenarios, and investigate MLLM applications in image processing and evaluation.
  
  <div class="research-tags-container">
    <span class="research-tag tag-tech">Low-level Vision</span>
    <span class="research-tag tag-tech">AIGC</span>
    <span class="research-tag tag-tech">MLLM</span>
  </div>

  <!-- <div class="summary-stats">
    <div class="stat-item">
      <div class="stat-number">1</div>
      <div class="stat-label">CVPR/Conferences</div>
      <div class="stat-tooltip">
        <strong>Publication:</strong><br>
        • CVPR'25 SnowMaster Paper
      </div>
    </div>
  </div> -->
</div>

<!-- Selected Papers -->
<h1>Selected Papers</h1>

<!-- 符号说明 -->
<div class="symbols-legend" style="margin: 15px 0; font-size: 1em; color: #555;">
  <span style="margin-right: 20px;"><strong>*</strong> - Equal Contribution</span>
  <!-- <span style="margin-right: 20px;"><strong><sup>&#9828;</sup></strong> - Project Lead</span> -->
  <span><strong><sup>✉️</sup></strong> - Corresponding Author</span>
</div>

<!-- 2026年论文 -->
<div class="year-section">
  <div class="year-divider">
    <h2 class="year-2025">2026</h2>
  </div>
  
  <!-- PosterReward -->
  <div class="publication-item">
    <div class="image-wrapper" data-description="CVPR'26">
        <a href="https://alexlai2860.github.io/images/posterreward/concat.png" target="_blank" title="Click to view full image">
            <img src="https://alexlai2860.github.io/images/posterreward/concat.png" alt="PosterReward">
        </a>
    </div>
    <div class="text-wrapper">
      <papertitle>
        <strong>
          PosterReward: Unlocking Accurate Evaluation for High-Quality Graphic Design Generation
        </strong>
      </papertitle>
      <br>
      <div>
        <span class="paper-tag tag-method">Reward Model</span>
        <span class="paper-tag tag-application">Graphic Design Evaluation</span>
      </div>
      <div class="pub-authors">
        <strong><u>Jianyu Lai*</u></strong>, Sixiang Chen*, Jialin Gao*, Hengyu Shi, Zhongying Liu, Fuxiang Zhai, Junfeng Luo, Xiaoming Wei, Lujia Wang, Lei Zhu<sup>✉️</sup>.
      </div>
      <div class="pub-venue"><em>Computer Vision and Pattern Recognition (CVPR)</em>, 2026</div>
      <div class="pub-links">
        <a href="/mypaper/posterreward/PosterReward_Arxiv_official.pdf" class="custom-link—paper">[Paper]</a>
        <a href="https://alexlai2860.github.io/PosterReward/" class="custom-link—code">[GitHub]</a>
        <a href="https://alexlai2860.github.io/PosterReward/" class="custom-link—project">[Project Website]</a>
        <a href="https://huggingface.co/PosterReward" class="custom-link—project">[Model]</a>
      </div>
    </div>
  </div>

  <!-- PosterOmni -->
  <div class="publication-item">
    <div class="image-wrapper" data-description="CVPR'26">
        <a href="https://ephemeral182.github.io/images/posteromni/teaser_0209.jpg" target="_blank" title="Click to view full image">
            <img src="https://ephemeral182.github.io/images/posteromni/teaser_0209.jpg" alt="PosterOmni">
        </a>
    </div>
    <div class="text-wrapper">
      <papertitle>
        <strong>
          PosterOmni: Generalized Artistic Poster Creation via Task Distillation and Unified Reward Feedback
        </strong>
      </papertitle>
      <br>
      <div>
        <span class="paper-tag tag-method">Task Distillation</span>
        <span class="paper-tag tag-application">Generalized Poster Creation</span>
      </div>
      <div class="pub-authors">
        Sixiang Chen*, <strong><u>Jianyu Lai*</u></strong>, Jialin Gao*, Hengyu Shi, Zhongying Liu, Tian Ye, Junfeng Luo, Xiaoming Wei, Lei Zhu<sup>✉️</sup>.
      </div>
      <div class="pub-venue"><em>Computer Vision and Pattern Recognition (CVPR)</em>, 2026</div>
      <div class="pub-links">
        <a href="https://arxiv.org/abs/2602.12127" class="custom-link—paper">[Paper]</a>
        <a href="https://github.com/Ephemeral182/PosterOmni" class="custom-link—code">[GitHub]</a>
        <a href="https://huggingface.co/PosterOmni" class="custom-link—project">[Model]</a>
        <a href="https://ephemeral182.github.io/PosterCraft/" class="custom-link—project">[Project Website]</a>
      </div>
    </div>
  </div>

<div class="year-section">
  <div class="year-divider">
    <h2 class="year-2025">2025</h2>
  </div>

  <!-- PosterCraft -->
  <div class="publication-item">
    <div class="image-wrapper" data-description="ICLR'26">
        <a href="https://ephemeral182.github.io/images/postercraft/pub/fig1.png" target="_blank" title="Click to view full image">
            <img src="https://ephemeral182.github.io/images/postercraft/pub/fig1.png" alt="PosterCraft">
        </a>
    </div>
    <div class="text-wrapper">
      <papertitle>
        <strong>
          PosterCraft: Rethinking High-Quality Aesthetic Poster Generation in a Unified Framework
        </strong>
      </papertitle>
      <br>
      <div>
        <span class="paper-tag tag-method">Unified Framework</span>
        <span class="paper-tag tag-application">Aesthetic Poster Generation</span>
      </div>
      <div class="pub-authors">
        Sixiang Chen*, <strong><u>Jianyu Lai*</u></strong>, Jialin Gao*, Tian Ye, Haoyu Chen, Hengyu Shi, Shitong Shao, Yunlong Lin, Song Fei, Zhaohu Xing, Yeying Jin, Junfeng Luo, Xiaoming Wei, Lei Zhu<sup>✉️</sup>.
      </div>
      <div class="pub-venue"><em>International Conference on Learning Representations (ICLR)</em>, 2026</div>
      <div class="pub-links">
        <a href="https://arxiv.org/abs/2506.10741" class="custom-link—paper">[Paper]</a>
        <a href="https://github.com/Ephemeral182/PosterCraft" class="custom-link—code">[GitHub]</a>
        <a href="https://ephemeral182.github.io/PosterCraft/" class="custom-link—project">[Project Website]</a>
      </div>
    </div>
  </div>
</div>

  <!-- GenHaze -->
  <div class="publication-item">
    <div class="image-wrapper" data-description="ICCV'25">
        <a href="https://ephemeral182.github.io/images/genhaze/teaser2.png" target="_blank" title="Click to view full image">
            <img src="https://ephemeral182.github.io/images/genhaze/teaser2.png" alt="GenHaze">
        </a>
    </div>
    <div class="text-wrapper">
      <papertitle>
        <strong>
          GenHaze: Pioneering Controllable One-Step Realistic Haze Generation for Real-World Dehazing
        </strong>
      </papertitle>
      <br>
      <div>
        <span class="paper-tag tag-method">Generative Model for Image Restoration</span>
        <span class="paper-tag tag-application">Real-world Generalization, Plug and Play</span>
      </div>
      <div class="pub-authors">
        Sixiang Chen, Tian Ye, Yunlong Lin, Yeying Jin, Yijun Yang, Haoyu Chen, <strong><u>Jianyu Lai</u></strong>, Song Fei, Zhaohu Xing, Fugee Tsung, Lei Zhu<sup>✉️</sup>.
      </div>
      <div class="pub-venue"><em>International Conference on Computer Vision (ICCV)</em>, 2025</div>
      <div class="pub-links">
        <!-- <a href="Ephemeral182.github.io" class="custom-link—paper">[Paper]</a> -->
        <!-- <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a> -->
      </div>
    </div>
  </div>

  <!-- SnowMaster -->
  <div class="publication-item">
    <div class="image-wrapper" data-description="CVPR'25">
        <a href="https://alexlai2860.github.io/images/snowmaster/overview_cvpr2025_snowmaster.png" target="_blank" title="Click to view full image">
            <img src="https://alexlai2860.github.io/images/snowmaster/overview_cvpr2025_snowmaster.png" alt="SnowMaster">
        </a>
    </div>
    <div class="text-wrapper">
      <papertitle>
        <strong>
          SnowMaster: Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization
        </strong>
      </papertitle>
      <br>
      <div>
        <span class="paper-tag tag-method">MLLM for Image Restoration</span>
        <span class="paper-tag tag-application">Multi-Model Preference Optimization</span>
      </div>
      <div class="pub-authors">
        <strong><u>Jianyu Lai*</u></strong>, Sixiang Chen*, Yunlong Lin, Tian Ye, Yun Liu, Song Fei, Zhaohu Xing, Hongtao Wu, Weiming Wang, Lei Zhu<sup>✉️</sup>.
      </div>
      <div class="pub-venue"><em>Computer Vision and Pattern Recognition (CVPR)</em>, 2025</div>
      <div class="pub-links">
        <a href="https://alexlai2860.github.io" class="custom-link—paper">[Paper]</a>
        <a href="https://alexlai2860.github.io" class="custom-link—code">[Code]</a>
      </div>
    </div>
  </div>
</div>

---