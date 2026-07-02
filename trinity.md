---
layout: trinity
permalink: /trinity/
title: "Trinity: A Code-Driven Multi-Agent Framework for Professional Graphic Design Creation"
---

<header class="hero" id="top">
  <div class="hero-inner">
    <div class="product-pill">Design agent framework for professional graphic design</div>
    <h1>
      <span class="hero-title-line">Trinity</span>
      <span class="hero-title-line hero-title-accent">Code as Design</span>
    </h1>
    <p class="hero-copy">A multi-agent framework that turns professional graphic design into editable, reviewable, and reusable HTML/CSS artifacts, with project-level memory and workflow experience that improves over repeated runs.</p>
    <div class="author-line">
      <strong>Jianyu Lai</strong>, Sixiang Chen, Jialin Gao, Xiangyu Zhu, Shuaibo Li, Song Fei, Lei Zhu, Zufeng Zhang<br>
      HKUST(GZ), Meituan, Tsinghua University, HKUST
    </div>
    <div class="hero-actions">
      <a class="button button-primary" href="/mypaper/trinity/trinity_20260702_110124.pdf">Read Paper Draft</a>
      <a class="button" href="#framework">Explore Framework</a>
      <a class="button" aria-disabled="true">Code Coming Soon</a>
    </div>

    <div class="hero-product">
      <div class="window-frame">
        <div class="window-top">
          <span class="dot"></span>
          <span class="dot"></span>
          <span class="dot"></span>
          <span class="window-path">trinity / design outputs / project canvas</span>
        </div>
        <img src="/images/trinity/teaser_official.jpg" alt="Trinity design outputs across multiple graphic design deliverables">
      </div>
      <div class="float-panel panel-left">
        <strong>HTML/CSS source</strong>
        <span>Editable foreground layers, deterministic rendering, and precise local revision.</span>
      </div>
      <div class="float-panel panel-right">
        <strong>Project memory</strong>
        <span>Master template, design handbook, and protected consistency-critical regions.</span>
      </div>
    </div>
  </div>
</header>

<main>
  <section class="section" id="overview">
    <div class="section-head reveal">
      <div>
        <p class="eyebrow">Overview</p>
        <h2 class="section-title">From one-off image generation to a design production workflow.</h2>
      </div>
      <p class="section-copy">Professional graphic design requires more than visual appeal. Campaigns need coherent families of deliverables, exact text and brand placement, repeated client edits, and lessons that carry into future production. Trinity treats design as code so the system can inspect, diff, protect, and revise every artifact.</p>
    </div>

    <div class="metrics-strip reveal">
      <div class="metric-tile">
        <strong>3</strong>
        <span>Collaborative layers: execution specialists, central Designer, and independent reviewers.</span>
      </div>
      <div class="metric-tile">
        <strong>92</strong>
        <span>RealDesignBench task instances in the current draft evaluation.</span>
      </div>
      <div class="metric-tile">
        <strong>10x</strong>
        <span>Sequential edit protocol to test accumulated fidelity across rounds.</span>
      </div>
      <div class="metric-tile">
        <strong>Code</strong>
        <span>Renderable HTML/CSS becomes the design representation and the audit surface.</span>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="capability-grid reveal">
      <article class="capability">
        <span class="capability-index">01</span>
        <h3>Code-native artifacts</h3>
        <p>Graphic designs are generated as structured HTML/CSS, enabling deterministic previews, local edits, and version-controllable visual composition.</p>
      </article>
      <article class="capability">
        <span class="capability-index">02</span>
        <h3>Agent-native studio</h3>
        <p>The Designer dispatches font, background, copy, and logo resources while reviewers examine code quality, layout quality, and task alignment.</p>
      </article>
      <article class="capability">
        <span class="capability-index">03</span>
        <h3>Series consistency</h3>
        <p>A master design is distilled into a handbook, then protected through tiered code rules so later deliverables keep the same visual identity.</p>
      </article>
      <article class="capability">
        <span class="capability-index">04</span>
        <h3>Dual knowledge</h3>
        <p>Professional reference patterns improve design decisions, while runtime experience rules reduce repeated workflow failures.</p>
      </article>
    </div>
  </section>

  <section class="section section-wide" id="framework">
    <div class="section-head reveal">
      <div>
        <p class="eyebrow">Framework</p>
        <h2 class="section-title">A local design studio made of agents, audits, and previews.</h2>
      </div>
      <p class="section-copy">The current manuscript places the Designer at the center of the system. It compiles the task, calls execution-layer resources, renders intermediate previews, passes deterministic audit gates, and receives reviewer feedback before final submission.</p>
    </div>
    <div class="figure-stage reveal">
      <img src="/images/trinity/system_framework_official.png" alt="Overview of the Trinity multi-agent framework">
      <div class="figure-caption">
        <span>Task compilation, tool-augmented design, checkpointing, audit gates, and multi-reviewer refinement.</span>
        <span class="caption-tag">Figure 2</span>
      </div>
    </div>
  </section>

  <section class="section-band" id="project">
    <div class="section section-wide">
      <div class="section-head reveal">
        <div>
          <p class="eyebrow">Project-Level Management</p>
          <h2 class="section-title">One master design, many consistent deliverables.</h2>
        </div>
        <p class="section-copy">A real campaign is a family, not a singleton. Trinity generates a master task first, extracts a reusable design handbook, and protects key code regions so later tasks can change content without drifting from the brand direction.</p>
      </div>

      <div class="process-grid reveal">
        <article class="process-step" data-step="01">
          <h3>Master task</h3>
          <p>Create the first deliverable through the full generation and review pipeline.</p>
        </article>
        <article class="process-step" data-step="02">
          <h3>Handbook extraction</h3>
          <p>Summarize color, typography, spacing, components, and reusable CSS variables.</p>
        </article>
        <article class="process-step" data-step="03">
          <h3>Tiered protection</h3>
          <p>Lock identity-critical regions while allowing task-specific content to change.</p>
        </article>
        <article class="process-step" data-step="04">
          <h3>Consistency review</h3>
          <p>Compare new deliverables against the master and design handbook.</p>
        </article>
      </div>

      <div class="figure-row">
        <div class="figure-stage reveal">
          <img src="/images/trinity/project_management_official.png" alt="Project management module in Trinity">
          <div class="figure-caption">
            <span>Master template, design handbook, inheritance, and protected edits.</span>
            <span class="caption-tag">Figure 3</span>
          </div>
        </div>
        <div class="figure-stage reveal">
          <img src="/images/trinity/comp_project_gen.jpg" alt="Qualitative project-level generation comparison">
          <div class="figure-caption">
            <span>Project-level generation comparison from the current paper draft.</span>
            <span class="caption-tag">Figure 5</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="section section-wide" id="knowledge">
    <div class="section-head reveal">
      <div>
        <p class="eyebrow">Knowledge</p>
        <h2 class="section-title">Design knowledge raises the ceiling. Workflow experience protects the floor.</h2>
      </div>
      <p class="section-copy">Trinity separates creative guidance from operational reliability. Design knowledge is extracted from professional references and retrieved at runtime; workflow experience is distilled from audit failures, incidents, and behavioral anomalies.</p>
    </div>
    <div class="figure-row">
      <div class="figure-stage reveal">
        <img src="/images/trinity/dual_knowledge_official.png" alt="Dual knowledge mechanism in Trinity">
        <div class="figure-caption">
          <span>Offline design pattern extraction plus runtime workflow experience accumulation.</span>
          <span class="caption-tag">Figure 4</span>
        </div>
      </div>
      <div class="figure-stage reveal">
        <img src="/images/trinity/reviewer_distribution.png" alt="Reviewer decision distribution in Trinity">
        <div class="figure-caption">
          <span>Reviewer distribution used in the current appendix analysis.</span>
          <span class="caption-tag">Appendix</span>
        </div>
      </div>
    </div>
  </section>

  <section class="section section-wide" id="results">
    <div class="section-head reveal">
      <div>
        <p class="eyebrow">Draft Results</p>
        <h2 class="section-title">A compact snapshot, not a final leaderboard.</h2>
      </div>
      <p class="section-copy">The paper is still being finalized, so this page only highlights the current trend: code-based generation stays competitive on single-image quality while improving project consistency and long-horizon editing fidelity.</p>
    </div>

    <div class="results-layout">
      <div class="result-stack reveal">
        <div class="result-item">
          <strong>8.15</strong>
          <span>Current project-level overall score for Trinity using Gemini-3.1-Pro + Seedream-4.5.</span>
        </div>
        <div class="result-item">
          <strong>7.96</strong>
          <span>Current single-image overall score for the same Trinity variant.</span>
        </div>
        <div class="result-item">
          <strong>7.78</strong>
          <span>Average cumulative fidelity under the 10-step edit protocol.</span>
        </div>
        <div class="result-item">
          <strong>71.9%</strong>
          <span>Pairwise edit win rate against GPT-Image-2 in the draft final-step comparison.</span>
        </div>
      </div>

      <div class="figure-stage reveal">
        <img src="/images/trinity/winrate_combined.png" alt="Pairwise win rate summary for Trinity">
        <div class="figure-caption">
          <span>Pairwise win rates grouped by generation, editing, coding-agent, and ablation categories.</span>
          <span class="caption-tag">Figure 6</span>
        </div>
      </div>
    </div>

    <div class="mini-gallery">
      <div class="figure-stage reveal">
        <img src="/images/trinity/supp_edit_comp.jpg" alt="Multi-round editing comparison for Trinity">
        <div class="figure-caption">
          <span>Multi-round editing comparison: layer routing preserves the original design more reliably.</span>
          <span class="caption-tag">Figure 7</span>
        </div>
      </div>
      <div>
        <div class="figure-stage reveal">
          <img src="/images/trinity/edit_fidelity_heatmap.png" alt="Edit fidelity heatmap for Trinity">
          <div class="figure-caption">
            <span>Edit fidelity heatmap from the current appendix.</span>
            <span class="caption-tag">Appendix</span>
          </div>
        </div>
        <div class="figure-row">
          <div class="figure-stage reveal">
            <img src="/images/trinity/dim_radar.png" alt="Dimension radar chart for Trinity evaluation">
            <div class="figure-caption">
              <span>Dimension radar.</span>
              <span class="caption-tag">Appendix</span>
            </div>
          </div>
          <div class="figure-stage reveal">
            <img src="/images/trinity/human_eval.png" alt="Human evaluation chart for Trinity">
            <div class="figure-caption">
              <span>Human evaluation.</span>
              <span class="caption-tag">Appendix</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="section" id="citation">
    <div class="section-head reveal">
      <div>
        <p class="eyebrow">Citation</p>
        <h2 class="section-title">Draft BibTeX</h2>
      </div>
      <p class="section-copy">This entry is intentionally provisional while the manuscript is still being finalized.</p>
    </div>
    <pre class="citation reveal"><code>@article{lai2026trinity,
  title={Trinity: A Code-Driven Multi-Agent Framework for Professional Graphic Design Creation},
  author={Lai, Jianyu and Chen, Sixiang and Gao, Jialin and Zhu, Xiangyu and Li, Shuaibo and Fei, Song and Zhu, Lei and Zhang, Zufeng},
  year={2026}
}</code></pre>
  </section>
</main>
