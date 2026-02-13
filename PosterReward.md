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
        <a href="/mypaper/posterreward/PosterReward_Arxiv_official.pdf" class="btn btn-primary"><span>📄</span> Paper</a>
        <a href="https://alexlai2860.github.io/PosterReward/" class="btn btn-secondary"><span>💻</span> Code</a>
        <a href="https://huggingface.co/PosterReward" class="btn btn-secondary"><span>🤗</span> Model</a>
    </div>
</div>

<div class="content-wrapper">

    <!-- Abstract -->
    <div style="max-width: 1000px; margin: 0 auto 6rem; background: rgba(255,255,255,0.6); padding: 3rem; border-radius: 24px; backdrop-filter: blur(10px); box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05);" id="abstract">
        <p style="font-size: 1.1rem; color: var(--text-secondary); line-height: 1.8; text-align: justify; margin-bottom: 1.5rem;">
            Recent advancements in the text-rendering capabilities of image generation models have made the end-to-end creation of graphic design content, such as posters, increasingly feasible. However, existing reward models fall short of accurately assessing design quality, as they primarily focus on global image aesthetics while overlooking the critical dimensions of typography and layout. Furthermore, the scarcity of domain-specific preference data remains a significant bottleneck, limiting the further development of graphic design evaluation and generation.
        </p>
        <p style="font-size: 1.1rem; color: var(--text-secondary); line-height: 1.8; text-align: justify;">
            To bridge this gap, we design an automated pipeline to construct a high-quality dataset of 70k poster preferences by leveraging the consensus of multiple Multi-modal Large Language Models (MLLMs) to simulate human-like judgment. Based on this dataset, we propose <strong>PosterReward</strong>, a reward model specifically designed for high-precision poster assessment through a cascaded, multi-stage training strategy. We also provide multiple variants of the model to cater to different application scenarios. Finally, we introduce <strong>PosterRewardBench</strong> and <strong>PosterBench</strong> to evaluate the performance of existing reward models in poster assessment and the generation capabilities of current text-to-image models in poster creation, respectively.
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
        .model-left-name .title-gradient { font-weight: 700; }
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
            min-width: 260px;
            max-width: 460px;
            min-height: 118px;
            color: var(--text-secondary);
            font-size: 0.83rem;
            line-height: 1.45;
            cursor: pointer;
            display: -webkit-box;
            -webkit-line-clamp: 6;
            -webkit-box-orient: vertical;
            overflow: hidden;
            position: relative;
            padding-bottom: 1.65rem;
        }
        .flow-text-node:hover { color: var(--primary); }
        .flow-text-node::after {
            content: "... Click to view full analysis ↗";
            position: absolute;
            right: 0.55rem;
            bottom: 0.4rem;
            font-size: 0.73rem;
            line-height: 1;
            color: #475569;
            background: rgba(241, 245, 249, 0.96);
            padding: 0.2rem 0.42rem;
            border-radius: 6px;
            border: 1px solid rgba(148, 163, 184, 0.35);
            pointer-events: none;
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
            position: relative;
            padding-bottom: 1.6rem;
        }
        .flow-judge-node:hover { color: var(--primary); }
        .flow-judge-node::after {
            content: "... Click to view full analysis ↗";
            position: absolute;
            right: 0.55rem;
            bottom: 0.4rem;
            font-size: 0.73rem;
            line-height: 1;
            color: #475569;
            background: rgba(241, 245, 249, 0.96);
            padding: 0.2rem 0.42rem;
            border-radius: 6px;
            border: 1px solid rgba(148, 163, 184, 0.35);
            pointer-events: none;
        }
        .analysis-key-highlight {
            color: #ea580c;
            font-weight: 700;
        }
        .flow-arrow {
            color: #6366f1;
            font-weight: 700;
            font-size: 1.05rem;
            transition: opacity 0.2s ease;
        }
        .flow-arrow:hover { opacity: 1; }
        .flow-chunk-scroll {
            width: calc(100% + 1.15rem);
            max-width: none;
            height: 320px;
            overflow-y: scroll;
            overflow-x: hidden;
            margin-top: 0.5rem;
            margin-right: -1.15rem;
            overscroll-behavior-y: contain;
            direction: ltr;
            scrollbar-gutter: stable;
        }
        .flow-chunk-scroll::-webkit-scrollbar { width: 8px; }
        .flow-chunk-scroll::-webkit-scrollbar-thumb { background: #94a3b8; border-radius: 4px; }
        .flow-chunk-scroll::-webkit-scrollbar-track { background: rgba(0,0,0,0.04); border-radius: 4px; }
        .flow-chunk {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            margin-bottom: 1.2rem;
            padding: 0.8rem 0;
            flex-shrink: 0;
            border-bottom: 1px solid rgba(0,0,0,0.06);
        }
        .flow-chunk:last-child { margin-bottom: 0; border-bottom: none; }
        .flow-chunk .flow-node { flex-shrink: 0; }
        .flow-chunk .img-wrap {
            width: 300px;
            flex-shrink: 0;
            cursor: pointer;
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .flow-chunk .img-wrap:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px -8px rgba(0,0,0,0.3);
        }
        .flow-chunk .img-wrap img {
            width: 100%;
            height: auto;
            display: block;
        }
        .flow-lite-row {
            display: flex;
            gap: 5rem;
            flex-wrap: wrap;
            justify-content: space-around;
        }
        .flow-lite-row .flow-lane { margin-bottom: 0; }
        .flow-lite-row .img-wrap,
        .flow-pairwise-row .img-wrap,
        .flow-pairwise-imgs .img-wrap {
            cursor: pointer;
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.25s ease, box-shadow 0.25s ease;
        }
        .flow-lite-row .img-wrap:hover,
        .flow-pairwise-row .img-wrap:hover,
        .flow-pairwise-imgs .img-wrap:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px -8px rgba(0,0,0,0.3);
        }
        .flow-lite-row .img-wrap { width: 300px; }
        .flow-lite-row .img-wrap img { width: 100%; height: auto; display: block; }
        .flow-pairwise-row {
            display: flex;
            align-items: center;
            gap: 0.6rem;
            flex-wrap: wrap;
        }
        .flow-pairwise-row .img-wrap { width: 300px; }
        .flow-pairwise-row .img-wrap img { width: 100%; height: auto; display: block; }
        .flow-pairwise-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 0.85rem;
            align-items: start;
        }
        .flow-pairwise-main {
            display: grid;
            grid-template-columns: minmax(440px, 1fr) auto minmax(300px, 1fr);
            gap: 0.85rem;
            align-items: center;
        }
        .flow-pairwise-imgs {
            display: flex;
            align-items: center;
            gap: 0.7rem;
            flex-wrap: nowrap;
        }
        .flow-pairwise-imgs .img-wrap { width: 230px; min-width: 180px; flex-shrink: 0; }
        .flow-pairwise-imgs .img-wrap img { width: 100%; height: auto; display: block; }
        .flow-pairwise-question {
            background: rgba(15, 23, 42, 0.06);
            border: 1px solid rgba(15, 23, 42, 0.08);
            color: var(--text-secondary);
            border-radius: 12px;
            padding: 0.6rem 0.9rem;
            font-size: 0.88rem;
            line-height: 1.4;
        }
        .flow-pairwise-right {
            min-width: 300px;
            max-width: 100%;
        }
        @media (max-width: 900px) {
            .flow-pairwise-main {
                grid-template-columns: 1fr;
                gap: 0.65rem;
            }
            .flow-pairwise-imgs {
                flex-wrap: wrap;
                justify-content: center;
            }
        }
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
            white-space: pre-wrap;
        }
        .analysis-overlay-content .analysis-strong {
            font-weight: 700;
            color: #111827;
        }
        .analysis-overlay-content .analysis-key-highlight {
            color: #ea580c;
            font-weight: 700;
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
        .rank-1 {
            display: inline-block;
            padding: 0.1rem 0.38rem;
            border-radius: 6px;
            font-weight: 700;
            color: #92400e;
            background: rgba(251, 191, 36, 0.22);
            border: 1px solid rgba(251, 191, 36, 0.45);
        }
        .rank-2 {
            display: inline-block;
            padding: 0.1rem 0.38rem;
            border-radius: 6px;
            font-weight: 600;
            color: #1e40af;
            background: rgba(147, 197, 253, 0.35);
            border: 1px solid rgba(96, 165, 250, 0.5);
        }
        .bench-group-row td {
            text-align: left;
            font-style: normal;
            font-weight: 600;
            color: #475569;
            background: rgba(148, 163, 184, 0.08);
            padding-left: 1rem;
            white-space: nowrap;
        }
        .img-overlay {
            display: none;
            position: fixed;
            inset: 0;
            z-index: 9998;
            background: rgba(15, 23, 42, 0.95);
            align-items: center;
            justify-content: center;
            padding: 2rem;
        }
        .img-overlay.active { display: flex; }
        .img-overlay img {
            max-width: 95vw;
            max-height: 95vh;
            object-fit: contain;
            border-radius: 8px;
            box-shadow: 0 25px 50px rgba(0,0,0,0.5);
        }
        .img-overlay-close {
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
        .img-overlay-close:hover { background: rgba(255,255,255,0.35); }
        @media (max-width: 1100px) {
            .model-eval-row { grid-template-columns: 1fr; }
            .flow-chunk-scroll { max-width: 100%; }
        }
    </style>

    <!-- Section 1: Capability Showcase -->
    <div class="split-section stacked-showcase" id="features">
        <div class="split-text">
            <span class="section-label">Capability Showcase</span>
            <h2 class="section-title">What is PosterReward</h2>
            <div class="model-eval-board">
                <div class="model-eval-row">
                    <div class="model-left-card">
                        <div class="model-left-name"><span class="title-gradient">PosterReward</span></div>
                        <p class="model-left-desc">Image + prompt are first analyzed, then mapped to scalar reward scores via the scoring module.</p>
                    </div>
                    <div class="eval-flow-card">
                        <div class="flow-shared-prompt"><strong>Shared Prompt:</strong> "A serene minimalist poster with Japanese negative space, showcasing a pagoda, skyscraper, cherry blossom tree, and stone lantern in a quiet urban park. At the top is the title "Tokyo Landmark Check-In Tour", and below the tree is the text "Discover Iconic Spots"."</div>
                        <div class="flow-chunk-scroll" id="posterreward-scroll" tabindex="0">
                            <div class="flow-chunk">
                                <div class="img-wrap img-zoomable" data-src="/images/posterreward/p001_01_seed684633929_chosen.jpg">
                                    <img src="/images/posterreward/p001_01_seed684633929_chosen.jpg" alt="Chosen poster">
                                </div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-text-node analysis-expand" data-full="Analysis (Chosen):&#10;&#10;**Image Analysis**&#10;&#10;**1. Fundamental Image Integrity:**&#10;The image exhibits excellent fundamental integrity. As a digital illustration, it is free from technical flaws like pixelation, unintended blur, or digital noise. The lines are crisp, and the color fields are solid and clean, consistent with a high-quality vector-style graphic. There are no signs of over or underexposure; the lighting is intentionally flat and even, which is appropriate for the minimalist poster style. The overall technical quality is professional and flawless.&#10;&#10;**2. AI Artifact and Realism Evaluation:**&#10;The image is exceptionally clean of common AI artifacts. The illustrative style is cohesive and consistently applied across all elements. The pagoda, skyscraper, cherry blossom tree, and stone lantern are all well-formed without any of the typical AI-generated distortions, such as illogical merging of objects or misshapen geometry. The simplified, graphic representation of the blossoms and leaves is a deliberate stylistic choice, not an artifact. The image successfully maintains its intended aesthetic without any disruptive elements that would break the illusion of a polished, human-made graphic design.&#10;&#10;**3. Typographical Precision Analysis:**&#10;The typographical execution is precise and fully compliant with the prompt. The title, &quot;Tokyo Landmark Check-In Tour,&quot; is correctly spelled, capitalized, and positioned at the top. The subtitle, &quot;Discover Iconic Spots,&quot; is also rendered accurately and placed below the central cherry blossom tree as specified. A clean, modern sans-serif font is used for both, ensuring excellent legibility. The scale difference between the title and subtitle creates a clear visual hierarchy. The text is seamlessly integrated into the composition, appearing as an intentional design element rather than an overlay.&#10;&#10;**4. Visual Prompt Interpretation:**&#10;The image is a masterful interpretation of the prompt. It successfully captures the &quot;serene minimalist poster&quot; aesthetic through its clean lines and muted color palette. The concept of &quot;Japanese negative space&quot; is well-realized, with ample empty space in the upper half that allows the title to breathe and draws focus to the key visual elements. All four specified landmarks—pagoda, skyscraper, cherry blossom tree, and stone lantern—are present and clearly depicted. The setting of a &quot;quiet urban park&quot; is effectively conveyed by blending traditional Japanese architecture with a modern city skyline in the background. The composition adheres perfectly to the layout instructions, creating a balanced and thematically coherent scene.&#10;&#10;**5. Standalone Artistic Evaluation:**&#10;Viewed independently of the prompt, this is a highly effective and aesthetically pleasing piece of graphic art. The composition is strong, using a central focal point (the cherry blossom tree) balanced by elements on the left and right, creating a harmonious visual flow. The color palette is sophisticated and calming, using a limited range of blues, greys, and a soft pink to evoke a tranquil mood. The use of negative space is excellent, giving the image a modern, uncluttered feel. The stylized, flat-shaded approach to light and shadow adds depth without compromising the minimalist aesthetic. It is a compelling, well-crafted image that successfully communicates a sense of peace and discovery.">Analysis (Chosen): <span class="analysis-key-highlight">The image exhibits excellent fundamental integrity.</span> As a digital illustration, it is free from technical flaws like pixelation, unintended blur, or digital noise.</div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-score-node flow-score-high">17.38</div>
                            </div>
                            <div class="flow-chunk">
                                <div class="img-wrap img-zoomable" data-src="/images/posterreward/p001_reject.png">
                                    <img src="/images/posterreward/p001_reject.png" alt="Rejected poster">
                                </div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-text-node analysis-expand" data-full="Analysis (Rejected):&#10;&#10;**Image Analysis**&#10;&#10;**1. Fundamental Image Integrity:**&#10;The image exhibits strong fundamental quality. It is sharp, well-resolved, and free from distracting digital noise, pixelation, or compression artifacts. The lighting is soft and evenly distributed, avoiding any harsh overexposure or deep, underexposed shadows that would obscure detail. The overall technical execution provides a clean and professional foundation, with no objective flaws that detract from its clarity or impact.&#10;&#10;**2. AI Artifact and Realism Evaluation:**&#10;The image presents a high degree of realism, but minor AI artifacts are present upon close inspection. The architecture of the pagoda and skyscraper is coherent and structurally sound. However, the carvings on the stone lantern are indistinct and appear as repetitive, slightly garbled patterns rather than legible characters. The texture of the grass in the foreground is somewhat uniform and lacks natural variation. The cherry blossoms on the tree, while beautiful, have a slightly soft, painterly quality that blurs the line between photorealism and digital art. These subtle artifacts do not significantly disrupt the overall illusion but mark it as a generated image.&#10;&#10;**3. Typographical Precision Analysis:**&#10;The typographical execution is a mixed success. The image correctly renders the main title, &quot;Tokyo Landmark Check-In Tour,&quot; at the top in a clean, bold, black sans-serif font. It also accurately includes the secondary text, &quot;Discover Iconic Spots.,&quot; below the tree in a legible white font. However, a significant flaw is the inclusion of extraneous, nonsensical text—&quot;Landmark Uleevpa.&quot;—directly below the main title. This appears to be a failed attempt by the AI to generate a subtitle, and it severely undermines the poster's professionalism and adherence to the prompt.&#10;&#10;**4. Visual Prompt Interpretation:**&#10;The image successfully interprets most of the prompt's core visual directives. It effectively showcases the four specified elements: a pagoda, a skyscraper, a cherry blossom tree, and a stone lantern, all within a &quot;quiet urban park&quot; setting. The juxtaposition of the traditional and modern architecture perfectly captures the &quot;urban park&quot; concept. The composition, while not strictly minimalist, uses negative space in the upper half to create a clean, uncluttered poster feel. The overall mood is serene and contemplative, aligning with the prompt's intent. The primary deviation is the failure to adhere strictly to a &quot;minimalist&quot; style, which is a common challenge for AI in combining multiple complex subjects.&#10;&#10;**5. Standalone Artistic Evaluation:**&#10;As a standalone piece, the image is aesthetically compelling and well-composed. The composition uses a strong diagonal line, guiding the viewer's eye from the pagoda on the left, across the central cherry blossom tree, to the lantern on the right. This creates a balanced and dynamic visual flow. The use of atmospheric perspective, with the background skyscrapers fading into the haze, adds a convincing sense of depth. The color palette is harmonious, contrasting the cool blues of the sky and modern buildings with the warm, earthy tones of the traditional architecture and the soft pink of the blossoms. The image successfully evokes a feeling of peaceful discovery and the beautiful coexistence of nature and city.">Analysis (Rejected): The image exhibits strong fundamental quality. <span class="analysis-key-highlight">However, a significant flaw is the inclusion of extraneous, nonsensical text—"Landmark Uleevpa."—directly below the main title.</span></div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-score-node flow-score-low">1.15</div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="model-eval-row">
                    <div class="model-left-card">
                        <div class="model-left-name"><span class="title-gradient">PosterReward</span>-Lite</div>
                        <p class="model-left-desc">A lightweight pointwise evaluator that predicts scores directly from image + prompt with minimal latency.</p>
                    </div>
                    <div class="eval-flow-card">
                        <div class="flow-shared-prompt"><strong>Shared Prompt:</strong> "A serene minimalist poster with Japanese negative space, showcasing a pagoda, skyscraper, cherry blossom tree, and stone lantern in a quiet urban park. At the top is the title "Tokyo Landmark Check-In Tour", and below the tree is the text "Discover Iconic Spots"."</div>
                        <div class="flow-lite-row">
                            <div class="flow-lane">
                                <div class="img-wrap img-zoomable" data-src="/images/posterreward/p001_01_seed684633929_chosen.jpg">
                                    <img src="/images/posterreward/p001_01_seed684633929_chosen.jpg" alt="Chosen poster">
                                </div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-score-node flow-score-high">14.38</div>
                            </div>
                            <div class="flow-lane">
                                <div class="img-wrap img-zoomable" data-src="/images/posterreward/p001_reject.png">
                                    <img src="/images/posterreward/p001_reject.png" alt="Rejected poster">
                                </div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-node flow-score-node flow-score-low">-1.66</div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="model-eval-row">
                    <div class="model-left-card">
                        <div class="model-left-name"><span class="title-gradient">PosterReward</span>-Pairwise</div>
                        <p class="model-left-desc">A pairwise judge that compares two candidates and outputs preference decisions with interpretable textual reasoning.</p>
                    </div>
                    <div class="eval-flow-card">
                        <div class="flow-shared-prompt"><strong>Shared Prompt:</strong> "A serene minimalist poster with Japanese negative space, showcasing a pagoda, skyscraper, cherry blossom tree, and stone lantern in a quiet urban park. At the top is the title "Tokyo Landmark Check-In Tour", and below the tree is the text "Discover Iconic Spots"."</div>
                        <div class="flow-pairwise-grid">
                            <div class="flow-pairwise-main">
                                <div class="flow-pairwise-imgs">
                                    <div class="img-wrap img-zoomable" data-src="/images/posterreward/p001_01_seed684633929_chosen.jpg">
                                        <img src="/images/posterreward/p001_01_seed684633929_chosen.jpg" alt="Image 1">
                                    </div>
                                    <div class="img-wrap img-zoomable" data-src="/images/posterreward/p001_reject.png">
                                        <img src="/images/posterreward/p001_reject.png" alt="Image 2">
                                    </div>
                                </div>
                                <div class="flow-arrow">→</div>
                                <div class="flow-pairwise-right">
                                    <div class="flow-node flow-judge-node analysis-expand" data-full="Yes.&#10;&#10;Image 1 is significantly better than Image 2 primarily due to its superior adherence to the &quot;serene minimalist poster with Japanese negative space&quot; aesthetic and its flawless text rendering. Image 1 perfectly captures the requested minimalist style with its clean lines, simplified forms, and ample negative space, creating a tranquil and cohesive design that aligns with the prompt's core artistic direction. In contrast, Image 2 adopts a realistic, photographic style that completely misses the &quot;minimalist&quot; and &quot;Japanese negative space&quot; requirements, making it less aligned with the prompt's aesthetic vision. Furthermore, Image 1 accurately renders all requested text without any AI artifacts, whereas Image 2 includes an extraneous, garbled line of text (&quot;Landmark Ueeepan.&quot;) below the main title, which is a clear AI artifact and detracts from its overall quality and prompt adherence.">Yes.<br><br><span class="analysis-key-highlight">Image 1 is significantly better than Image 2 primarily due to its superior adherence to the "serene minimalist poster with Japanese negative space" aesthetic and its flawless text rendering.</span></div>
                                </div>
                            </div>
                            <div class="flow-pairwise-question">Is Image 1 better than Image 2? Please answer Yes or No first, then provide the reason.</div>
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
    <div id="img-overlay" class="img-overlay" onclick="if(event.target===this)this.classList.remove('active')">
        <button class="img-overlay-close" onclick="document.getElementById('img-overlay').classList.remove('active')" aria-label="Close">×</button>
        <img src="" alt="Enlarged" onclick="event.stopPropagation()">
    </div>
    <script>
        (function(){
            function escapeHtml(str) {
                return str
                    .replace(/&/g, '&amp;')
                    .replace(/</g, '&lt;')
                    .replace(/>/g, '&gt;')
                    .replace(/"/g, '&quot;')
                    .replace(/'/g, '&#39;');
            }
            function highlightMeaningfulSentences(html) {
                var sentenceSignal = /(significantly better|superior adherence|flawless text rendering|significant flaw|extraneous,?\s+nonsensical text|extraneous,?\s+garbled line of text|clear ai artifact|minor ai artifacts?|failed attempt|severely undermines|completely misses|excellent fundamental integrity|strong fundamental quality|free from technical flaws|fully compliant|typographical execution is precise|typographical execution is a mixed success)/i;
                var maxHighlights = 6;
                var highlightCount = 0;
                var lines = html.split('\n');
                return lines.map(function(line) {
                    var trimmed = line.trim();
                    if (!trimmed || trimmed.indexOf('@@B') !== -1) return line;
                    var sentences = line.match(/[^.!?]+[.!?]?/g);
                    if (!sentences) return line;
                    return sentences.map(function(sentence) {
                        var part = sentence.trim();
                        if (!part) return sentence;
                        if (highlightCount < maxHighlights && sentenceSignal.test(part)) {
                            highlightCount += 1;
                            return '<span class="analysis-key-highlight">' + part + '</span>';
                        }
                        return part;
                    }).join(' ');
                }).join('\n');
            }
            function formatAnalysisContent(raw) {
                var html = escapeHtml(raw || '');
                var boldTokens = [];
                html = html.replace(/\*\*(.*?)\*\*/g, function(_, txt) {
                    var token = '@@B' + boldTokens.length + '@@';
                    boldTokens.push('<strong class="analysis-strong">' + txt + '</strong>');
                    return token;
                });
                html = highlightMeaningfulSentences(html);
                boldTokens.forEach(function(block, idx) {
                    var tokenRe = new RegExp('@@B' + idx + '@@', 'g');
                    html = html.replace(tokenRe, block);
                });
                return html.replace(/\n/g, '<br>');
            }
            document.querySelectorAll('.analysis-expand').forEach(function(el){
                el.addEventListener('click', function(){
                    var full = el.getAttribute('data-full') || el.textContent;
                    var overlay = document.getElementById('analysis-overlay');
                    overlay.querySelector('.analysis-overlay-content').innerHTML = formatAnalysisContent(full);
                    overlay.classList.add('active');
                });
            });
            document.querySelectorAll('.img-zoomable').forEach(function(el){
                el.addEventListener('click', function(){
                    var src = el.getAttribute('data-src') || el.querySelector('img')?.src;
                    if (src) {
                        var overlay = document.getElementById('img-overlay');
                        overlay.querySelector('img').src = src;
                        overlay.classList.add('active');
                    }
                });
            });
            var scrollEl = document.getElementById('posterreward-scroll');
            if (scrollEl) {
                scrollEl.addEventListener('wheel', function(e) {
                    var top = this.scrollTop, h = this.clientHeight, sh = this.scrollHeight;
                    if ((e.deltaY > 0 && top < sh - h - 1) || (e.deltaY < 0 && top > 1)) {
                        e.preventDefault();
                        this.scrollTop += e.deltaY;
                    }
                }, { passive: false });
            }
        })();
    </script>

    <!-- Section 2: Automated Preference Data Construction -->
    <div class="split-section stacked-showcase" id="data">
        <div class="split-text">
            <span class="section-label">Automated Preference Data Construction</span>
            <h2 class="section-title">From Raw Image Pools to Reliable Preferences Dataset</h2>
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
            <h2 class="section-title">Pairwise and Pointwise Joint Training Framework</h2>
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

    <!-- Section 4: Experiments -->
    <div class="split-section stacked-showcase" id="experiments">
        <div class="split-text">
            <span class="section-label">Experiments</span>
            <h2 class="section-title">Experimental Results</h2>
            
            <!-- 对比实验 -->
            <div style="margin-bottom: 5rem;">
                <h3 style="text-align: center; margin-bottom: 1.5rem; font-size: 1.3rem; color: var(--text-main);">Main Comparisons</h3>
                <p style="text-align: center; color: var(--text-secondary); margin-bottom: 3rem; max-width: 900px; margin-left: auto; margin-right: auto;">
                    We evaluate PosterReward against existing reward models on poster assessment tasks, demonstrating superior performance in both pointwise accuracy and pairwise preference prediction.
                </p>

                <!-- Pointwise Reward Models -->
                <div class="v-media-card" style="margin-bottom: 2rem;">
                    <h4 style="text-align: center; margin-bottom: 1.2rem; font-size: 1.1rem; color: var(--text-secondary);">Pointwise Reward Models</h4>
                    <p style="text-align: center; color: var(--text-secondary); margin-bottom: 1.5rem; font-size: 0.95rem;">
                        Performance comparison across various benchmarks. All values represent accuracy (↑). PRB is an abbreviation for PosterRewardBench.
                    </p>
                    <div class="table-scroll-wrapper">
                        <table class="results-table" style="max-width: 900px; margin: 0 auto;">
                            <thead>
                                <tr>
                                    <th>Model</th>
                                    <th>MMRB2</th>
                                    <th>HPDv3</th>
                                    <th>PRB-Basic</th>
                                    <th>PRB-Ad</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>ImageReward</td>
                                    <td>53.0</td>
                                    <td>58.6</td>
                                    <td>60.7</td>
                                    <td>49.3</td>
                                </tr>
                                <tr>
                                    <td>PickScore</td>
                                    <td>57.6</td>
                                    <td>65.6</td>
                                    <td>66.7</td>
                                    <td>44.1</td>
                                </tr>
                                <tr>
                                    <td>HPSv2</td>
                                    <td>55.0</td>
                                    <td>65.3</td>
                                    <td>70.8</td>
                                    <td>43.7</td>
                                </tr>
                                <tr>
                                    <td>UnifiedReward*</td>
                                    <td>56.9</td>
                                    <td>59.4</td>
                                    <td>60.0</td>
                                    <td>52.7</td>
                                </tr>
                                <tr>
                                    <td>HPSv3</td>
                                    <td>58.5</span></td>
                                    <td>76.9</span></td>
                                    <td>72.9</span></td>
                                    <td>41.2</td>
                                </tr>
                                <tr>
                                    <td><strong>PosterReward-Lite</strong></td>
                                    <td><span class="rank-1">60.5</span></td>
                                    <td><span class="rank-2">77.1</span></td>
                                    <td><span class="rank-2">83.9</span></td>
                                    <td><span class="rank-2">85.0</span></td>
                                </tr>
                                <tr>
                                    <td><strong>PosterReward</strong></td>
                                    <td><span class="rank-2">59.6</span></td>
                                    <td><span class="rank-1">77.8</span></td>
                                    <td><span class="rank-1">86.7</span></td>
                                    <td><span class="rank-1">86.0</span></td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>

                <!-- Pairwise Reward Models -->
                <div class="v-media-card" style="margin-bottom: 3rem;">
                    <h4 style="text-align: center; margin-bottom: 1.2rem; font-size: 1.1rem; color: var(--text-secondary);">Pairwise Reward Models</h4>
                    <p style="text-align: center; color: var(--text-secondary); margin-bottom: 1.5rem; font-size: 0.95rem;">
                        Performance comparison on PosterRewardBench (PRB). "Yes" and "No" refer to the accuracy on samples with positive and negative ground truth labels, respectively.
                    </p>
                    <div class="table-scroll-wrapper">
                        <table class="results-table" style="max-width: 900px; margin: 0 auto;">
                            <thead>
                                <tr>
                                    <th>Model</th>
                                    <th colspan="3">PRB-Basic Acc. ↑</th>
                                    <th colspan="3">PRB-Ad Acc. ↑</th>
                                </tr>
                                <tr style="font-size: 0.9rem;">
                                    <th></th>
                                    <th>Yes</th>
                                    <th>No</th>
                                    <th>Avg.</th>
                                    <th>Yes</th>
                                    <th>No</th>
                                    <th>Avg.</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>UnifiedReward-think</td>
                                    <td>75.1</td>
                                    <td>61.5</td>
                                    <td>68.3</td>
                                    <td>52.6</td>
                                    <td>48.5</td>
                                    <td>50.6</td>
                                </tr>
                                <tr>
                                    <td>Qwen3-VL-Plus</td>
                                    <td>89.9</td>
                                    <td>39.2</td>
                                    <td>64.5</td>
                                    <td>98.7</td>
                                    <td>14.2</td>
                                    <td>56.4</td>
                                </tr>
                                <tr>
                                    <td>Gemini-2.5-Flash</td>
                                    <td>94.7</td>
                                    <td>33.3</td>
                                    <td>64.0</td>
                                    <td>95.2</td>
                                    <td>28.8</td>
                                    <td>62.0</td>
                                </tr>
                                <tr>
                                    <td>Gemini-2.5-Pro</td>
                                    <td>75.6</td>
                                    <td>83.1</td>
                                    <td>79.3</td>
                                    <td>81.8</td>
                                    <td>68.6</td>
                                    <td>75.2</td>
                                </tr>
                                <tr>
                                    <td>GPT-5</td>
                                    <td>90.4</td>
                                    <td>80.5</td>
                                    <td><span class="rank-1">85.4</span></td>
                                    <td>89.8</td>
                                    <td>75.9</td>
                                    <td><span class="rank-2">82.9</span></td>
                                </tr>
                                <tr>
                                    <td><strong>PosterReward-Pairwise</strong></td>
                                    <td>82.0</td>
                                    <td>84.0</td>
                                    <td><span class="rank-2">83.0</span></td>
                                    <td>84.1</td>
                                    <td>83.6</td>
                                    <td><span class="rank-1">83.8</span></td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>

            <!-- User Study on Analysis Module -->
            <div style="margin-bottom: 4rem;">
                <h3 style="text-align: center; margin-bottom: 1.5rem; font-size: 1.3rem; color: var(--text-main);">User Study on Analysis Module</h3>
                <p style="text-align: center; color: var(--text-secondary); margin-bottom: 2rem; max-width: 900px; margin-left: auto; margin-right: auto;">
                    Human evaluation demonstrates the progressive improvement of our cascaded training strategy.
                </p>
                <div class="v-media-card" style="max-width: 900px; margin: 0 auto;">
                    <img src="/images/posterreward/comparison_plot_gemini3flash_v2.png" alt="User study on analysis module" style="width: 100%; border-radius: 12px; display: block;">
                    <p class="v-media-caption" style="margin-top: 1rem; text-align: center;">Overall preference comparison across different training stages. Right model win rate increases progressively with each component.</p>
                </div>
            </div>

            <!-- 消融实验 -->
            <div style="margin-bottom: 3rem;">
                <h3 style="text-align: center; margin-bottom: 1.5rem; font-size: 1.3rem; color: var(--text-main);">Ablation Study</h3>
                <p style="text-align: center; color: var(--text-secondary); margin-bottom: 2rem; max-width: 900px; margin-left: auto; margin-right: auto;">
                    We analyze the contribution of each component in our cascaded training framework.
                </p>
                
                <!-- 两个消融实验表格并排 -->
                <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 1.5rem; max-width: 1200px; margin: 0 auto; align-items: stretch;">
                    <!-- Table 3: Ablation on PosterReward-Pairwise -->
                    <div class="v-media-card" style="display: flex; flex-direction: column;">
                        <h4 style="text-align: center; margin-bottom: 1rem; font-size: 1rem; color: var(--text-secondary);">PosterReward-Pairwise</h4>
                        <div class="table-scroll-wrapper" style="flex: 1;">
                            <table class="results-table" style="width: 100%; font-size: 0.85rem;">
                                <thead>
                                    <tr>
                                        <th rowspan="2">Method</th>
                                        <th colspan="3" style="text-align: center;">Advanced Acc. ↑</th>
                                        <th colspan="3" style="text-align: center;">Basic Acc. ↑</th>
                                    </tr>
                                    <tr>
                                        <th>Yes</th>
                                        <th>No</th>
                                        <th>Avg.</th>
                                        <th>Yes</th>
                                        <th>No</th>
                                        <th>Avg.</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td>SFT (Single)</td>
                                        <td>81.77</td>
                                        <td>82.09</td>
                                        <td>81.93</td>
                                        <td>80.85</td>
                                        <td>82.59</td>
                                        <td>81.72</td>
                                    </tr>
                                    <tr>
                                        <td>SFT (Joint)</td>
                                        <td>82.09</td>
                                        <td>83.32</td>
                                        <td>82.71</td>
                                        <td>80.08</td>
                                        <td>83.75</td>
                                        <td>81.92</td>
                                    </tr>
                                    <tr>
                                        <td>+ RSFT (Single)</td>
                                        <td>82.67</td>
                                        <td>83.24</td>
                                        <td>82.96</td>
                                        <td>80.66</td>
                                        <td>83.56</td>
                                        <td>82.11</td>
                                    </tr>
                                    <tr style="background: rgba(251, 191, 36, 0.12);">
                                        <td><strong>+ RSFT (Joint)</strong></td>
                                        <td><strong>84.06</strong></td>
                                        <td><strong>83.57</strong></td>
                                        <td><strong>83.82</strong></td>
                                        <td><strong>82.01</strong></td>
                                        <td><strong>83.95</strong></td>
                                        <td><strong>82.98</strong></td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                        <p style="font-size: 0.8rem; color: var(--text-secondary); margin-top: 0.8rem; text-align: center;">"Yes" and "No" refer to the ground truth of the response.</p>
                    </div>

                    <!-- Table 4: Ablation on PosterReward Components -->
                    <div class="v-media-card" style="display: flex; flex-direction: column;">
                        <h4 style="text-align: center; margin-bottom: 1rem; font-size: 1rem; color: var(--text-secondary);">PosterReward Components</h4>
                        <div class="table-scroll-wrapper" style="flex: 1; display: flex; align-items: center;">
                            <table class="results-table" style="width: 100%; font-size: 0.85rem;">
                                <thead>
                                    <tr>
                                        <th>Model / Component</th>
                                        <th>HPDv3</th>
                                        <th>PRB-Basic</th>
                                        <th>PRB-Ad</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td><em>PosterReward-Lite</em></td>
                                        <td>77.1</td>
                                        <td>83.9</td>
                                        <td>85.0</td>
                                    </tr>
                                    <tr>
                                        <td>+ Analysis</td>
                                        <td>77.5</td>
                                        <td>85.7</td>
                                        <td>85.8</td>
                                    </tr>
                                    <tr style="background: rgba(251, 191, 36, 0.12);">
                                        <td><strong>+ Analysis + GRPO</strong></td>
                                        <td><strong>77.8</strong></td>
                                        <td><strong>86.7</strong></td>
                                        <td><strong>86.0</strong></td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                        <p style="font-size: 0.8rem; color: var(--text-secondary); margin-top: 0.8rem; text-align: center;">Cumulative impact of each component on key benchmarks.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Section 5: PosterBench -->
    <div class="table-container" id="results">
        <h2 style="text-align: center; margin-bottom: 0.8rem; font-family: 'Plus Jakarta Sans', sans-serif;">
            PosterBench Leaderboard
            <span style="display: inline-block; margin-left: 0.55rem; padding: 0.15rem 0.5rem; border-radius: 999px; font-size: 0.72rem; font-weight: 600; color: #334155; background: rgba(148, 163, 184, 0.18); border: 1px solid rgba(148, 163, 184, 0.35); vertical-align: middle;">v1.0, 2026/02</span>
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
                    <tr class="bench-group-row">
                        <td colspan="5">Closed-Source Models</td>
                    </tr>
                    <tr>
                        <td>Nano-Banana</td>
                        <td><span class="rank-1">11.60</span></td>
                        <td><span class="rank-1">11.69</span></td>
                        <td>4.94</td>
                        <td><span class="rank-1">14.49</span></td>
                    </tr>
                    <tr>
                        <td>Seedream4.0</td>
                        <td>11.46</td>
                        <td>11.44</td>
                        <td>4.95</td>
                        <td>13.93</td>
                    </tr>
                    <tr>
                        <td>GPT-Image-1</td>
                        <td>11.16</td>
                        <td>11.38</td>
                        <td><span class="rank-1">4.85</span></td>
                        <td>13.43</td>
                    </tr>
                    <tr>
                        <td>Seedream3.0</td>
                        <td>5.01</td>
                        <td>5.13</td>
                        <td>6.28</td>
                        <td>9.75</td>
                    </tr>
                    <tr class="bench-group-row">
                        <td colspan="5">Open-Source Models</td>
                    </tr>
                    <tr>
                        <td>Z-Image-Turbo</td>
                        <td>7.65</td>
                        <td>7.31</td>
                        <td>6.00</td>
                        <td>10.47</td>
                    </tr>
                    <tr>
                        <td>Qwen-Image-2512</td>
                        <td><span class="rank-1">11.86</span></td>
                        <td><span class="rank-1">11.63</span></td>
                        <td><span class="rank-1">5.28</span></td>
                        <td><span class="rank-1">13.85</span></td>
                    </tr>
                    <tr>
                        <td>Qwen-Image</td>
                        <td>7.69</td>
                        <td>7.72</td>
                        <td>5.57</td>
                        <td>11.06</td>
                    </tr>
                    <tr>
                        <td>Flux.1-dev</td>
                        <td>2.55</td>
                        <td>2.42</td>
                        <td>7.10</td>
                        <td>7.81</td>
                    </tr>
                    <tr>
                        <td>Flux-Krea</td>
                        <td>5.00</td>
                        <td>5.14</td>
                        <td>6.87</td>
                        <td>9.58</td>
                    </tr>
                    <tr>
                        <td>SD3.5-L</td>
                        <td>-2.90</td>
                        <td>-3.92</td>
                        <td>5.76</td>
                        <td>1.24</td>
                    </tr>
                </tbody>
            </table>
        </div>
        <p style="text-align: center; margin-top: 1.5rem; color: var(--text-secondary); font-size: 0.9rem;">
            PosterBench evaluation results. Higher Mean/Median/Best-of-8 indicate better average and scalable performance; lower Std indicates more stable quality across prompts.
        </p>
    </div>

    <!-- Section 5: Application - Reward Model in Post Training and Test-Time Scaling -->
    <div class="split-section stacked-showcase" id="posttraining">
        <div class="split-text">
            <span class="section-label">Application</span>
            <h2 class="section-title">Reward Model in Post Training and Test-Time Scaling</h2>
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

            <!-- 视觉比较 -->
            <div style="margin-top: 5rem;">
                <h3 style="text-align: center; margin-bottom: 1.5rem; font-size: 1.3rem; color: var(--text-main);">Visual Comparison</h3>
                <p style="text-align: center; color: var(--text-secondary); margin-bottom: 2rem; max-width: 900px; margin-left: auto; margin-right: auto;">
                    PosterReward enables effective post-training improvement through Best-of-8 selection and GRPO training. Below we show qualitative comparisons between models before and after applying PosterReward-guided optimization.
                </p>

                <!-- BO8筛选效果对比 -->
                <div style="margin-bottom: 4rem;">
                    <h4 style="text-align: center; margin-bottom: 1.2rem; font-size: 1.1rem; color: var(--text-secondary);">Best-of-8 Selection with PosterReward</h4>
                    <p style="text-align: center; color: var(--text-secondary); margin-bottom: 1.5rem; font-size: 0.95rem;">
                        Using PosterReward to select the best from 8 candidates significantly improves output quality compared to random selection.
                    </p>
                    <div class="v-media-stack">
                        <div class="v-media-card">
                            <img src="" alt="BO8 selection comparison" onerror="this.parentElement.style.display='none'">
                            <p class="v-media-caption">Left: Random selection from 8 candidates. Right: PosterReward-guided selection.</p>
                        </div>
                    </div>
                </div>

                <!-- GRPO训练效果对比 -->
                <div style="margin-bottom: 3rem;">
                    <h4 style="text-align: center; margin-bottom: 1.2rem; font-size: 1.1rem; color: var(--text-secondary);">GRPO Post-Training with PosterReward</h4>
                    <p style="text-align: center; color: var(--text-secondary); margin-bottom: 1.5rem; font-size: 0.95rem;">
                        Fine-tuning with PosterReward as reward signal improves typography, layout coherence, and prompt adherence.
                    </p>
                    <div class="v-media-stack">
                        <div class="v-media-card">
                            <img src="" alt="GRPO training comparison" onerror="this.parentElement.style.display='none'">
                            <p class="v-media-caption">Comparison between base model and GRPO-trained model using PosterReward.</p>
                        </div>
                    </div>
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
