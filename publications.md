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
}

.custom-link—code {
  color: #4CAF50;
  background: rgba(76,175,80,0.1);
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

.image-wrapper {
  text-align: center;
  padding: 5px;
}
.image-wrapper img {
  width: 100%;
  max-width: 100%;
  border-radius: 12px;
}
</style>

<!-- 摘要部分 -->
<div class="summary-section">
  <h1>Publications</h1>
  My research focuses on AI-generated content (AIGC) and advanced image restoration techniques.
  <br><br>
  I strive to develop robust solutions for real-world adverse conditions by leveraging multimodal large language models and innovative feedback optimization methods.
  
  <div class="research-tags-container">
    <span class="research-tag tag-tech">MLLM</span>
    <span class="research-tag tag-tech">Image Restoration</span>
    <span class="research-tag tag-focus">Real-world Applications</span>
  </div>

  <div class="summary-stats">
    <div class="stat-item">
      <div class="stat-number">1</div>
      <div class="stat-label">CVPR/Conferences</div>
      <div class="stat-tooltip">
        <strong>Publication:</strong><br>
        • CVPR'25 SnowMaster Paper
      </div>
    </div>
  </div>
</div>

<!-- Selected Papers -->
<h1>Selected Papers</h1>

<!-- 符号说明 -->
<div class="symbols-legend" style="margin: 15px 0; font-size: 1em; color: #555;">
  <span style="margin-right: 20px;"><strong>*</strong> - Equal Contribution</span>
  <span style="margin-right: 20px;"><strong><sup>&#9828;</sup></strong> - Project Lead</span>
  <span><strong><sup>✉️</sup></strong> - Corresponding Author</span>
</div>

<!-- 2025年论文 -->
<div class="year-section">
  <div class="year-divider">
    <h2 class="year-2025">2025</h2>
  </div>
  <table style="width:100%; border:0; border-collapse: separate; margin: auto;">
    <tbody>
      <!-- PosterCraft -->
      <tr>
        <td style="width:35%;" class="image-wrapper" data-description="arXiv'25">
            <a href="https://ephemeral182.github.io/images/postercraft/pub/fig1.png" target="_blank" title="Click to view full image">
                <img src="https://ephemeral182.github.io/images/postercraft/pub/fig1.png" alt="PosterCraft">
            </a>
        </td>
        <td style="width:65%;" valign="middle" class="text-wrapper">
          <papertitle>
            <strong>
              🔥🔥🔥 PosterCraft: Rethinking High-Quality Aesthetic Poster Generation in a Unified Framework
            </strong>
          </papertitle>
          <br>
          <div>
            <span class="paper-tag tag-method">Unified Framework</span>
            <span class="paper-tag tag-application">Aesthetic Poster Generation</span>
          </div>
          Sixiang Chen*, <strong><u>Jianyu Lai*</u></strong>, Jialin Gao*, Tian Ye, Haoyu Chen, Hengyu Shi, Shitong Shao, Yunlong Lin, Song Fei, Zhaohu Xing, Yeying Jin, Junfeng Luo, Xiaoming Wei, Lei Zhu<sup>✉️</sup>.
          <br>
          <em>arXiv</em>, 2025
          <br>
          <a href="https://arxiv.org/abs/2506.10741" class="custom-link—paper">[Paper]</a>
          <a href="https://github.com/Ephemeral182/PosterCraft" class="custom-link—code">[GitHub]</a>
          <a href="https://ephemeral182.github.io/PosterCraft/" class="custom-link—project">[Project Website]</a>
        </td>
      </tr>
      <!-- GenHaze -->
      <tr>
        <td style="width:35%;" class="image-wrapper" data-description="ICCV'25">
            <a href="https://ephemeral182.github.io/images/genhaze/teaser2.png" target="_blank" title="Click to view full image">
                <img src="https://ephemeral182.github.io/images/genhaze/teaser2.png" alt="GenHaze">
            </a>
        </td>
        <td style="width:65%;" valign="middle" class="text-wrapper">
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
          Sixiang Chen*, Tian Ye, Yunlong Lin, Yeying Jin, Yijun Yang, Haoyu Chen, <strong><u>Jianyu Lai</u></strong>, Song Fei, Zhaohu Xing, Fugee Tsung, Lei Zhu<sup>✉️</sup>.
          <br>
          <em>International Conference on Computer Vision (ICCV)</em>, 2025
          <br>
          <a href="Ephemeral182.github.io" class="custom-link—paper">[Paper]</a>
          <a href="Ephemeral182.github.io" class="custom-link—code">[Code]</a>
        </td>
      </tr>
      <!-- SnowMaster -->
      <tr>
        <td style="width:35%;" class="image-wrapper" data-description="CVPR'25">
          <img src="https://alexlai2860.github.io/images/snowmaster/overview_cvpr2025_snowmaster.png" alt="SnowMaster">
        </td>
        <td style="width:65%;" valign="middle" class="text-wrapper">
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
          <strong><u>Jianyu Lai*</u></strong>, Sixiang Chen*, Yunlong Lin, Tian Ye, Yun Liu, Song Fei, Zhaohu Xing, Hongtao Wu, Weiming Wang, Lei Zhu<sup>✉️</sup>.
          <br>
          <em>Computer Vision and Pattern Recognition (CVPR)</em>, 2025
          <br>
          <a href="https://alexlai2860.github.io" class="custom-link—paper">[Paper]</a>
          <a href="https://alexlai2860.github.io" class="custom-link—code">[Code]</a>
        </td>
      </tr>
    </tbody>
  </table>
</div>

---