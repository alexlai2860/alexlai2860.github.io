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

.intro {
    background: rgba(255, 255, 255, 0.9);
    border-radius: 24px;
    padding: 2.5rem;
    margin-bottom: 3rem;
    box-shadow: 0 15px 35px rgba(30, 41, 59, 0.08);
    border: 1px solid rgba(13, 148, 136, 0.1);
}

.intro-text .eyebrow {
    font-size: 0.85rem;
    text-transform: uppercase;
    letter-spacing: 0.15em;
    color: #0d9488;
    font-weight: 600;
    margin-bottom: 0.75rem;
}

.intro-text h1 {
    font-size: 2.25rem;
    font-weight: 800;
    color: #0f172a;
    margin-bottom: 1.25rem;
    line-height: 1.2;
}

.intro-text p {
    font-size: 1.05rem;
    color: #334155;
    line-height: 1.75;
    margin-bottom: 1.5rem;
}

.intro-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
}

.intro-tags span {
    background: linear-gradient(135deg, rgba(13, 148, 136, 0.12), rgba(15, 118, 110, 0.12));
    color: #0d9488;
    padding: 0.5rem 1rem;
    border-radius: 20px;
    font-size: 0.9rem;
    font-weight: 500;
    border: 1px solid rgba(13, 148, 136, 0.2);
}

.intro-counters {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.5rem;
    margin-top: 2rem;
}

.counter-card {
    background: rgba(248, 250, 252, 0.9);
    border-radius: 16px;
    padding: 1.5rem;
    text-align: center;
    border: 1px solid rgba(13, 148, 136, 0.1);
    transition: all 0.3s ease;
}

.counter-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(13, 148, 136, 0.15);
    border-color: rgba(13, 148, 136, 0.3);
}

.counter-value {
    font-size: 2.5rem;
    font-weight: 800;
    background: linear-gradient(135deg, #0d9488, #0f766e);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.counter-label {
    font-size: 0.85rem;
    color: #64748b;
    margin-top: 0.5rem;
}

.section-header {
    margin-bottom: 2rem;
}

.section-header h2 {
    font-size: 1.75rem;
    font-weight: 700;
    color: #0f172a;
    position: relative;
    display: inline-block;
}

.section-header h2::after {
    content: '';
    position: absolute;
    bottom: -8px;
    left: 0;
    width: 60px;
    height: 3px;
    background: linear-gradient(90deg, #0d9488, #0f766e);
    border-radius: 2px;
}

.highlight-block {
    margin: 3rem 0;
}

.highlight-list {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

.highlight-card {
    display: flex;
    gap: 2rem;
    background: rgba(255, 255, 255, 0.9);
    border-radius: 20px;
    padding: 1.5rem;
    box-shadow: 0 10px 30px rgba(30, 41, 59, 0.08);
    transition: all 0.4s ease;
    border: 1px solid rgba(30, 41, 59, 0.05);
}

.highlight-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 20px 50px rgba(13, 148, 136, 0.12);
    border-color: rgba(13, 148, 136, 0.2);
}

.highlight-media {
    flex: 0 0 280px;
    position: relative;
}

.highlight-media img {
    width: 100%;
    border-radius: 12px;
    box-shadow: 0 8px 20px rgba(13, 148, 136, 0.1);
}

.highlight-media .badge {
    position: absolute;
    top: 12px;
    left: 12px;
    padding: 0.35rem 0.85rem;
    border-radius: 20px;
    font-size: 0.75rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.05em;
}

.badge-cyan {
    background: linear-gradient(135deg, #0d9488, #0891b2);
    color: white;
}

.badge-green {
    background: linear-gradient(135deg, #059669, #047857);
    color: white;
}

.badge-teal {
    background: linear-gradient(135deg, #0f766e, #115e59);
    color: white;
}

.highlight-content {
    flex: 1;
}

.highlight-content h3 {
    font-size: 1.25rem;
    font-weight: 700;
    color: #0f172a;
    margin-bottom: 0.75rem;
    line-height: 1.4;
}

.highlight-content .authors {
    font-size: 0.9rem;
    color: #64748b;
    margin-bottom: 0.75rem;
}

.highlight-content .summary {
    font-size: 0.95rem;
    color: #475569;
    line-height: 1.6;
    margin-bottom: 1rem;
}

.resource-list {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
}

.resource-list a {
    display: inline-flex;
    align-items: center;
    padding: 0.5rem 1rem;
    background: rgba(13, 148, 136, 0.1);
    color: #0d9488;
    border-radius: 8px;
    font-size: 0.85rem;
    font-weight: 500;
    transition: all 0.3s ease;
    border: 1px solid rgba(13, 148, 136, 0.2);
}

.resource-list a:hover {
    background: rgba(13, 148, 136, 0.2);
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(13, 148, 136, 0.2);
}

.timeline-block {
    margin: 3rem 0;
}

.timeline-heading {
    margin-bottom: 2rem;
}

.timeline-heading h2 {
    font-size: 1.75rem;
    font-weight: 700;
    color: #0f172a;
}

.timeline-list {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

.timeline-row {
    display: flex;
    gap: 1.5rem;
    background: rgba(255, 255, 255, 0.9);
    border-radius: 16px;
    padding: 1.5rem;
    box-shadow: 0 8px 24px rgba(30, 41, 59, 0.06);
    transition: all 0.3s ease;
    border-left: 4px solid transparent;
}

.timeline-row:hover {
    transform: translateX(8px);
    box-shadow: 0 12px 32px rgba(13, 148, 136, 0.1);
    border-left-color: #0d9488;
}

.timeline-meta {
    flex: 0 0 100px;
}

.meta-date {
    font-size: 0.85rem;
    font-weight: 600;
    color: #0d9488;
    background: rgba(13, 148, 136, 0.1);
    padding: 0.35rem 0.75rem;
    border-radius: 6px;
}

.timeline-body {
    flex: 1;
}

.timeline-body h3 {
    font-size: 1.1rem;
    font-weight: 600;
    color: #0f172a;
    margin-bottom: 0.5rem;
    line-height: 1.4;
}

.pub-prefix {
    font-weight: 700;
    color: #0d9488;
}

.timeline-authors {
    font-size: 0.9rem;
    color: #64748b;
    margin-bottom: 0.5rem;
}

.timeline-body p {
    font-size: 0.95rem;
    color: #475569;
    line-height: 1.5;
    margin-bottom: 0.75rem;
}

.resource-inline {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
}

.resource-inline a {
    font-size: 0.85rem;
    color: #0d9488;
    padding: 0.25rem 0.5rem;
    background: rgba(13, 148, 136, 0.08);
    border-radius: 4px;
    transition: all 0.2s ease;
}

.resource-inline a:hover {
    background: rgba(13, 148, 136, 0.15);
}

@media (max-width: 768px) {
    .highlight-card {
        flex-direction: column;
    }
    
    .highlight-media {
        flex: none;
    }
    
    .intro-counters {
        grid-template-columns: 1fr;
    }
    
    .timeline-row {
        flex-direction: column;
        gap: 0.75rem;
    }
    
    .timeline-meta {
        flex: none;
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

    <section class="highlight-block fade-in">
        <div class="section-header">
            <h2>Highlight Research</h2>
        </div>

        <div class="highlight-list">
            <article class="highlight-card">
                <div class="highlight-media">
                    <img src="https://alexlai2860.github.io/images/posterreward/concat.png" alt="PosterReward">
                    <span class="badge badge-cyan">CVPR 2026</span>
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
                    <span class="badge badge-cyan">CVPR 2026</span>
                </div>
                <div class="highlight-content">
                    <h3>PosterOmni — Generalized Artistic Poster Creation via Task Distillation and Unified Reward Feedback</h3>
                    <p class="authors">Sixiang Chen*, <strong><u>Jianyu Lai*</u></strong>, Jialin Gao*, Hengyu Shi*, Zhongying Liu*, Tian Ye, Junfeng Luo, Xiaoming Wei, Lei Zhu✉️</p>
                    <p class="summary">One model for poster creation—unifying local edits and global design for generalized multi-task image/poster-to-poster generation. ✨ Your intelligent assistant for high-quality aesthetic poster creation!</p>
                    <div class="resource-list">
                        <a href="https://arxiv.org/abs/2602.12127">📄 Paper</a>
                        <a href="https://ephemeral182.github.io/PosterOmni/">🌐 Project</a>
                        <a href="https://huggingface.co/MeiGen-AI/PosterOmni_v1">🤗 Model</a>
                        <a href="https://github.com/MeiGen-AI/PosterOmni">🐙 GitHub</a>
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
                        <a href="https://github.com/Ephemeral182/PosterCraft">🐙 GitHub</a>
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
