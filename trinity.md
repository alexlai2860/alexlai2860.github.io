---
layout: trinity
permalink: /trinity/
title: "Trinity: A Code-Driven Multi-Agent Framework for Professional Graphic Design Creation"
---

<header class="hero">
  <div class="hero-media">
    <img src="/images/trinity/teaser_official.jpg" alt="Trinity design outputs across graphic design deliverables">
  </div>
  <div class="hero-content">
    <div class="status-row">
      <span class="status-chip">Draft paper</span>
      <span class="status-chip">Design agents</span>
      <span class="status-chip">Code-driven creation</span>
    </div>
    <h1>Trinity</h1>
    <p class="hero-subtitle">A code-driven multi-agent framework for professional graphic design creation, built around editable HTML/CSS, project-level memory, reviewer-guided iteration, and accumulated design knowledge.</p>
    <div class="authors">
      <strong>Jianyu Lai</strong>, Sixiang Chen, Jialin Gao, Xiangyu Zhu, Shuaibo Li, Song Fei, Lei Zhu, Zufeng Zhang<br>
      HKUST(GZ), Meituan, Tsinghua University, HKUST
    </div>
    <div class="action-row">
      <a class="action" href="/mypaper/trinity/trinity_20260702_110124.pdf">Paper Draft</a>
      <a class="action" href="#method">Framework</a>
      <span class="action action-muted">Code coming soon</span>
    </div>
  </div>
</header>

<main>
  <section class="section" id="abstract">
    <div class="section-head">
      <div>
        <p class="eyebrow">Abstract</p>
        <h2 class="section-title">Design as editable, reviewable, reusable code.</h2>
      </div>
      <p class="section-copy">Professional graphic design is not a single pretty image: it is a coordinated production workflow that must preserve brand identity, survive repeated edits, and improve as experience accumulates.</p>
    </div>
    <div class="abstract-grid">
      <div class="abstract-text">
        <p>Current diffusion-based approaches are powerful for isolated image generation, but they struggle with cross-deliverable consistency, non-destructive editing, and persistent project memory. <strong>Trinity</strong> reframes graphic design as renderable HTML/CSS code generation, making every layout inspectable, editable, and version-controllable.</p>
        <p>The framework organizes production into three collaborative layers: specialist execution agents, a central Designer agent that implements designs as code, and independent Reviewer agents that provide structured feedback. A master-template system extracts a design handbook from the first deliverable, while tiered code protection keeps later outputs visually consistent.</p>
        <p>Trinity further combines design knowledge reverse-engineered from professional references with workflow experience distilled from deterministic runtime signals, enabling self-improvement without parameter updates.</p>
      </div>
      <aside class="signal-list" aria-label="Trinity draft signals">
        <div class="signal">
          <div class="signal-value">3</div>
          <div class="signal-label">Collaborative layers: execution, design, review.</div>
        </div>
        <div class="signal">
          <div class="signal-value">92</div>
          <div class="signal-label">RealDesignBench task instances in the current draft.</div>
        </div>
        <div class="signal">
          <div class="signal-value">10x</div>
          <div class="signal-label">Sequential edit protocol for multi-round fidelity.</div>
        </div>
      </aside>
    </div>
  </section>

  <section class="section">
    <div class="feature-grid">
      <article class="feature-card">
        <span class="feature-index">01</span>
        <h3>Code-native design</h3>
        <p>Visual composition is produced as deterministic HTML/CSS, supporting structural diffs, precise edits, and browser-based verification.</p>
      </article>
      <article class="feature-card">
        <span class="feature-index">02</span>
        <h3>Project memory</h3>
        <p>A master task becomes a reusable design handbook, letting later deliverables inherit typography, color, spacing, and brand rules.</p>
      </article>
      <article class="feature-card">
        <span class="feature-index">03</span>
        <h3>Reviewer loop</h3>
        <p>Code, visual, layout, and user-alignment reviewers provide structured feedback before the Designer submits a final artifact.</p>
      </article>
      <article class="feature-card">
        <span class="feature-index">04</span>
        <h3>Dual knowledge</h3>
        <p>Professional reference patterns raise the quality ceiling, while runtime experience rules guard the framework's execution floor.</p>
      </article>
    </div>
  </section>

  <section class="section section-wide" id="method">
    <div class="section-head">
      <div>
        <p class="eyebrow">Framework</p>
        <h2 class="section-title">A studio-like multi-agent architecture.</h2>
      </div>
      <p class="section-copy">The Designer agent sits at the hub, dispatching background, font, copy, and logo resources while receiving deterministic audits and independent reviewer feedback. The result is a design workflow that is both creative and inspectable.</p>
    </div>
    <div class="figure-stage">
      <img src="/images/trinity/system_framework_official.png" alt="Overview of the Trinity multi-agent framework">
      <div class="caption">System overview: task compilation, tool-augmented design, deterministic audit gates, progress checking, and multi-reviewer refinement.</div>
    </div>
  </section>

  <section class="section-band" id="project">
    <div class="section section-wide">
      <div class="section-head">
        <div>
          <p class="eyebrow">Project-Level Creation</p>
          <h2 class="section-title">One visual identity, many deliverables.</h2>
        </div>
        <p class="section-copy">Real commercial design work usually needs a family of outputs. Trinity extracts a handbook from the master design and protects consistency-critical code regions, so later tasks can adapt content without drifting away from the project identity.</p>
      </div>
      <div class="workflow-map">
        <div class="workflow-node">
          <h3>Master task</h3>
          <p>Generate the first deliverable through the full pipeline and treat it as the visual source of truth.</p>
        </div>
        <div class="workflow-node">
          <h3>Design handbook</h3>
          <p>Extract reusable color, typography, spacing, and component rules as natural language plus CSS variables.</p>
        </div>
        <div class="workflow-node">
          <h3>Protected variants</h3>
          <p>Subsequent outputs inherit the handbook while locked regions prevent unintentional brand drift.</p>
        </div>
      </div>
      <div class="figure-row">
        <div class="figure-stage">
          <img src="/images/trinity/project_management_official.png" alt="Project management module in Trinity">
          <div class="caption">Master-template project management with handbook extraction and tiered protection.</div>
        </div>
        <div class="figure-stage">
          <img src="/images/trinity/comp_project_gen.jpg" alt="Qualitative comparison of project-level graphic design generation">
          <div class="caption">Qualitative project generation snapshot from the current draft.</div>
        </div>
      </div>
    </div>
  </section>

  <section class="section section-wide">
    <div class="section-head">
      <div>
        <p class="eyebrow">Knowledge</p>
        <h2 class="section-title">Two memories for better design and safer execution.</h2>
      </div>
      <p class="section-copy">Design knowledge answers how to design better in a scenario; workflow experience answers how to operate reliably inside the framework. They are injected as context rather than learned through parameter updates.</p>
    </div>
    <div class="figure-row">
      <div class="figure-stage">
        <img src="/images/trinity/dual_knowledge_official.png" alt="Dual knowledge mechanism in Trinity">
        <div class="caption">Design knowledge retrieval and workflow experience accumulation.</div>
      </div>
      <div class="figure-stage">
        <img src="/images/trinity/dataset_and_knowledge.png" alt="Dataset and knowledge construction in Trinity">
        <div class="caption">Benchmark and knowledge construction pipeline.</div>
      </div>
    </div>
  </section>

  <section class="section section-wide" id="results">
    <div class="section-head">
      <div>
        <p class="eyebrow">Current Draft Results</p>
        <h2 class="section-title">Competitive quality with stronger consistency and edit fidelity.</h2>
      </div>
      <p class="section-copy">The manuscript is still evolving, so these numbers are shown as a compact snapshot rather than a final leaderboard. The stronger story is the pattern: code-based generation narrows the quality gap while improving project consistency and multi-round editing fidelity.</p>
    </div>
    <div class="results-grid">
      <div class="metric-board">
        <div class="metric">
          <strong>8.15</strong>
          <span>Project-level overall score for the Gemini-3.1-Pro + Seedream-4.5 Trinity variant in the current table.</span>
        </div>
        <div class="metric">
          <strong>7.96</strong>
          <span>Single-image overall score for the same Trinity variant, close to strong end-to-end baselines.</span>
        </div>
        <div class="metric">
          <strong>7.78</strong>
          <span>Average cumulative edit fidelity across the current 10-step editing protocol.</span>
        </div>
        <div class="metric">
          <strong>71.9%</strong>
          <span>Pairwise edit win rate against GPT-Image-2 on final step-10 outputs in the draft protocol.</span>
        </div>
      </div>
      <div class="figure-stage">
        <img src="/images/trinity/winrate_combined.png" alt="Pairwise win rate summary for Trinity">
        <div class="caption">Pairwise comparison summary grouped by generation, editing, coding-agent, and ablation categories.</div>
      </div>
    </div>
    <div class="figure-row">
      <div class="figure-stage">
        <img src="/images/trinity/dim_radar.png" alt="Dimension radar chart for Trinity evaluation">
        <div class="caption">Per-dimension radar chart for the draft evaluation.</div>
      </div>
      <div class="figure-stage">
        <img src="/images/trinity/supp_edit_comp.jpg" alt="Multi-round editing comparison for Trinity">
        <div class="caption">Multi-round editing comparison: code-based layer routing preserves more of the original design.</div>
      </div>
    </div>
  </section>

  <section class="section" id="citation">
    <div class="section-head">
      <div>
        <p class="eyebrow">Citation</p>
        <h2 class="section-title">Draft BibTeX</h2>
      </div>
      <p class="section-copy">This entry is intentionally provisional while the manuscript is still being finalized.</p>
    </div>
    <pre class="citation"><code>@article{lai2026trinity,
  title={Trinity: A Code-Driven Multi-Agent Framework for Professional Graphic Design Creation},
  author={Lai, Jianyu and Chen, Sixiang and Gao, Jialin and Zhu, Xiangyu and Li, Shuaibo and Fei, Song and Zhu, Lei and Zhang, Zufeng},
  year={2026}
}</code></pre>
  </section>
</main>
