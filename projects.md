---
layout: page
title: Projects
permalink: /projects/
---

<style>
/* 整体背景色 */
body {
  background-color: #f0f5fa;
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

/* 研究标签样式 */
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

/* 项目条目样式（采用类似论文卡片的样式） */
.project-item {
  background: #fff;
  border-radius: 16px;
  margin-bottom: 25px;
  padding: 20px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.05);
  transition: all 0.3s ease;
}

.project-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.1);
}

/* 项目标签样式 */
.project-tag {
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

.tag-opensource {
  background: linear-gradient(135deg, rgba(33,150,243,0.1), rgba(33,150,243,0.2));
  color: #2196F3;
  border: 1px solid rgba(33,150,243,0.3);
}

.tag-github {
  background: linear-gradient(135deg, rgba(76,175,80,0.1), rgba(76,175,80,0.2));
  color: #4CAF50;
  border: 1px solid rgba(76,175,80,0.3);
}

.tag-video {
  background: linear-gradient(135deg, rgba(255,152,0,0.1), rgba(255,152,0,0.2));
  color: #FF9800;
  border: 1px solid rgba(255,152,0,0.3);
}

/* 项目链接样式 */
.project-links {
  margin-top: 15px;
}

.project-link {
  display: inline-block;
  padding: 6px 12px;
  border-radius: 6px;
  text-decoration: none;
  margin: 0 8px 8px 0;
  transition: all 0.3s ease;
  font-size: 0.85em;
  border: 1px solid;
}

.link-github {
  color: #4CAF50;
  background: rgba(76,175,80,0.1);
  border-color: rgba(76,175,80,0.2);
}

.link-video {
  color: #FF9800;
  background: rgba(255,152,0,0.1);
  border-color: rgba(255,152,0,0.2);
}

.project-link:hover {
  transform: translateY(-1px);
}

.link-github:hover {
  background: rgba(76,175,80,0.2);
  border-color: rgba(76,175,80,0.4);
}

.link-video:hover {
  background: rgba(255,152,0,0.2);
  border-color: rgba(255,152,0,0.4);
}
</style>

<!-- 摘要部分 -->
<div class="summary-section">
  <h1>Projects</h1>
  <p>
    Explore my research projects and open-source contributions spanning robotics, computer vision, and creative multimedia applications.
  </p>
  <div class="research-tags-container">
    <span class="research-tag tag-tech">Robotics</span>
    <span class="research-tag tag-tech">Computer Vision</span>
    <span class="research-tag tag-focus">Multimedia</span>
  </div>
</div>

<!-- Research Projects -->
<h2>Research Projects</h2>

<div class="project-item">
  <h3>Gait Face Fusion Recognition System Based on Multi Perspective Collaboration</h3>
  <p><em>Duration: 2023.9 – 2024.5</em></p>
  <p>
    A national-level project developing a multi-person gait recognition system with a visual interface that integrates facial and gait features.
    I led the design and implementation of an occlusion gait restoration module to significantly improve recognition accuracy.
  </p>
</div>

<div class="project-item">
  <h3>Auto-Focus-Assistant</h3>
  <p><em>Duration: 2022.11 – 2023.6</em></p>
  <p>
    An independent R&D project leveraging depth cameras and advanced computer vision techniques to deliver an efficient auto-focus system.
    The system processes spatial depth and RGB data using YolofastestV2 for object detection, supporting multiple focusing modes including manual, automatic, and continuous tracking.
  </p>
  <div class="project-links">
    <span class="project-tag tag-github">📦 GitHub</span>
    <a href="https://github.com/alexlai2860/Auto-focus-assistant" class="project-link link-github" target="_blank">[GitHub Repository]</a>
    <span class="project-tag tag-video">🎥 Demo</span>
    <a href="https://www.bilibili.com/video/BV1Yh4y147x5/" class="project-link link-video" target="_blank">[Demo Video]</a>
  </div>
</div>

<div class="project-item">
  <h3>Original Aspiration: RoboMaster Short Film Project</h3>
  <p><em>Duration: 2022.9 – 2023.1</em></p>
  <p>
    A team-driven filmmaking project in which I served as the team leader.
    I managed screenplay, directing, cinematography, and post-production editing.
    The project documented the preparation for a robotics competition and received positive feedback.
  </p>
  <div class="project-links">
    <span class="project-tag tag-video">🎬 Short Film</span>
    <a href="https://www.bilibili.com/video/BV1MM411t7SY/" class="project-link link-video" target="_blank">[Watch Film]</a>
  </div>
</div>

<div class="project-item">
  <h3>National College Student Robot Competition (RoboMaster University Championship)</h3>
  <p><em>Duration: 2021.9 – 2022.7</em></p>
  <p>
    A robotics competition where I participated as a UAV team member.
    My responsibilities included designing and developing the UAV target detection system, debugging during flight tests, and maintaining the robot vision library.
  </p>
</div>