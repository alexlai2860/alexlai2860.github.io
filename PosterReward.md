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
        <a href="https://github.com/Ephemeral182/PosterOmni" class="btn btn-secondary"><span>💻</span> Code</a>
        <a href="https://huggingface.co/PosterOmni" class="btn btn-secondary"><span>🤗</span> Model</a>
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

    <!-- Section 1: Capabilities (Left Text, Right Image) -->
    <div class="split-section" id="features">
        <div class="split-text">
            <span class="section-label">Capabilities</span>
            <h2 class="section-title">Diverse Poster Creation Tasks</h2>
            <div class="feature-list">
                <div class="feature-item">
                    <div class="number-badge">1</div>
                    <span class="feature-heading">Local Editing Precision</span>
                    <p class="feature-desc">Performs precise local adjustments including extending, filling, rescaling, and identity-driven generation while preserving the original subject.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">2</div>
                    <span class="feature-heading">Global Creation Reasoning</span>
                    <p class="feature-desc">Handles abstract high-level tasks such as layout-driven and style-driven generation, ensuring aesthetic coherence across the entire poster.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">3</div>
                    <span class="feature-heading">Unified Framework</span>
                    <p class="feature-desc">Seamlessly integrates multiple editing and generation capabilities into a single model without switching pipelines.</p>
                </div>
            </div>
        </div>
        <div class="split-visual">
            <img src="/images/posterreward/teaser_0209.jpg" alt="PosterReward Capabilities Teaser">
        </div>
    </div>

    <!-- Section 2: Data Pipeline (Right Text, Left Image - using reverse) -->
    <div class="split-section reverse" id="data">
        <div class="split-text">
            <span class="section-label">Data Engineering</span>
            <h2 class="section-title">Automated Data Construction</h2>
            <div class="feature-list">
                <div class="feature-item">
                    <div class="number-badge">1</div>
                    <span class="feature-heading">Prompt & Image Generation</span>
                    <p class="feature-desc">Leverages GPT-4 and Qwen to generate diverse, structured prompts and initial images covering various themes.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">2</div>
                    <span class="feature-heading">Multimodal Filtering</span>
                    <p class="feature-desc">Employs OCR and VLM-based filtering to ensure textual correctness and layout-content consistency.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">3</div>
                    <span class="feature-heading">Task-Specific Construction</span>
                    <p class="feature-desc">Automatically synthesizes paired data for 6 specific tasks using tools like SAM-2 and BrushNet.</p>
                </div>
            </div>
        </div>
        <div class="split-visual">
            <img src="/images/posterreward/posterreward_datapipeline.jpg" alt="Data Construction Pipeline">
        </div>
    </div>

    <!-- Section 3: Methodology (Left Text, Right Image) -->
    <div class="split-section" id="method">
        <div class="split-text">
            <span class="section-label">Methodology</span>
            <h2 class="section-title">Progressive Training Pipeline</h2>
            <div class="feature-list">
                <div class="feature-item">
                    <div class="number-badge">1</div>
                    <span class="feature-heading">Task-Specific SFT</span>
                    <p class="feature-desc">Trains specialized experts for local editing and global creation to ensure high fidelity in distinct domains.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">2</div>
                    <span class="feature-heading">Task Distillation</span>
                    <p class="feature-desc">Distills knowledge from experts into a unified student model, merging pixel precision with aesthetic understanding.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">3</div>
                    <span class="feature-heading">Unified Reward Feedback</span>
                    <p class="feature-desc">Aligns with human preferences using a reward model that evaluates both aesthetic appeal and instruction adherence.</p>
                </div>
                <div class="feature-item">
                    <div class="number-badge">4</div>
                    <span class="feature-heading">Omni-Edit RL</span>
                    <p class="feature-desc">Uses Reinforcement Learning to refine generation quality and align it with professional design standards.</p>
                </div>
            </div>
        </div>
        <div class="split-visual">
            <img src="/images/posterreward/overview.jpg" alt="PosterReward Methodology Overview">
        </div>
    </div>

    <!-- Leaderboard -->
    <div class="table-container" id="results">
        <h2 style="text-align: center; margin-bottom: 2rem; font-family: 'Plus Jakarta Sans', sans-serif;">
            PosterBench Leaderboard <span class="benchmark-badge">PosterBench</span>
        </h2>
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
            Performance of different models on PosterBench. Mean, Median, and Top8-Avg represent the respective scores. Std denotes the standard deviation of scores, indicating stability (lower is better).
        </p>
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
