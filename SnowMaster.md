---
layout: post1
permalink: /SnowMaster/index.html #/publications.html
title: "SnowMaster: Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization"
---


<h2 class="post-title" style="margin-bottom:7px;margin-top:20px;font-weight:400;">SnowMaster: Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization</h2>
<!-- <h2 class="post-title" style="margin-bottom:20px;margin-top:7px;">Unified Removal of Raindrops and Rain Streaks</h2>  -->

<div class="post-authors" style="margin-bottom:5px;">
  <a href="https://alexlai2860.github.io">Jianyu Lai</a><sup>1,*</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://ephemeral182.github.io">Sixiang Chen</a><sup>1,*, &#9828;</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://lyl1015.github.io/">Yunlong Lin</a><sup>2</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://owen718.github.io">Tian Ye</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  Yun Liu<sup>3</sup>&nbsp;&nbsp;&nbsp;
  Song Fei<sup>1</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://ge-xing.github.io/">Zhaohu Xing</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://hongtao-wu.github.io/">Hongtao Wu</a><sup>1</sup>&nbsp;&nbsp;&nbsp;
  Weiming Wang<sup>4</sup>&nbsp;&nbsp;&nbsp;
  <a href="https://sites.google.com/site/indexlzhu/home">Lei Zhu</a><sup>1,5,✉️</sup>
  <br>
  <sup>1</sup>The Hong Kong University of Science and Technology (Guangzhou)&nbsp;&nbsp;&nbsp;
  <sup>2</sup>Xiamen University&nbsp;&nbsp;&nbsp;
  <sup>3</sup>Southwestern University&nbsp;&nbsp;&nbsp;
  <sup>4</sup>Hong Kong Metropolitan University&nbsp;&nbsp;&nbsp;
  <sup>5</sup>The Hong Kong University of Science and Technology&nbsp;&nbsp;&nbsp;
</div>

<div class="symbols-legend" style="margin: 15px 0; font-size: 1em; color: #555;">
  <span style="margin-right: 20px;"><strong>*</strong> - Equal Contribution</span>
  <span style="margin-right: 20px;"><strong><sup>&#9828;</sup></strong> - Project Lead</span>
  <span><strong><sup>✉️</sup></strong> - Corresponding Author</span>
</div>

<div class="post-authors" style="margin-bottom:20px;">
  Computer Vision and Pattern Recognition (CVPR), 2025
</div>


<div style="margin-bottom: 0.7em;" class="post-authors">
                <div class="col-md-8 col-md-offset-2 text-center">
                    <ul class="nav nav-pills nav-justified" style="box-shadow:0 0">
                        <li>
                            <a href="https://alexlai2860.github.io/SnowMaster/">
                            <!-- <a href="https://arxiv.org/abs/2112.05504"> -->
                            <img class="post-logo" src="https://alexlai2860.github.io/images/logo/paper.jpg" height="50px">
                                <h5><strong>arXiv</strong></h5>
                            </a>
                        </li>
                        <li>
                             <a href="https://alexlai2860.github.io/SnowMaster/">
                            <img class="post-logo" src="https://alexlai2860.github.io/images/logo/paper.jpg" height="50px">
                                <h5><strong>CVPR 2025</strong></h5>
                            </a>
                        </li>
                        <li>
                             <a href="https://alexlai2860.github.io/SnowMaster/">
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
                                <h5><strong>Supplementery</strong></h5>
                            </a>
                        </li>
                    </ul>
                </div>
        </div>

<div class="post-line"></div>

<div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">
<div class="post-img-group">
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%" src="https://ephemeral182.github.io/images/real_gif1.gif" alt="Left Image"><!--&nbsp;&nbsp;!-->
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%" src="https://ephemeral182.github.io/images/real_gif2.gif" alt="Right Image">
  </div> 
  <div class="post-img-group">
    <img class="post-img" style="left:0;right:0;margin-bottom:0;width:100%" src="https://ephemeral182.github.io/images/350.gif" alt="Left Image">
  </div> 
  </div> 



  <!-- <div class="post-img-group">
    <img class="post-img" src="../assets/img/VideoDesnowing/1.gif" alt="Left Image">
    <img class="post-img" src="../assets/img/VideoDesnowing/2.gif" alt="Right Image">
  </div> -->

<!-- <img src="../assets/img/VideoDesnowing/1.gif" class="post-img" role="img"> -->


<div style="background-color:#f0f1f3a6;">
  <h2 class="post-section" style="padding-left: 25px; margin-bottom: 0px; padding-top: 20px;">Abstract</h2>
  <p style="padding: 25px; padding-top: 10px;">
    Snowfall presents significant challenges for visual data processing, necessitating specialized desnowing algorithms. However, existing models often fail to generalize effectively due to their heavy reliance on synthetic datasets. Furthermore, current real-world snowfall datasets are limited in scale and lack dedicated evaluation metrics designed specifically for snowfall degradation, thus hindering the effective integration of real snowy images into model training to reduce domain gaps.
    To address these challenges, we first introduce RealSnow10K, a large-scale, high-quality dataset consisting of over 10,000 annotated real-world snowy images. In addition, we curate a preference dataset comprising 36,000 expert-ranked image pairs, enabling the adaptation of multimodal large language models (MLLMs) to better perceive snowy image quality through our innovative Multi-Model Preference Optimization (MMPO). Finally, we propose the <strong>SnowMaster</strong>, which employs MMPO-enhanced MLLM to perform accurate snowy image evaluation and pseudo-label filtering for semi-supervised training. Experiments demonstrate that SnowMaster delivers superior desnowing performance under real-world conditions.
  </p>
</div>

<h2 class="post-section" style="text-align: center; padding-left: 25px; margin-bottom: 10px; padding-top: 20px;">Method</h2>
<div style="box-shadow:3px 6px 13px 0px rgba(0,0,0,0.5)">
  <div class="post-img-group">
    <!-- <img class="post-img" style="max-width:100%" src="https://alexlai2860.github.io/images/overview_cvpr2025_snowmaster.png" alt="Overall Framework"> -->
    <img class="post-img" style="display: block; max-width:100%" src="https://alexlai2860.github.io/images/snowmaster/overview_cvpr2025_snowmaster.png" alt="Overall Framework">
  </div>
</div>

<h2 class="post-section" style="
    text-align: center;
    padding-left: 25px;
    margin-bottom: 10px;
    padding-top: 20px;
">Quantitative Comparison</h2>
<div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">
  <div class="post-img-group">
    <img class="post-img" style="max-width:100%;margin-bottom:0;" src="https://alexlai2860.github.io/images/snowmaster/NRIQA_comparison.png"  alt="Left Image">
  </div>
  </div>


<h2 class="post-section" style="
    text-align: center;
    padding-left: 25px;
    margin-bottom: 10px;
    padding-top: 20px;
">Visual Comparison</h2>
<div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">
  <div class="post-img-group">
    <img class="post-img" style="max-width:100%;margin-bottom:2px;" src="https://ephemeral182.github.io/images/udr_visual1.png"  alt="Left Image">
  </div>
    <div class="post-img-group">
    <img class="post-img" style="max-width:100%;margin-bottom:0;" src="https://ephemeral182.github.io/images/udr_visual3.png"  alt="Left Image">
  </div>
    <div class="post-img-group">
    <img class="post-img" style="max-width:100%;margin-bottom:0;" src="https://ephemeral182.github.io/images/udr_visual4.png"  alt="Left Image">
  </div>
    <div class="post-img-group">
    <img class="post-img" style="max-width:100%;margin-bottom:10px;" src="https://ephemeral182.github.io/images/udr_visual5.png"  alt="Left Image">
  </div>
  </div>



 <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">  
<div class="post-img-group">
<iframe style="max-width:50%;margin-top:0px;text-align: left;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="250"  src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=1486a714-3ea3-11ee-b5bd-6595d9b17862"></iframe>
<iframe style="max-width:50%;margin-bottom:0px;text-align: right;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="250" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=209744e0-3ea4-11ee-b5bd-6595d9b17862"></iframe>
</div> 
<div class="post-img-group">
<iframe style="max-width:50%;margin-top:0px;text-align: left;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="250"  src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=c58fedd2-3f3d-11ee-b5bd-6595d9b17862"></iframe>
<iframe style="max-width:50%;margin-bottom:0px;text-align: right;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="50%" height="250" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=0ded7a4a-3f3e-11ee-b5bd-6595d9b17862"></iframe>
</div> 
<div class="post-img-group">
<iframe style="max-width:100%;margin-bottom:0px;text-align: right;margin: 0;padding: 0;display: flex;" frameborder="0" class="juxtapose" width="100%" height="371" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=2ad2a594-3f3f-11ee-b5bd-6595d9b17862"></iframe>
</div>
</div>

<!-- <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">
<div class="post-img-group">
<img style="padding: 10px; width: 450;text-align: left;" frameborder="0" class="juxtapose" height="455" width="600" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=ae97ac46-3ea2-11ee-b5bd-6595d9b17862">
<img style="padding: 10px; width: 450;text-align: right;" frameborder="0" class="juxtapose" height="455" width="600" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid=5b6cf096-3e7d-11ee-b5bd-6595d9b17862">
</div> 
</div>  -->

<!-- <div style="box-shadow:3px 6px 13px 0px  rgba(0,0,0,0.5)">
<div class="post-img-group">
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%;height:70" src="https://ephemeral182.github.io/images/real3.gif" alt="Left Image"><!--&nbsp;&nbsp;
    <img class="post-img" style="left:0;right:0;margin-bottom:0px;max-width:50%;height:70" src="https://ephemeral182.github.io/images/real4.gif" alt="Right Image">
  </div> 
</div>  -->

<!-- <h2 class="post-section"  style="font-weight:300;"><strong>R</strong>ealistic <strong>V</strong>ideo De<strong>S</strong>nowing <strong>D</strong>ataset</h2>

- <strong>RVSD</strong> contains a total of 110 pairs of videos. 
- Each pair contains <strong>snowy</strong> and  <strong>hazy</strong> videos and corresponding snow-free and haze-free ground truth videos. 
- We use a rendering engine (Unreal Engine 5) and various augmentation techniques to generate snow and haze with diverse and realistic physical properties. This results in more realistic and varied synthesized videos, which improve the model's performance on real-world data. 



<div class="post-section"  style="font-weight:700;">Download</div>
<!-- <div style="font-weight:300;">Train (100 videos):  [Google Drive]  [Baidu Netdisk (password: 7t74)]</div>
<div style="font-weight:300;">Test (20 videos):  [Google Drive]  [Baidu Netdisk (password: 7t74)] </div> -->



<!-- - **Train (80 videos):**  
    [Google Drive]  [Baidu Netdisk (password: 7t74)]
- **Test (30 videos):**  
    [Google Drive]  [Baidu Netdisk (password: 7t74)] --> 

<h2 class="post-section">Citation</h2>


```
@inproceedings{lai2025snowmaster,
  title={SnowMaster: Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization},
  author={Lai, Jianyu and Chen, Sixiang and Lin, Yunlong and Ye, Tian and Liu, Yun and Fei, Song and Xing, Zhaohu and Wu, Hongtao and Wang, Weiming and Zhu, Lei},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year={2025}
}