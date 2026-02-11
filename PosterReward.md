---
layout: posterreward
permalink: /PosterReward/
title: PosterReward - Unlocking Accurate Evaluation for High-Quality Graphic Design Generation
---

<div class="hero-section">
    <!-- Logo if available -->
    <img src="/images/posterreward/logo_svg.png" alt="PosterReward Logo" style="width: 100px; margin-bottom: 2rem; display: none;" onerror="this.style.display='none'">
    
    <h1 class="project-title">
        <span class="title-gradient">PosterReward</span>: Unlocking Accurate Evaluation for High-Quality Graphic Design Generation
    </h1>

    <div class="authors-container">
        <div class="author-list">
            <span class="author-name">Jianyu Lai<sup class="author-sup">1,2,*</sup></span>,
            <span class="author-name">Sixiang Chen<sup class="author-sup">1,2,*</sup></span>,
            <span class="author-name">Jialin Gao<sup class="author-sup">2,*</sup></span>,
            <span class="author-name">Hengyu Shi<sup class="author-sup">2</sup></span>,
            <span class="author-name">Zhongying Liu<sup class="author-sup">2</sup></span>,
            <span class="author-name">Fuxiang Zhai<sup class="author-sup">1</sup></span>,
            <span class="author-name">Junfeng Luo<sup class="author-sup">2</sup></span>,
            <span class="author-name">Xiaoming Wei<sup class="author-sup">2</sup></span>,
            <span class="author-name">Lujia Wang<sup class="author-sup">1</sup></span>,
            <span class="author-name">Lei Zhu<sup class="author-sup">1,3,†</sup></span>
        </div>
        
        <div class="affiliations">
            <span><sup class="author-sup">1</sup>HKUST(GZ)</span>
            <span><sup class="author-sup">2</sup>Meituan</span>
            <span><sup class="author-sup">3</sup>HKUST</span>
        </div>
    </div>

    <div style="margin-top: 2rem;">
        <a href="https://arxiv.org/abs/2501.11646" class="btn btn-primary"><span>📄</span> Paper</a>
        <a href="https://alexlai2860.github.io/PosterReward/" class="btn btn-secondary"><span>💻</span> Code</a>
        <a href="https://huggingface.co/PosterReward" class="btn btn-secondary"><span>🤗</span> Model</a>
    </div>
</div>

<div class="content-wrapper">

    <!-- Abstract -->
    <div style="max-width: 1000px; margin: 0 auto 6rem; background: rgba(255,255,255,0.6); padding: 3rem; border-radius: 24px; backdrop-filter: blur(10px); box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05);" id="abstract">
        <p style="font-size: 1.1rem; color: var(--text-secondary); line-height: 1.8; text-align: justify; margin-bottom: 1.5rem;">
            Recent advancements in the text-rendering capabilities of image generation models have made the end-to-end creation of graphic design content, such as posters, increasingly feasible. However, existing reward models fall short of accurately assessing design quality, as they primarily focus on global image aesthetics while overlooking the critical dimensions of typography and layout. Furthermore, the scarcity of domain-specific preference data remains a significant bottleneck, which limits the further development of graphic design evaluation and generation.
        </p>
        <p style="font-size: 1.1rem; color: var(--text-secondary); line-height: 1.8; text-align: justify;">
            To bridge this gap, we introduce an automated pipeline to construct a high-quality dataset of 70k poster preferences by leveraging the consensus of multiple Multi-modal Large Language Models (MLLMs) to simulate human-like judgment at scale. Utilizing this dataset, we develop <strong>PosterReward</strong>, a reward model specifically designed for high-precision poster assessment through a cascaded, multi-stage training strategy. We also provide multiple variants of the model to cater to different application scenarios. Finally, we introduce <strong>PosterRewardBench</strong> and <strong>PosterBench</strong> to evaluate the performance of existing reward models in poster assessment and the generation capabilities of current text-to-image models in poster creation, respectively.
        </p>
    </div>

    <style>
        .stacked-showcase {
            display: block;
            margin: 7rem 0;
        }
        .stacked-showcase .split-text {
            width: 100%;
            min-width: 0;
        }
        .v-media-stack {
            display: flex;
            flex-direction: column;
            gap: 1.4rem;
            margin-top: 2rem;
            width: 100%;
            max-width: 1240px;
        }
        .v-media-card {
            width: 100%;
            background: rgba(255, 255, 255, 0.65);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.7);
            border-radius: 18px;
            padding: 0.95rem;
            box-shadow: 0 12px 30px -12px rgba(0, 0, 0, 0.15);
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .v-media-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 20px 36px -14px rgba(0, 0, 0, 0.22);
        }
        .v-media-card img {
            width: 100%;
            border-radius: 12px;
            display: block;
            background: white;
            border: 1px solid rgba(0, 0, 0, 0.05);
        }
        .v-media-caption {
            margin-top: 0.9rem;
            color: var(--text-secondary);
            font-size: 0.92rem;
            line-height: 1.55;
            text-align: left;
        }
        .stacked-showcase .feature-list {
            display: grid;
            grid-template-columns: repeat(3, minmax(0, 1fr));
            gap: 1.2rem;
            margin-top: 1.8rem;
        }
        .stacked-showcase .feature-item {
            height: 100%;
        }
        @media (max-width: 1100px) {
            .stacked-showcase .feature-list {
                grid-template-columns: repeat(2, minmax(0, 1fr));
            }
        }
        @media (max-width: 768px) {
            .stacked-showcase .feature-list {
                grid-template-columns: 1fr;
            }
        }

        .model-eval-board {
            display: flex;
            flex-direction: column;
            gap: 1.2rem;
            margin-top: 2rem;
        }
        .model-eval-row {
            display: grid;
            grid-template-columns: 180px 1fr;
            gap: 1.2rem;
            align-items: stretch;
        }
        .model-left-card {
            background: rgba(255, 255, 255, 0.72);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.7);
            border-radius: 18px;
            padding: 1.1rem;
            box-shadow: 0 12px 30px -12px rgba(0, 0, 0, 0.15);
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .model-left-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 16px 36px -14px rgba(0, 0, 0, 0.2);
        }
        .model-left-name {
            font-weight: 700;
            font-size: 1.05rem;
            color: var(--text-main);
            margin-bottom: 0.45rem;
        }
        .model-left-desc {
            font-size: 0.9rem;
            color: var(--text-secondary);
            line-height: 1.45;
        }
        .eval-flow-card {
            background: rgba(255, 255, 255, 0.68);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.7);
            border-radius: 18px;
            padding: 1rem;
            box-shadow: 0 12px 30px -12px rgba(0, 0, 0, 0.15);
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .eval-flow-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 16px 36px -14px rgba(0, 0, 0, 0.2);
        }
        .flow-shared-prompt {
            background: rgba(15, 23, 42, 0.06);
            border: 1px solid rgba(15, 23, 42, 0.08);
            color: var(--text-main);
            border-radius: 12px;
            padding: 0.55rem 0.8rem;
            font-size: 0.88rem;
            margin-bottom: 0.8rem;
        }
        .flow-lane {
            display: flex;
            align-items: center;
            gap: 0.55rem;
            margin-bottom: 0.7rem;
            flex-wrap: wrap;
        }
        .flow-node {
            background: white;
            border: 1px solid rgba(0, 0, 0, 0.07);
            border-radius: 12px;
            padding: 0.5rem;
            box-shadow: 0 8px 22px -14px rgba(0, 0, 0, 0.25);
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .flow-node:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 28px -12px rgba(0, 0, 0, 0.35);
        }
        .flow-node img {
            width: 100%;
            height: auto;
            object-fit: cover;
            border-radius: 8px;
            display: block;
        }
        .flow-node-label {
            font-size: 0.74rem;
            color: var(--text-secondary);
            margin-top: 0.35rem;
            text-align: center;
        }
        .flow-text-node {
            min-width: 200px;
            max-width: 360px;
            color: var(--text-secondary);
            font-size: 0.83rem;
            line-height: 1.38;
            cursor: pointer;
        }
        .flow-text-node:hover { color: var(--primary); }
        .flow-text-node::after {
            content: " ⊞";
            font-size: 0.75em;
            opacity: 0.6;
        }
        .flow-score-node {
            min-width: 90px;
            text-align: center;
            font-weight: 700;
            font-size: 1.05rem;
            color: white;
            border: none;
        }
        .flow-score-high { background: linear-gradient(135deg, #16a34a, #22c55e); }
        .flow-score-low { background: linear-gradient(135deg, #f97316, #ef4444); }
        .flow-judge-node {
            min-width: 240px;
            max-width: 420px;
            color: var(--text-main);
            font-size: 0.86rem;
            line-height: 1.42;
            cursor: pointer;
        }
        .flow-judge-node:hover { color: var(--primary); }
        .flow-judge-node::after {
            content: " ⊞";
            font-size: 0.75em;
            opacity: 0.6;
        }
        .flow-arrow {
            color: #6366f1;
            font-weight: 700;
            font-size: 1.05rem;
            transition: opacity 0.2s ease;
        }
        .flow-arrow:hover { opacity: 1; }
        .flow-img-scroll {
            width: 200px;
            height: 220px;
            overflow-y: auto;
            overflow-x: hidden;
            border-radius: 12px;
            background: #f8fafc;
            border: 1px solid rgba(0, 0, 0, 0.08);
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .flow-img-scroll:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 28px -12px rgba(0, 0, 0, 0.25);
        }
        .flow-img-scroll::-webkit-scrollbar { width: 6px; }
        .flow-img-scroll::-webkit-scrollbar-thumb { background: #cbd5e1; border-radius: 3px; }
        .flow-img-scroll img {
            width: 100%;
            height: auto;
            display: block;
            border-radius: 0;
        }
        .flow-img-scroll img + img { border-top: 4px solid rgba(0,0,0,0.06); }
        .analysis-overlay {
            display: none;
            position: fixed;
            inset: 0;
            z-index: 9999;
            background: rgba(15, 23, 42, 0.92);
            align-items: center;
            justify-content: center;
            padding: 2rem;
        }
        .analysis-overlay.active { display: flex; }
        .analysis-overlay-content {
            max-width: 720px;
            max-height: 85vh;
            overflow-y: auto;
            background: rgba(255,255,255,0.95);
            color: var(--text-main);
            padding: 2rem;
            border-radius: 16px;
            font-size: 0.95rem;
            line-height: 1.7;
            box-shadow: 0 25px 50px rgba(0,0,0,0.3);
        }
        .analysis-overlay-close {
            position: absolute;
            top: 1.5rem;
            right: 1.5rem;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255,255,255,0.2);
            color: white;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            line-height: 1;
        }
        .analysis-overlay-close:hover { background: rgba(255,255,255,0.35); }
        .flow-dual-lane {
            display: grid;
            grid-template-columns: auto 1fr;
            gap: 0 0.6rem;
            align-items: center;
        }
        .flow-dual-lane .flow-img-scroll {
            grid-row: 1 / -1;
            align-self: stretch;
        }
        .flow-single-img {
            width: 140px;
            flex-shrink: 0;
        }
        .flow-single-img img {
            width: 100%;
            height: auto;
            max-height: 160px;
            object-fit: contain;
        }
        @media (max-width: 1100px) {
            .model-eval-row {
                grid-template-columns: 1fr;
            }
            .flow-dual-lane { grid-template-columns: 1fr; }
            .flow-dual-lane .flow-img-scroll { max-width: 100%; }
        }
    </style>

    <!-- Section 1: Capability Showcase -->
    <div class="split-section stacked-showcase" id="features">
        <div class="split-text">
            <span class="section-label">Capability Showcase</span>
            <h2 class="section-title">What is PosterReward and How the Three Models Respond</h2>
            <div class="model-eval-board">
                <div class="model-eval-row">
                    <div class="model-left-card">
                        <div class="model-left-name">PosterReward</div>
                        <p class="model-left-desc">Image + prompt are first analyzed, then mapped to scalar reward scores via the scoring module.</p>
                    </div>
                    <div class="eval-flow-card">
                        <div class="flow-shared-prompt"><strong>Shared Prompt:</strong> "Tokyo Landmark Check-In Tour — Discover Iconic Spots."</div>
                        <div class="flow-dual-lane">
                            <div class="flow-img-scroll">
                                <img src="/images/posterreward/p001_01_seed684633929_chosen.jpg" alt="Chosen poster">
                                <img src="/images/posterreward/p001_reject.png" alt="Rejected poster">
                            </div>
                            <div class="flow-lane">
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-text-node analysis-expand" data-full="Analysis (Chosen): Clean typography hierarchy, coherent skyline composition, and high instruction faithfulness. The chosen sample demonstrates superior text rendering and layout balance.">Analysis: clean typography hierarchy, coherent skyline composition, and high instruction faithfulness.</div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-score-node flow-score-high">20.0</div>
                            </div>
                            <div class="flow-lane" style="margin-bottom: 0;">
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-text-node analysis-expand" data-full="Analysis (Rejected): Text readability issues, awkward phrase generation, and weaker global visual balance. The rejected sample shows lower fidelity to the prompt and less polished typography.">Analysis: text readability issues, awkward phrase generation, and weaker global visual balance.</div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-score-node flow-score-low">5.0</div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="model-eval-row">
                    <div class="model-left-card">
                        <div class="model-left-name">PosterReward-Lite</div>
                        <p class="model-left-desc">A lightweight pointwise evaluator that predicts scores directly from image + prompt with minimal latency.</p>
                    </div>
                    <div class="eval-flow-card">
                        <div class="flow-shared-prompt"><strong>Shared Prompt:</strong> "Tokyo Landmark Check-In Tour — Discover Iconic Spots."</div>
                        <div class="flow-dual-lane">
                            <div class="flow-img-scroll">
                                <img src="/images/posterreward/p001_01_seed684633929_chosen.jpg" alt="Chosen poster">
                                <img src="/images/posterreward/p001_reject.png" alt="Rejected poster">
                            </div>
                            <div class="flow-lane">
                                <div class="flow-arrow">→</div>
                                <span style="font-size:0.87rem;color:var(--text-secondary);">Chosen</span>
                                <div class="flow-node flow-score-node flow-score-high">17.8</div>
                            </div>
                            <div class="flow-lane" style="margin-bottom: 0;">
                                <div class="flow-arrow">→</div>
                                <span style="font-size:0.87rem;color:var(--text-secondary);">Rejected</span>
                                <div class="flow-node flow-score-node flow-score-low">7.1</div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="model-eval-row">
                    <div class="model-left-card">
                        <div class="model-left-name">PosterReward-Pairwise</div>
                        <p class="model-left-desc">A pairwise judge that compares two candidates and outputs preference decisions with interpretable textual reasoning.</p>
                    </div>
                    <div class="eval-flow-card">
                        <div class="flow-shared-prompt"><strong>Shared Prompt:</strong> "Tokyo Landmark Check-In Tour — Discover Iconic Spots."</div>
                        <div class="flow-dual-lane">
                            <div class="flow-img-scroll">
                                <img src="/images/posterreward/p001_01_seed684633929_chosen.jpg" alt="Candidate A">
                                <img src="/images/posterreward/p001_reject.png" alt="Candidate B">
                            </div>
                            <div class="flow-lane" style="margin-bottom: 0;">
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-judge-node analysis-expand" data-full="Judgment: Prefer Candidate A (top image). Reasoning: Stronger text realism and semantic clarity. The chosen candidate shows cleaner typography hierarchy, coherent skyline composition, and higher instruction faithfulness. The rejected candidate exhibits text readability issues and weaker global visual balance.">Judgment: Prefer Candidate A. Reasoning highlights stronger text realism, clearer semantics, and better composition consistency.</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div id="analysis-overlay" class="analysis-overlay" onclick="if(event.target===this)this.classList.remove('active')">
        <button class="analysis-overlay-close" onclick="document.getElementById('analysis-overlay').classList.remove('active')" aria-label="Close">×</button>
        <div class="analysis-overlay-content" onclick="event.stopPropagation()"></div>
    </div>
    <script>
        (function(){
            document.querySelectorAll('.analysis-expand').forEach(function(el){
                el.addEventListener('click', function(){
                    var full = el.getAttribute('data-full') || el.textContent;
                    var overlay = document.getElementById('analysis-overlay');
                    overlay.querySelector('.analysis-overlay-content').textContent = full;
                    overlay.classList.add('active');
                });
            });
        })();
    </script>

    <!-- Section 2: Automated Preference Data Construction -->
    <div class="split-section stacked-showcase" id="data">
        <div class="split-text">
            <span class="section-label">Automated Preference Data Construction</span>
            <h2 class="section-title">From Large Raw Pools to Reliable Poster Preferences</h2>
            <div class="v-media-stack">
                <div class="v-media-card">
                    <img src="/images/posterreward/dataset_pipe.png" alt="Automated preference data collection pipeline">
                    <p class="v-media-caption">Automated AI-judged preference data pipeline with cascaded filtering, pair generation, and multi-model consensus validation.</p>
                </div>
                <div class="v-media-card">
                    <img src="/images/posterreward/dataset_examples.jpg" alt="Preference pair examples">
                    <p class="v-media-caption">Representative chosen-vs-rejected preference pairs, with dimensions such as aesthetics, text readability, layout coherence, and prompt alignment.</p>
                </div>
            </div>
            <div class="feature-list">
                <div class="feature-item">
                    <div class="number-badge">1</div>
                    <span class="feature-heading">Large-scale pool generation and staged filtering</span>
                    <p class="feature-desc">We build cinematic and non-cinematic sample pools from multiple generators, then progressively reduce noise using aesthetic scoring, similarity constraints, and stability checks before expensive model voting.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">2</div>
                    <span class="feature-heading">Consensus-based pair selection with bias control</span>
                    <p class="feature-desc">Preference labels are verified by multiple advanced MLLMs under order-swapped pairwise prompting, which suppresses positional bias and retains only stable, high-confidence comparisons.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">3</div>
                    <span class="feature-heading">Poster-Preference-70K</span>
                    <p class="feature-desc">The final dataset emphasizes typography, layout, and instruction faithfulness, addressing the underrepresentation of graphic design quality signals in general-purpose visual preference datasets.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Section 3: Unified Cascaded Training Framework -->
    <div class="split-section stacked-showcase" id="method">
        <div class="split-text">
            <span class="section-label">Unified Cascaded Training Framework</span>
            <h2 class="section-title">Jointly Optimizing Analysis, Pairwise Judgment, and Scoring</h2>
            <div class="v-media-stack">
                <div class="v-media-card">
                    <img src="/images/posterreward/training_framework.png" alt="PosterReward training framework">
                    <p class="v-media-caption">The complete cascaded framework that unifies discriminative and pairwise reward learning through SFT, rejection sampling, score-module optimization, and reinforcement fine-tuning.</p>
                </div>
            </div>
            <div class="feature-list">
                <div class="feature-item">
                    <div class="number-badge">1</div>
                    <span class="feature-heading">Joint SFT and rejection-sampling refinement</span>
                    <p class="feature-desc">Single-image analysis and paired-image comparison are trained together, then refined by rejection sampling to improve answer quality and preference consistency.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">2</div>
                    <span class="feature-heading">Score module training with pairwise supervision</span>
                    <p class="feature-desc">The scoring head is optimized on chosen/rejected triplets with Bradley-Terry loss, converting rich analysis into stable scalar reward differences.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">3</div>
                    <span class="feature-heading">RL-based analysis enhancement</span>
                    <p class="feature-desc">A GRPO stage improves analysis outputs while keeping the scorer frozen, making final rewards more robust for downstream post-training.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- Section 4: Application - Test Time Scaling and Graphic Design Evaluation -->
    <div class="table-container" id="results">
        <h2 style="text-align: center; margin-bottom: 0.8rem; font-family: 'Plus Jakarta Sans', sans-serif;">
            Application: Test Time Scaling & Graphic Design Evaluation
        </h2>
        <p style="text-align: center; color: var(--text-secondary); margin-bottom: 1.8rem; max-width: 980px; margin-left: auto; margin-right: auto;">
            PosterReward supports stronger decision quality at inference through richer analysis traces and demonstrates high agreement with design-centric quality criteria on poster generation benchmarks.
        </p>
        <div class="table-scroll-wrapper">
            <table class="results-table" id="posterbench-leaderboard">
                <thead>
                    <tr>
                        <th style="width: 28%; cursor: pointer;" data-sort-key="model">Model</th>
                        <th style="width: 18%; cursor: pointer;" data-sort-key="mean">Mean ↑</th>
                        <th style="width: 18%; cursor: pointer;" data-sort-key="median">Median ↑</th>
                        <th style="width: 18%; cursor: pointer;" data-sort-key="std">Std ↓</th>
                        <th style="width: 18%; cursor: pointer;" data-sort-key="top8">Best-of-8 Avg ↑</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td colspan="5" style="text-align: left; font-style: italic; color: var(--text-secondary);">Closed-Source Models</td>
                    </tr>
                    <tr>
                        <td>Nano-Banana</td>
                        <td><span class="rank-1">9.86</span></td>
                        <td>9.63</td>
                        <td><span class="rank-1">5.59</span></td>
                        <td>13.17</td>
                    </tr>
                    <tr>
                        <td>Seedream4.0</td>
                        <td>9.23</td>
                        <td><span class="rank-1">10.38</span></td>
                        <td>6.81</td>
                        <td><span class="rank-1">13.90</span></td>
                    </tr>
                    <tr>
                        <td>GPT-Image-1</td>
                        <td>6.57</td>
                        <td>6.72</td>
                        <td>6.04</td>
                        <td>11.73</td>
                    </tr>
                    <tr>
                        <td>Seedream3.0</td>
                        <td>2.21</td>
                        <td>1.93</td>
                        <td>7.13</td>
                        <td>8.40</td>
                    </tr>
                    <tr>
                        <td colspan="5" style="text-align: left; font-style: italic; color: var(--text-secondary);">Open-Source Models</td>
                    </tr>
                    <tr>
                        <td>Z-Image-Turbo</td>
                        <td>6.83</td>
                        <td>7.34</td>
                        <td>7.05</td>
                        <td>12.28</td>
                    </tr>
                    <tr>
                        <td>Qwen-Image-2512</td>
                        <td>6.83</td>
                        <td>7.34</td>
                        <td>7.05</td>
                        <td>12.28</td>
                    </tr>
                    <tr>
                        <td>Qwen-Image</td>
                        <td>6.83</td>
                        <td>7.34</td>
                        <td>7.05</td>
                        <td>12.28</td>
                    </tr>
                    <tr>
                        <td>Flux.1-dev</td>
                        <td>4.89</td>
                        <td>4.93</td>
                        <td>5.89</td>
                        <td>10.56</td>
                    </tr>
                    <tr>
                        <td>Flux-Krea</td>
                        <td>4.38</td>
                        <td>5.47</td>
                        <td>8.36</td>
                        <td>9.11</td>
                    </tr>
                    <tr>
                        <td>SD3.5-L</td>
                        <td>-2.19</td>
                        <td>-3.57</td>
                        <td>6.52</td>
                        <td>2.80</td>
                    </tr>
                </tbody>
            </table>
        </div>
        <p style="text-align: center; margin-top: 1.5rem; color: var(--text-secondary); font-size: 0.9rem;">
            PosterBench evaluation results. Higher Mean/Median/Best-of-8 indicate better average and scalable performance; lower Std indicates more stable quality across prompts.
        </p>
    </div>

    <!-- Section 5: Application - Reward Model in Post Training -->
    <div class="split-section stacked-showcase" id="posttraining">
        <div class="split-text">
            <span class="section-label">Application</span>
            <h2 class="section-title">Reward Model in Post Training</h2>
            <div class="feature-list">
                <div class="feature-item">
                    <div class="number-badge">1</div>
                    <span class="feature-heading">A practical reward source for RL alignment</span>
                    <p class="feature-desc">PosterReward provides dense, design-aware scalar feedback over typography, composition, and semantic faithfulness, making it suitable as a reward function in post-training loops for image generation systems.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">2</div>
                    <span class="feature-heading">Bridging pairwise preference and pointwise optimization</span>
                    <p class="feature-desc">The pairwise model improves preference reliability and interpretability, while the discriminative scorer supports efficient large-batch optimization, offering a unified path from data curation to policy improvement.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">3</div>
                    <span class="feature-heading">Transferable to diverse post-training scenarios</span>
                    <p class="feature-desc">Beyond benchmark ranking, the reward can guide rejection sampling, reranking, and reinforcement fine-tuning for poster generation, helping models move from generic aesthetics to task-specific design quality.</p>
                </div>
            </div>
        </div>
    </div>

    <script>
        (function () {
            const table = document.getElementById('posterbench-leaderboard');
            if (!table) return;

            const headers = Array.from(table.querySelectorAll('thead th'));
            const tbody = table.querySelector('tbody');

            function parseNumber(text) {
                const value = parseFloat(text.replace(/[^\d.-]/g, ''));
                return Number.isFinite(value) ? value : NaN;
            }

            function getCellValue(row, colIndex) {
                const cell = row.children[colIndex];
                if (!cell) return '';
                const text = cell.textContent.trim();
                return text;
            }

            function collectSections() {
                const rows = Array.from(tbody.querySelectorAll('tr'));
                const sections = [];
                let current = null;

                rows.forEach((row) => {
                    const firstCell = row.firstElementChild;
                    const isGroupRow = firstCell && firstCell.getAttribute('colspan');
                    if (isGroupRow) {
                        current = { header: row, rows: [] };
                        sections.push(current);
                    } else if (current) {
                        current.rows.push(row);
                    }
                });
                return sections;
            }

            function sortSectionRows(rows, colIndex, order, isNumeric) {
                const multiplier = order === 'asc' ? 1 : -1;
                rows.sort((a, b) => {
                    const aText = getCellValue(a, colIndex);
                    const bText = getCellValue(b, colIndex);

                    if (isNumeric) {
                        const aNum = parseNumber(aText);
                        const bNum = parseNumber(bText);
                        const aVal = Number.isFinite(aNum) ? aNum : -Infinity;
                        const bVal = Number.isFinite(bNum) ? bNum : -Infinity;
                        return (aVal - bVal) * multiplier;
                    }

                    return aText.localeCompare(bText) * multiplier;
                });
            }

            function applySort(colIndex, order) {
                const isNumeric = colIndex !== 0;
                const sections = collectSections();
                sections.forEach((section) => {
                    sortSectionRows(section.rows, colIndex, order, isNumeric);
                });

                const fragment = document.createDocumentFragment();
                sections.forEach((section) => {
                    fragment.appendChild(section.header);
                    section.rows.forEach((row) => fragment.appendChild(row));
                });
                tbody.appendChild(fragment);
            }

            headers.forEach((th, index) => {
                th.addEventListener('click', () => {
                    const currentOrder = th.getAttribute('data-sort-order') || 'desc';
                    const nextOrder = currentOrder === 'asc' ? 'desc' : 'asc';
                    headers.forEach((h) => h.removeAttribute('data-sort-order'));
                    th.setAttribute('data-sort-order', nextOrder);
                    applySort(index, nextOrder);
                });
            });

            applySort(1, 'desc');
        })();
    </script>

    <!-- Gallery Section -->
    <div style="margin-top: 8rem;">
        <h2 style="text-align: center; font-family: 'Plus Jakarta Sans', sans-serif; font-size: 2.5rem; margin-bottom: 3rem;">Gallery</h2>
        <div class="gallery-grid">
            <img src="/images/posterreward/case1.png" alt="Case 1" onerror="this.style.display='none'">
            <img src="/images/posterreward/case2.png" alt="Case 2" onerror="this.style.display='none'">
            <img src="/images/posterreward/case3.png" alt="Case 3" onerror="this.style.display='none'">
            <img src="/images/posterreward/case4.png" alt="Case 4" onerror="this.style.display='none'">
        </div>
    </div>

</div>
