---
permalink: / 
title: ""
excerpt: "About me"
author_profile: true

redirect_from:
  - /about/
  - /about.html

---

<style>
:root {
  --accent: #6366f1;
  --accent-light: #818cf8;
  --bg-card: #fafafa;
  --text-primary: #111;
  --text-secondary: #555;
  --text-muted: #888;
  --border: #e5e5e5;
}

.intro-text {
  font-size: 1.2em;
  line-height: 1.7;
  color: var(--text-primary);
  font-weight: 400;
}
.intro-text strong {
  font-weight: 600;
}
.intro-text a {
  color: var(--accent);
  text-decoration: none;
  border-bottom: 2px solid var(--accent-light);
}

/* Modern Card */
.modern-card {
  background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);
  padding: 2em;
  border-radius: 16px;
  margin: 2em 0;
  color: white;
}
.modern-card h3 {
  color: white;
  font-size: 1.4em;
  margin: 0 0 0.8em 0;
  font-weight: 700;
}
.modern-card p {
  opacity: 0.92;
  line-height: 1.6;
  margin-bottom: 1em;
}
.modern-card a {
  color: #fde68a;
}
.modern-card .papers {
  display: flex;
  gap: 0.8em;
  flex-wrap: wrap;
  margin-top: 1.2em;
}
.modern-card .paper-chip {
  background: rgba(255,255,255,0.2);
  padding: 0.5em 1em;
  border-radius: 8px;
  font-size: 0.85em;
  backdrop-filter: blur(4px);
  transition: background 0.2s;
  text-decoration: none;
  color: white;
}
.modern-card .paper-chip:hover {
  background: rgba(255,255,255,0.35);
}
.modern-card .paper-chip .venue {
  opacity: 0.7;
  font-size: 0.85em;
  margin-left: 0.3em;
}

/* Tabs */
.tabs {
  margin: 2em 0;
}
.tab-nav {
  display: flex;
  gap: 0;
  border-bottom: 2px solid var(--border);
  margin-bottom: 1.5em;
}
.tab-nav button {
  background: none;
  border: none;
  padding: 0.8em 1.5em;
  font-size: 0.95em;
  font-weight: 600;
  color: var(--text-muted);
  cursor: pointer;
  position: relative;
  transition: color 0.2s;
}
.tab-nav button:hover {
  color: var(--text-secondary);
}
.tab-nav button.active {
  color: var(--accent);
}
.tab-nav button.active::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--accent);
}
.tab-panel {
  display: none;
}
.tab-panel.active {
  display: block;
}
.tab-panel h4 {
  font-size: 1em;
  color: var(--text-secondary);
  font-weight: 500;
  margin: 0 0 1.5em 0;
}

/* Paper Grid */
.paper-grid {
  display: grid;
  gap: 0;
}
.paper-row {
  display: grid;
  grid-template-columns: auto 1fr auto;
  gap: 1.5em;
  padding: 0.6em 0;
  border-bottom: 1px solid var(--border);
  align-items: center;
}
.paper-row:last-child {
  border-bottom: none;
}
.paper-row .name {
  min-width: 120px;
}
.paper-row .name a {
  font-weight: 600;
  font-size: 1em;
  color: var(--text-primary);
  text-decoration: none;
  transition: color 0.15s;
  white-space: nowrap;
}
.paper-row .name a:hover {
  color: var(--accent);
}
.paper-row .desc {
  color: var(--text-secondary);
  font-size: 0.95em;
}
.paper-row .venue {
  text-align: right;
}
.paper-row .venue span, .paper-row .venue-badge {
  display: inline-block;
  padding: 0.3em 0.7em;
  border-radius: 4px;
  font-size: 0.75em;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}
.venue-iclr { background: #e0f2fe; color: #0369a1; }
.venue-neurips { background: #fce7f3; color: #be185d; }
.venue-colm { background: #d1fae5; color: #047857; }
.venue-tmlr { background: #fef3c7; color: #b45309; }
.venue-tacl { background: #ede9fe; color: #6d28d9; }
.venue-aaai { background: #fee2e2; color: #b91c1c; }
.venue-jmlr { background: #e0e7ff; color: #4338ca; }
.venue-arxiv { background: #f3f4f6; color: #4b5563; }
.venue-acl { background: #dcfce7; color: #15803d; }
.venue-icml { background: #dbeafe; color: #1d4ed8; }
.venue-emnlp { background: #ccfbf1; color: #0f766e; }
.venue-aacl { background: #fef9c3; color: #a16207; }
.paper-row .venue .award {
  background: linear-gradient(90deg, #f59e0b, #ef4444);
  color: white;
  padding: 0.3em 0.7em;
  border-radius: 4px;
  font-weight: 700;
  font-size: 0.75em;
}

/* CTA */
.cta {
  background: var(--bg-card);
  padding: 1.5em 2em;
  border-radius: 12px;
  border: 1px solid var(--border);
  text-align: center;
  margin: 2em 0;
}
.cta strong {
  color: var(--accent);
}

/* Hero */
.hero-title {
  font-size: 2em;
  font-weight: 700;
  color: var(--text-primary);
  margin: 0 0 0.3em 0;
  line-height: 1.2;
}
.hero-subtitle {
  font-size: 1.15em;
  color: var(--accent);
  font-weight: 500;
  margin-bottom: 1em;
}
.hero-text {
  font-size: 1.05em;
  line-height: 1.7;
  color: var(--text-secondary);
}
.hero-text a {
  color: var(--accent);
  text-decoration: none;
  font-weight: 500;
}

/* Research Philosophy */
.research-intro {
  font-size: 1em;
  line-height: 1.7;
  color: var(--text-secondary);
  margin-bottom: 1.5em;
  padding-left: 1em;
  border-left: 3px solid var(--accent);
}
</style>

<h1 class="hero-title">Pierre Colombo</h1>
<p class="hero-subtitle">👨‍🏫 Associate Professor · 🧪 Chief Science Officer</p>
<p class="hero-text">
I lead AI research at <a href="https://www.centralesupelec.fr/">CentraleSupélec</a> (Paris-Saclay) and <a href="https://equall.ai/">Equall.ai</a>. My work focuses on making large language models <strong>reliable</strong>, <strong>measurable</strong>, and <strong>deployable</strong> in domains where errors matter—like law, and enterprise systems.
</p>

---

<div class="modern-card">
<h3>🏛️ Equall.ai — AI for Law</h3>
<p>Legal AI demands precision and domain expertise. We built <strong>SaulLM</strong>—the first LLM for law—and use it to power <strong>M&A due diligence</strong> automation currently used at Big Laws.</p>
<div class="papers">
  <a href="https://arxiv.org/abs/2403.03883" class="paper-chip">SaulLM-7B <span class="venue">arXiv</span></a>
  <a href="https://arxiv.org/abs/2407.19584" class="paper-chip">SaulLM-141B <span class="venue">NEURIPS</span></a>
  <a href="https://equall.ai/" class="paper-chip">→ Equall.ai</a>
</div>
</div>

---

## 🔬 Research

<p class="research-intro">
I believe AI research should be <strong>open</strong>, <strong>reproducible</strong>, and <strong>useful</strong>. I build models that anyone can use, develop evaluation methods that reveal true capabilities, and focus on problems that matter in the real world. Good research creates tools that others can build on—not just papers.
</p>

<div class="tabs">
  <div class="tab-nav">
    <button class="active" onclick="switchTab(event, 'llm')">🚀 LLMs & Multimodal</button>
    <button onclick="switchTab(event, 'eval')">📊 Evaluation</button>
    <button onclick="switchTab(event, 'fair')">⚖️ Fairness</button>
  </div>

  <div id="llm" class="tab-panel active">
    <h4>Open, multilingual, and multimodal models</h4>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2407.01449">ColPali</a></div>
        <div class="desc">SOTA document retrieval with vision-language</div>
        <div class="venue"><span class="venue-iclr">ICLR</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2510.21849">TowerVision</a></div>
        <div class="desc">Multilinguality in vision-language models</div>
        <div class="venue"><span class="venue-arxiv">arXiv</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2510.01149">ModernVBERT</a></div>
        <div class="desc">Smaller visual document retrievers</div>
        <div class="venue"><span class="venue-arxiv">arXiv</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2402.17733">TowerLLM</a></div>
        <div class="desc">GPT-4 translation quality with 7B params</div>
        <div class="venue"><span class="venue-colm">COLM</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2402.00786">CroissantLLM</a></div>
        <div class="desc">First bilingual French-English LLM</div>
        <div class="venue"><span class="venue-tmlr">TMLR</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2409.16235">EuroLLM</a></div>
        <div class="desc">Multilingual LLMs for European languages</div>
        <div class="venue"><span class="venue-neurips">NeurIPS</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2503.05500">EuroBERT</a></div>
        <div class="desc">Scaling multilingual encoders for Europe</div>
        <div class="venue"><span class="venue-colm">COLM</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2402.12030">Distillation</a></div>
        <div class="desc">Cross-tokenizer distillation for LLMs</div>
        <div class="venue"><span class="venue-tmlr">TMLR</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2211.05100">BLOOM</a></div>
        <div class="desc">176B open multilingual model</div>
        <div class="venue"><span class="venue-jmlr">JMLR</span></div>
      </div>
    </div>
  </div>

  <div id="eval" class="tab-panel">
    <h4>Metrics that measure what matters</h4>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2310.10482">xCOMET</a></div>
        <div class="desc">Fine-grained translation evaluation</div>
        <div class="venue"><span class="venue-tacl">TACL</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://ojs.aaai.org/index.php/AAAI/article/view/21299">InfoLM</a></div>
        <div class="desc">Information-theoretic generation metrics</div>
        <div class="venue"><span class="award">🏆 Best Paper AAAI</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2303.16104">Hallucinations</a></div>
        <div class="desc">Detection in neural machine translation</div>
        <div class="venue"><span class="venue-tacl">TACL</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2211.13527">OOD Detection</a></div>
        <div class="desc">Beyond Mahalanobis for textual OOD</div>
        <div class="venue"><span class="venue-neurips">NeurIPS</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2202.03799">Benchmarking</a></div>
        <div class="desc">Fair model comparison methods</div>
        <div class="venue"><span class="venue-neurips">NeurIPS</span></div>
      </div>
    </div>
  </div>

  <div id="fair" class="tab-panel">
    <h4>Fair and safe AI systems</h4>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><a href="https://aclanthology.org/2021.acl-long.511/">Disentanglement</a></div>
        <div class="desc">Fair generation via mutual information</div>
        <div class="venue"><span class="venue-acl">ACL</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://proceedings.mlr.press/v162/pichler22a.html">Entropy Estimation</a></div>
        <div class="desc">Fair classification via differential entropy</div>
        <div class="venue"><span class="venue-icml">ICML</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://proceedings.neurips.cc/paper_files/paper/2020/hash/2cfa3753d6a524711acb5fce38eeca1a-Abstract.html">Heavy-tailed</a></div>
        <div class="desc">Robust text classification</div>
        <div class="venue"><span class="venue-neurips">NeurIPS</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2310.14001">Attack Detection</a></div>
        <div class="desc">Stronger textual adversarial detectors</div>
        <div class="venue"><span class="venue-emnlp">EMNLP</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2302.09852">Safe Classification</a></div>
        <div class="desc">Robustness in text classification</div>
        <div class="venue"><span class="venue-aaai">AAAI</span></div>
      </div>
    </div>
  </div>

  <div id="pubs" class="tab-panel">
    <h4>Full publication list</h4>
    <p style="color: var(--text-secondary); margin-bottom: 1em;">
      100+ papers · 5000+ citations · <a href="https://scholar.google.com/citations?user=YOUR_ID" style="color: var(--accent);">Google Scholar</a>
    </p>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><a href="#">2024</a></div>
        <div class="desc">ColPali, SaulLM-141B, EuroLLM, TowerVision...</div>
        <div class="venue"><span class="venue-neurips">15 papers</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="#">2023</a></div>
        <div class="desc">xCOMET, CroissantLLM, Hallucinations...</div>
        <div class="venue"><span class="venue-iclr">20 papers</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="#">2022</a></div>
        <div class="desc">InfoLM, BLOOM, OOD Detection...</div>
        <div class="venue"><span class="venue-icml">18 papers</span></div>
      </div>
    </div>
  </div>

  <div id="teach" class="tab-panel">
    <h4>Teaching & academic service</h4>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><strong>Teaching</strong></div>
        <div class="desc">Introduction to Deep Learning</div>
        <div class="venue"><span class="venue-colm">CentraleSupélec</span></div>
      </div>
      <div class="paper-row">
        <div class="name"></div>
        <div class="desc">Natural Language Processing</div>
        <div class="venue"><span class="venue-tacl">Master M2</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><strong>Service</strong></div>
        <div class="desc">Area Chair</div>
        <div class="venue"><span class="venue-acl">ACL</span> <span class="venue-emnlp">EMNLP</span> <span class="venue-neurips">NeurIPS</span></div>
      </div>
      <div class="paper-row">
        <div class="name"></div>
        <div class="desc">Reviewer</div>
        <div class="venue"><span class="venue-iclr">ICLR</span> <span class="venue-icml">ICML</span> <span class="venue-aaai">AAAI</span></div>
      </div>
    </div>
  </div>
</div>

<script>
function switchTab(e, id) {
  document.querySelectorAll('.tab-nav button').forEach(b => b.classList.remove('active'));
  document.querySelectorAll('.tab-panel').forEach(p => p.classList.remove('active'));
  e.target.classList.add('active');
  document.getElementById(id).classList.add('active');
}
</script>

---

<div class="cta">
<strong>Let's collaborate. 🤝</strong> I work with CMU, IST Lisbon, Edinburgh, INRIA, Telecom Paris, Sorbonne Universite and industry partners.<br>
Open to collaborations.
</div>
