---
layout: post1
permalink: /SnowMaster/index.html
title: "SnowMaster: Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization"
---

<h2 class="post-title" style="margin-bottom:7px;margin-top:20px;font-weight:400;">SnowMaster: Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization</h2>

<div class="post-authors" style="margin-bottom:5px;">
  <a href="https://alexlai2860.github.io">Jianyu Lai</a><sup>1,*</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://ephemeral182.github.io">Sixiang Chen</a><sup>1,*</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://lyl1015.github.io/">Yunlong Lin</a><sup>2</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://owen718.github.io">Tian Ye</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  Yun Liu<sup>3</sup>&nbsp;&nbsp;&nbsp;
  Song Fei<sup>1</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://ge-xing.github.io/">Zhaohu Xing</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://hongtao-wu.github.io/">Hongtao Wu</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  Weiming Wang<sup>4</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://sites.google.com/site/indexlzhu/home">Lei Zhu</a><sup>1,5,✉️</sup>
</div>

<div class="post-authors" style="margin-bottom:10px; font-size: 0.9em; color: #666;">
  <sup>1</sup>The Hong Kong University of Science and Technology (Guangzhou)&nbsp;&nbsp;&nbsp;
  <sup>2</sup>Xiamen University&nbsp;&nbsp;&nbsp;
  <sup>3</sup>Southwestern University<br>
  <sup>4</sup>Hong Kong Metropolitan University&nbsp;&nbsp;&nbsp;
  <sup>5</sup>The Hong Kong University of Science and Technology
</div>

<div class="post-authors" style="margin-bottom:20px; font-weight: bold;">
  Computer Vision and Pattern Recognition (CVPR), 2025
</div>

<div style="margin-bottom: 1em;" class="post-authors">
  <div class="col-md-8 col-md-offset-2 text-center">
    <ul class="nav nav-pills nav-justified" style="box-shadow:0 0">
      <li>
        <a href="https://alexlai2860.github.io/mypaper/cvpr2025_snowmaster/SnowMasterfinalrelease.pdf">
          <img class="post-logo" src="https://alexlai2860.github.io/images/logo/paper.jpg" height="50px">
          <h5><strong>Paper</strong></h5>
        </a>
      </li>
      <li>
        <a href="https://alexlai2860.github.io/SnowMaster/">
          <img class="post-logo" src="https://alexlai2860.github.io/images/logo/paper.jpg" height="50px">
          <h5><strong>CVPR 2025</strong></h5>
        </a>
      </li>
      <li>
        <a href="https://drive.google.com/file/d/1NMLhuUVD6gCifyqJJbeacljrB1pV8byh/view?usp=sharing">
          <img class="post-logo" src="https://alexlai2860.github.io/images/logo/datatset.jpg" height="50px">
          <h5><strong>Dataset</strong></h5>
        </a>
      </li>                        
      <li>
        <a href="https://alexlai2860.github.io/SnowMaster/">
          <img class="post-logo" src="https://alexlai2860.github.io/images/logo/github.png" height="50px">
          <h5><strong>Code</strong></h5>
        </a>
      </li>
      <li>
        <a href="https://alexlai2860.github.io/mypaper/cvpr2025_snowmaster/04956_supp.pdf">
          <img class="post-logo" src="https://alexlai2860.github.io/images/logo/supplementary.jpg" height="50px">
          <h5><strong>Supplementary</strong></h5>
        </a>
      </li>
    </ul>
  </div>
</div>

<div class="post-line"></div>

<!-- 演示效果展示 -->
<div style="box-shadow:3px 6px 13px 0px rgba(0,0,0,0.5); margin-bottom: 2em;">
  <div class="post-img-group">
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%" src="https://alexlai2860.github.io/images/snowmaster/gif_hq/gif_img2_6s_h264.gif" alt="Desnowing Result 1">
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%" src="https://alexlai2860.github.io/images/snowmaster/gif_hq/gif_img5_6s_h264.gif" alt="Desnowing Result 2">
  </div> 
  <div class="post-img-group">
    <img class="post-img" style="left:0;right:0;margin-bottom:0;width:100%" src="https://alexlai2860.github.io/images/snowmaster/gif_hq/gif_img6_6s_h264_crop_small.gif" alt="Desnowing Result 3">
  </div> 
</div>

<!-- Abstract 部分 -->
<div style="background-color:#f0f1f3a6; margin-bottom: 2em;">
  <h2 class="post-section" style="padding-left: 25px; margin-bottom: 0px; padding-top: 20px;">Abstract</h2>
  <p style="padding: 25px; padding-top: 10px; text-align: justify; line-height: 1.6;">
    Snowfall presents significant challenges for visual data processing, necessitating specialized desnowing algorithms. However, existing models often fail to generalize effectively due to their heavy reliance on synthetic datasets. Furthermore, current real-world snowfall datasets are limited in scale and lack dedicated evaluation metrics designed specifically for snowfall degradation, thus hindering the effective integration of real snowy images into model training to reduce domain gaps.
    <br><br>
    To address these challenges, we first introduce RealSnow10K, a large-scale, high-quality dataset consisting of over 10,000 annotated real-world snowy images. In addition, we curate a preference dataset comprising 36,000 expert-ranked image pairs, enabling the adaptation of multimodal large language models (MLLMs) to better perceive snowy image quality through our innovative Multi-Model Preference Optimization (MMPO). Finally, we propose the <strong>SnowMaster</strong>, which employs MMPO-enhanced MLLM to perform accurate snowy image evaluation and pseudo-label filtering for semi-supervised training. Experiments demonstrate that SnowMaster delivers superior desnowing performance under real-world conditions.
  </p>
</div>

<!-- Dataset 部分 -->
<h2 class="post-section" style="text-align: center; margin-bottom: 20px; padding-top: 20px;">Dataset</h2>
<div style="box-shadow:3px 6px 13px 0px rgba(0,0,0,0.5); margin-bottom: 2em;">
  <img class="post-img" style="display: block; max-width:100%; margin: 0;" src="https://alexlai2860.github.io/images/snowmaster/dataset_construction_fix.png" alt="Overall Framework">
</div>

<!-- Method 部分 -->
<h2 class="post-section" style="text-align: center; margin-bottom: 20px; padding-top: 20px;">Method</h2>
<div style="box-shadow:3px 6px 13px 0px rgba(0,0,0,0.5); margin-bottom: 2em;">
  <img class="post-img" style="display: block; max-width:100%; margin: 0;" src="https://alexlai2860.github.io/images/snowmaster/overview_cvpr2025_snowmaster.png" alt="Overall Framework">
</div>

<!-- Quantitative Comparison 部分 -->
<h2 class="post-section" style="text-align: center; margin-bottom: 20px; padding-top: 20px;">Quantitative Comparison</h2>
<div style="box-shadow:3px 6px 13px 0px rgba(0,0,0,0.5); margin-bottom: 2em;">
  <div class="post-img-group">
    <img class="post-img" style="max-width:100%;margin-bottom:0;" src="https://alexlai2860.github.io/images/snowmaster/NRIQA_comparison.png" alt="Quantitative Results">
  </div>
</div>


<!-- Method 部分 -->
<h2 class="post-section" style="text-align: center; margin-bottom: 20px; padding-top: 20px;">Visual Comparison</h2>
<div style="box-shadow:3px 6px 13px 0px rgba(0,0,0,0.5); margin-bottom: 2em;">
  <img class="post-img" style="display: block; max-width:100%; margin: 0;" src="https://alexlai2860.github.io/images/snowmaster/visual_comp_fix_Page1new.png" alt="Visual Comparison 1">
</div>


<!-- Visual Comparison 部分 -->
<h2 class="post-section" style="text-align: center; margin-bottom: 20px; padding-top: 20px;">More Examples</h2>

<!-- 交互式对比 -->
<div style="box-shadow:3px 6px 13px 0px rgba(0,0,0,0.5); margin-bottom: 2em;">  
  <div class="post-img-group">
    <iframe style="max-width:50%;margin-top:0px;text-align: left;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="270" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=400508fe-41d5-11f0-bb24-0936e1cb08fb"></iframe>
    <iframe style="max-width:50%;margin-bottom:0px;text-align: right;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="270" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=4d74d646-41d4-11f0-bb24-0936e1cb08fb"></iframe>
  </div> 
  <div class="post-img-group">
    <iframe style="max-width:50%;margin-top:0px;text-align: left;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="270" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=e371a146-41d0-11f0-bb24-0936e1cb08fb"></iframe>
    <iframe style="max-width:50%;margin-bottom:0px;text-align: right;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="270" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=a393d210-41d5-11f0-bb24-0936e1cb08fb"></iframe>
  </div> 
  <div class="post-img-group">
    <iframe style="max-width:100%;margin-bottom:0px;text-align: center;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="100%" height="540" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=f9a47ab0-41d0-11f0-bb24-0936e1cb08fb"></iframe>
  </div>
  <div class="post-img-group">
    <iframe style="width:100%; margin:0; padding:0; display:block;" frameborder="0" class="juxtapose" width="100%" height="450" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=bd2752d4-0a2a-11f0-9397-d93975fe8866"></iframe>
  </div>
</div>

<!-- Citation 部分 -->
<h2 class="post-section" style="margin-top: 40px;">Citation</h2>

```bibtex
@inproceedings{lai2025snowmaster,
  title={SnowMaster: Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization},
  author={Lai, Jianyu and Chen, Sixiang and Lin, Yunlong and Ye, Tian and Liu, Yun and Fei, Song and Xing, Zhaohu and Wu, Hongtao and Wang, Weiming and Zhu, Lei},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year={2025}
}
```
```