---
layout: fancy_home
permalink: /publications/
title: Publications
---

<style>
.pub-container {
    max-width: 1000px;
    margin: 0 auto;
}

.eyebrow {
    text-transform: uppercase;
    letter-spacing: 0.18em;
    font-size: 0.85rem;
    margin: 0;
    color: #0d9488;
    font-weight: 600;
}

.intro {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    padding: 2.5rem;
    border-radius: 32px;
    background: rgba(255, 255, 255, 0.92);
    box-shadow: 0 24px 60px rgba(30, 41, 59, 0.1);
    border: 1px solid rgba(13, 148, 136, 0.1);
}

.intro-text {
    flex: 1 1 360px;
}

.intro-text h1 {
    margin: 0.4rem 0 1rem;
    font-size: 2.4rem;
    font-weight: 800;
    color: #0f172a;
    line-height: 1.2;
}

.intro-text p {
    font-size: 1.05rem;
    color: #334155;
    line-height: 1.75;
}

.intro-tags {
    margin-top: 1.5rem;
}

.intro-tags span {
    display: inline-block;
    padding: 0.4rem 1rem;
    border-radius: 999px;
    border: 1px solid rgba(13, 148, 136, 0.3);
    margin: 0 0.5rem 0.5rem 0;
    font-size: 0.85rem;
    color: #0d9488;
    background: rgba(13, 148, 136, 0.08);
}

.intro-counters {
    display: flex;
    flex: 1 1 260px;
    gap: 1rem;
}

.counter-card {
    flex: 1;
    background: white;
    border-radius: 22px;
    border: 1px solid rgba(13, 148, 136, 0.15);
    text-align: center;
    padding: 1.2rem;
    transition: all 0.3s ease;
}

.counter-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 35px rgba(13, 148, 136, 0.15);
    border-color: rgba(13, 148, 136, 0.3);
}

.counter-value {
    font-size: 2.1rem;
    font-weight: 800;
    color: #0d9488;
}

.counter-label {
    font-size: 0.9rem;
    color: #64748b;
    margin-top: 0.4rem;
}

.section-header {
    margin: 3rem 0 1.5rem;
}

.section-header h2,
.timeline-heading h2 {
    margin: 0;
    font-size: 1.25rem;
    font-family: 'Inter', 'Helvetica Neue', Arial, sans-serif;
    text-transform: uppercase;
    letter-spacing: 0.18em;
    color: #0f766e;
    font-weight: 700;
}

.highlight-list {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

.highlight-card {
    position: relative;
    display: flex;
    align-items: stretch;
    gap: 1.8rem;
    padding: 1.6rem 1.8rem 1.6rem 2.8rem;
    border-radius: 30px;
    background: rgba(255, 255, 255, 0.92);
    border: 1px solid rgba(30, 41, 59, 0.06);
    box-shadow: 0 25px 65px rgba(30, 41, 59, 0.1);
    backdrop-filter: blur(10px);
    overflow: visible;
    transition: all 0.4s ease;
}

.highlight-card::before {
    content: '';
    position: absolute;
    left: -6px;
    top: 18px;
    bottom: 18px;
    width: 10px;
    border-radius: 999px;
    background: linear-gradient(180deg, #0d9488, #0891b2);
    box-shadow: 0 6px 18px rgba(13, 148, 136, 0.35);
}

.highlight-card::after {
    content: '';
    position: absolute;
    left: -12px;
    top: 10px;
    bottom: 10px;
    width: 22px;
    border-radius: 999px;
    background: linear-gradient(180deg, rgba(13, 148, 136, 0.16), rgba(8, 145, 178, 0.12));
    filter: blur(5px);
    z-index: -1;
}

.highlight-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 30px 70px rgba(13, 148, 136, 0.15);
}

.highlight-media {
    flex: 0 0 280px;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
}

.highlight-media img {
    width: 100%;
    height: auto;
    max-height: 220px;
    object-fit: contain;
    border-radius: 22px;
    background: #fff;
    padding: 0.35rem;
    box-shadow: 0 8px 20px rgba(13, 148, 136, 0.12);
}

.badge {
    position: absolute;
    top: -8px;
    left: -12px;
    padding: 0.3rem 0.8rem;
    border-radius: 999px;
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    color: #fff;
    font-weight: 600;
}

.badge-teal {
    background: linear-gradient(135deg, #0d9488, #0891b2);
}

.badge-green {
    background: linear-gradient(135deg, #059669, #047857);
}

.badge-cyan {
    background: linear-gradient(135deg, #0891b2, #0e7490);
}

.highlight-content {
    flex: 1;
    display: flex;
    flex-direction: column;
}

.highlight-content h3 {
    margin: 0 0 0.35rem;
    font-size: 1.15rem;
    line-height: 1.35;
    font-weight: 700;
    color: #0f172a;
}

.authors {
    margin: 0 0 0.6rem;
    font-size: 0.85rem;
    color: #64748b;
}

.authors strong u {
    color: #ffffff !important;
    font-weight: 700 !important;
    text-decoration: none !important;
    background: linear-gradient(135deg, #0d9488, #0891b2) !important;
    padding: 2px 8px !important;
    border-radius: 6px !important;
    box-shadow: 0 2px 8px rgba(13, 148, 136, 0.3) !important;
}

.summary {
    margin: 0;
    font-size: 0.95rem;
    color: #475569;
    line-height: 1.6;
}

.resource-list {
    margin-top: auto;
    padding-top: 0.8rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
    align-items: center;
}

.resource-list a {
    font-size: 0.85rem;
    font-weight: 600;
    text-decoration: none;
    color: #0d9488;
    padding: 0.25rem 0.6rem;
    border-radius: 6px;
    background: rgba(13, 148, 136, 0.08);
    transition: all 0.2s ease;
}

.resource-list a:hover {
    background: rgba(13, 148, 136, 0.15);
    color: #0f766e;
}

.gh-btn-wrap {
    display: inline-flex;
    align-items: center;
    margin-left: 0.3rem;
}

.gh-btn-wrap iframe {
    border: none;
}

.timeline-block {
    margin-top: 4rem;
}

.timeline-heading {
    margin-bottom: 1rem;
}

.timeline-list {
    border-top: 2px solid rgba(13, 148, 136, 0.2);
}

.timeline-row {
    display: flex;
    gap: 1.5rem;
    padding: 1.6rem 0;
    border-bottom: 1px solid rgba(30, 41, 59, 0.08);
    transition: all 0.3s ease;
}

.timeline-row:hover {
    background: rgba(13, 148, 136, 0.03);
    padding-left: 1rem;
    margin-left: -1rem;
    margin-right: -1rem;
    padding-right: 1rem;
    border-radius: 12px;
}

.timeline-meta {
    min-width: 150px;
    text-align: right;
}

.meta-type {
    display: block;
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 0.12em;
    color: #94a3b8;
}

.meta-date {
    margin-top: 0.3rem;
    font-weight: 600;
    color: #0d9488;
}

.timeline-body h3 {
    margin: 0 0 0.35rem;
    font-size: 1.1rem;
    font-weight: 600;
    color: #0f172a;
    line-height: 1.4;
}

.timeline-body .pub-prefix {
    color: #0d9488;
    font-weight: 700;
    margin-right: 0.4rem;
}

.timeline-authors {
    margin: 0.2rem 0 0.35rem;
    font-size: 0.9rem;
    color: #6b7280;
}

.timeline-authors strong u {
    color: #ffffff !important;
    font-weight: 700 !important;
    text-decoration: none !important;
    background: linear-gradient(135deg, #0d9488, #0891b2) !important;
    padding: 2px 8px !important;
    border-radius: 6px !important;
    box-shadow: 0 2px 8px rgba(13, 148, 136, 0.3) !important;
}

.timeline-body p {
    margin: 0;
    color: #475569;
    line-height: 1.5;
}

.resource-inline {
    margin-top: 0.6rem;
    font-size: 0.9rem;
}

.resource-inline a {
    color: #0d9488;
    font-weight: 600;
    text-decoration: none;
    transition: color 0.2s ease;
}

.resource-inline a:hover {
    color: #0f766e;
}

.resource-inline a + a::before {
    content: " | ";
    color: #94a3b8;
}

@media (max-width: 900px) {
    .intro {
        flex-direction: column;
    }
    
    .intro-counters {
        width: 100%;
    }
    
    .highlight-card {
        flex-direction: column;
    }
    
    .highlight-media {
        width: 100%;
    }
    
    .timeline-row {
        flex-direction: column;
    }
    
    .timeline-meta {
        text-align: left;
    }
}
</style>

<div class="pub-container">
    <section class="intro fade-in">
        <div class="intro-text">
            <p class="eyebrow">Research Snapshot</p>
            <h1>Visual Frontiers & Generative Intelligence</h1>
            <p>My research lies at the intersection of <strong>Low-level Vision</strong>, <strong>AIGC</strong>, and <strong>Multimodal Large Language Models</strong>. I build frameworks like <strong>PosterCraft</strong> and <strong>PosterOmni</strong> for high-quality poster generation, design reward models for human-aligned generation in <strong>PosterReward</strong>, and explore MLLM applications in image restoration tasks like <strong>SnowMaster</strong> and <strong>GenHaze</strong>.</p>
            <div class="intro-tags">
                <span>Low-level Vision</span>
                <span>AIGC</span>
                <span>Reward Modeling</span>
                <span>MLLM</span>
            </div>
        </div>
        <div class="intro-counters">
            <div class="counter-card">
                <div class="counter-value">3</div>
                <div class="counter-label">CVPR / ICCV</div>
            </div>
            <div class="counter-card">
                <div class="counter-value">1</div>
                <div class="counter-label">ICLR</div>
            </div>
            <div class="counter-card">
                <div class="counter-value">5</div>
                <div class="counter-label">Total Publications</div>
            </div>
        </div>
    </section>

    <section class="highlight-block">
        <div class="section-header">
            <h2>Highlight Research</h2>
        </div>

        <div class="highlight-list">
            <article class="highlight-card">
                <div class="highlight-media">
                    <img src="https://alexlai2860.github.io/images/posterreward/concat.png" alt="PosterReward">
                    <span class="badge badge-teal">CVPR 2026</span>
                </div>
                <div class="highlight-content">
                    <h3>PosterReward: Unlocking Accurate Evaluation for High-Quality Graphic Design Generation</h3>
                    <p class="authors"><strong><u>Jianyu Lai*</u></strong>, Sixiang Chen*, Jialin Gao*, Hengyu Shi, Zhongying Liu, Fuxiang Zhai, Junfeng Luo, Xiaoming Wei, Lujia Wang, Lei Zhu✉️</p>
                    <p class="summary">A comprehensive reward model for design aesthetics and typography, trained on an automated preference dataset to unlock accurate evaluation for high-quality graphic design generation.</p>
                    <div class="resource-list">
                        <a href="/mypaper/posterreward/PosterReward_Arxiv_official.pdf">📄 Paper</a>
                        <a href="/PosterReward/">🌐 Project</a>
                        <a href="https://huggingface.co/PosterReward">🤗 Model</a>
                    </div>
                </div>
            </article>

            <article class="highlight-card">
                <div class="highlight-media">
                    <img src="https://ephemeral182.github.io/images/posteromni/teaser_0209.jpg" alt="PosterOmni">
                    <span class="badge badge-teal">CVPR 2026</span>
                </div>
                <div class="highlight-content">
                    <h3>PosterOmni — Generalized Artistic Poster Creation via Task Distillation and Unified Reward Feedback</h3>
                    <p class="authors">Sixiang Chen*, <strong><u>Jianyu Lai*</u></strong>, Jialin Gao*, Hengyu Shi*, Zhongying Liu*, Tian Ye, Junfeng Luo, Xiaoming Wei, Lei Zhu✉️</p>
                    <p class="summary">One model for poster creation—unifying local edits and global design for generalized multi-task image/poster-to-poster generation. ✨ Your intelligent assistant for high-quality aesthetic poster creation!</p>
                    <div class="resource-list">
                        <a href="https://arxiv.org/abs/2602.12127">📄 Paper</a>
                        <a href="https://ephemeral182.github.io/PosterOmni/">🌐 Project</a>
                        <a href="https://huggingface.co/MeiGen-AI/PosterOmni_v1">🤗 Model</a>
                        <a href="https://github.com/MeiGen-AI/PosterOmni" target="_blank" rel="noopener">🐙 GitHub</a>
                        <span class="gh-btn-wrap">
                            <iframe src="https://ghbtns.com/github-btn.html?user=MeiGen-AI&repo=PosterOmni&type=star&count=true&size=small" frameborder="0" scrolling="0" width="100" height="20" title="PosterOmni GitHub Star"></iframe>
                        </span>
                        <span class="gh-btn-wrap">
                            <iframe src="https://ghbtns.com/github-btn.html?user=MeiGen-AI&repo=PosterOmni&type=fork&count=true&size=small" frameborder="0" scrolling="0" width="98" height="20" title="PosterOmni GitHub Fork"></iframe>
                        </span>
                    </div>
                </div>
            </article>

            <article class="highlight-card">
                <div class="highlight-media">
                    <img src="https://ephemeral182.github.io/images/postercraft/pub/fig1.png" alt="PosterCraft">
                    <span class="badge badge-green">ICLR 2026</span>
                </div>
                <div class="highlight-content">
                    <h3>PosterCraft — Rethinking High-Quality Aesthetic Poster Generation in a Unified Framework</h3>
                    <p class="authors">Sixiang Chen*, <strong><u>Jianyu Lai*</u></strong>, Jialin Gao*, Tian Ye, Haoyu Chen, Hengyu Shi, Shitong Shao, Yunlong Lin, Song Fei, Zhaohu Xing, Yeying Jin, Junfeng Luo, Xiaoming Wei, Lei Zhu✉️</p>
                    <p class="summary">A new framework for high-quality aesthetic poster generation. ✨ From your prompts to high-quality aesthetic posters!</p>
                    <div class="resource-list">
                        <a href="https://arxiv.org/abs/2506.10741">📄 Paper</a>
                        <a href="https://ephemeral182.github.io/PosterCraft/">🌐 Project</a>
                        <a href="https://huggingface.co/PosterCraft/PosterCraft-v1_RL">🤗 Model</a>
                        <a href="https://github.com/Ephemeral182/PosterCraft" target="_blank" rel="noopener">🐙 GitHub</a>
                        <span class="gh-btn-wrap">
                            <iframe src="https://ghbtns.com/github-btn.html?user=Ephemeral182&repo=PosterCraft&type=star&count=true&size=small" frameborder="0" scrolling="0" width="100" height="20" title="PosterCraft GitHub Star"></iframe>
                        </span>
                        <span class="gh-btn-wrap">
                            <iframe src="https://ghbtns.com/github-btn.html?user=Ephemeral182&repo=PosterCraft&type=fork&count=true&size=small" frameborder="0" scrolling="0" width="98" height="20" title="PosterCraft GitHub Fork"></iframe>
                        </span>
                    </div>
                </div>
            </article>
        </div>
    </section>

    <section class="timeline-block fade-in">
        <div class="timeline-heading">
            <h2>Selected Publications</h2>
        </div>
        <div class="timeline-list">
            <article class="timeline-row">
                <div class="timeline-meta">
                    <span class="meta-type">Conference</span>
                    <span class="meta-date">Feb 2026</span>
                </div>
                <div class="timeline-body">
                    <h3><span class="pub-prefix">[CVPR 2026]</span> PosterOmni — Generalized Artistic Poster Creation via Task Distillation and Unified Reward Feedback</h3>
                    <p class="timeline-authors">Sixiang Chen*, <strong><u>Jianyu Lai*</u></strong>, Jialin Gao*, Hengyu Shi*, Zhongying Liu*, Tian Ye, Junfeng Luo, Xiaoming Wei, Lei Zhu</p>
                    <p>One model for poster creation—unifying local edits and global design for generalized multi-task image/poster-to-poster generation.</p>
                    <div class="resource-inline">
                        <a href="https://ephemeral182.github.io/PosterOmni/">Project Page</a>
                        <a href="https://arxiv.org/abs/2602.12127">Paper</a>
                        <a href="https://github.com/MeiGen-AI/PosterOmni">Code</a>
                        <a href="https://huggingface.co/MeiGen-AI/PosterOmni_v1">Model</a>
                    </div>
                </div>
            </article>

            <article class="timeline-row">
                <div class="timeline-meta">
                    <span class="meta-type">Conference</span>
                    <span class="meta-date">Feb 2026</span>
                </div>
                <div class="timeline-body">
                    <h3><span class="pub-prefix">[CVPR 2026]</span> PosterReward: Unlocking Accurate Evaluation for High-Quality Graphic Design Generation</h3>
                    <p class="timeline-authors"><strong><u>Jianyu Lai*</u></strong>, Sixiang Chen*, Jialin Gao*, Hengyu Shi, Zhongying Liu, Fuxiang Zhai, Junfeng Luo, Xiaoming Wei, Lujia Wang, Lei Zhu</p>
                    <p>A comprehensive reward model for design aesthetics and typography, trained on automated preference dataset.</p>
                    <div class="resource-inline">
                        <a href="/PosterReward/">Project Page</a>
                        <a href="/mypaper/posterreward/PosterReward_Arxiv_official.pdf">Paper</a>
                        <a href="https://huggingface.co/PosterReward">Model</a>
                    </div>
                </div>
            </article>

            <article class="timeline-row">
                <div class="timeline-meta">
                    <span class="meta-type">Conference</span>
                    <span class="meta-date">Jan 2026</span>
                </div>
                <div class="timeline-body">
                    <h3><span class="pub-prefix">[ICLR 2026]</span> PosterCraft — Rethinking High-Quality Aesthetic Poster Generation in a Unified Framework</h3>
                    <p class="timeline-authors">Sixiang Chen*, <strong><u>Jianyu Lai*</u></strong>, Jialin Gao*, Tian Ye, Haoyu Chen, Hengyu Shi, Shitong Shao, Yunlong Lin, Song Fei, Zhaohu Xing, Yeying Jin, Junfeng Luo, Xiaoming Wei, Lei Zhu</p>
                    <p>A unified framework for high-quality aesthetic poster generation.</p>
                    <div class="resource-inline">
                        <a href="https://ephemeral182.github.io/PosterCraft/">Project Page</a>
                        <a href="https://arxiv.org/abs/2506.10741">Paper</a>
                        <a href="https://github.com/Ephemeral182/PosterCraft">Code</a>
                        <a href="https://huggingface.co/PosterCraft/PosterCraft-v1_RL">Model</a>
                    </div>
                </div>
            </article>

            <article class="timeline-row">
                <div class="timeline-meta">
                    <span class="meta-type">Conference</span>
                    <span class="meta-date">Jun 2025</span>
                </div>
                <div class="timeline-body">
                    <h3><span class="pub-prefix">[ICCV 2025]</span> GenHaze — Pioneering Controllable One-Step Realistic Haze Generation for Real-World Dehazing</h3>
                    <p class="timeline-authors">Sixiang Chen, Tian Ye, Yunlong Lin, Yeying Jin, Yijun Yang, Haoyu Chen, <strong><u>Jianyu Lai</u></strong>, Song Fei, Zhaohu Xing, Fugee Tsung, Lei Zhu</p>
                    <p>Proposes a one-step, reference-controllable haze generator that better matches real-world haze complexity.</p>
                    <div class="resource-inline">
                        <a href="https://ephemeral182.github.io/GenHaze/">Project Page</a>
                    </div>
                </div>
            </article>

            <article class="timeline-row">
                <div class="timeline-meta">
                    <span class="meta-type">Conference</span>
                    <span class="meta-date">Feb 2025</span>
                </div>
                <div class="timeline-body">
                    <h3><span class="pub-prefix">[CVPR 2025]</span> SnowMaster — Comprehensive Real-world Image Desnowing via MLLM with Multi-Model Feedback Optimization</h3>
                    <p class="timeline-authors"><strong><u>Jianyu Lai*</u></strong>, Sixiang Chen*, Yunlong Lin, Tian Ye, Yun Liu, Song Fei, Zhaohu Xing, Hongtao Wu, Weiming Wang, Lei Zhu</p>
                    <p>Uses an MLLM as an evaluator to rank/filter pseudo-labels, enabling semi-supervised training for real-world desnowing.</p>
                    <div class="resource-inline">
                        <a href="https://openaccess.thecvf.com/content/CVPR2025/papers/Lai_SnowMaster_Comprehensive_Real-world_Image_Desnowing_via_MLLM_with_Multi-Model_Feedback_CVPR_2025_paper.pdf">Paper</a>
                    </div>
                </div>
            </article>
        </div>
    </section>
</div>
