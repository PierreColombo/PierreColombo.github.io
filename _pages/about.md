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
  --accent-dark: #4f46e5;
  --bg-card: #fafafa;
  --text-primary: #111;
  --text-secondary: #555;
  --text-muted: #888;
  --border: #e5e5e5;
}

/* Hero */
.hero-title {
  font-size: 2.1em;
  font-weight: 700;
  color: var(--text-primary);
  margin: 0 0 0.2em 0;
  line-height: 1.15;
  letter-spacing: -0.01em;
}
.hero-subtitle {
  font-size: 1.1em;
  color: var(--accent);
  font-weight: 600;
  margin: 0 0 0.8em 0;
  display: flex;
  flex-wrap: wrap;
  gap: 0.5em 0.9em;
  align-items: center;
}
.hero-subtitle .now {
  background: linear-gradient(90deg, #6366f1, #8b5cf6);
  color: white;
  padding: 0.2em 0.7em;
  border-radius: 6px;
  font-size: 0.85em;
  font-weight: 700;
  letter-spacing: 0.02em;
}
.hero-subtitle .past {
  color: var(--text-muted);
  font-weight: 500;
  font-size: 0.9em;
}
.hero-text {
  font-size: 1.05em;
  line-height: 1.65;
  color: var(--text-secondary);
  margin-bottom: 0.5em;
}
.hero-text a {
  color: var(--accent);
  text-decoration: none;
  font-weight: 500;
  border-bottom: 1px solid var(--accent-light);
}
.hero-text strong {
  color: var(--text-primary);
  font-weight: 600;
}

/* Stats banner */
.stats-banner {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1em;
  margin: 1.8em 0;
  padding: 1.2em;
  background: linear-gradient(135deg, #f5f3ff 0%, #eef2ff 100%);
  border-radius: 12px;
  border: 1px solid #e0e7ff;
}
.stat {
  text-align: center;
}
.stat .num {
  display: block;
  font-size: 1.7em;
  font-weight: 700;
  color: var(--accent-dark);
  line-height: 1;
  margin-bottom: 0.25em;
  letter-spacing: -0.02em;
}
.stat .label {
  font-size: 0.75em;
  color: var(--text-secondary);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-weight: 600;
}
.stats-banner .source {
  grid-column: 1 / -1;
  text-align: center;
  font-size: 0.78em;
  color: var(--text-muted);
  margin-top: 0.3em;
}
.stats-banner .source a {
  color: var(--accent);
  text-decoration: none;
}
@media (max-width: 600px) {
  .stats-banner { grid-template-columns: repeat(2, 1fr); }
}

/* Section heading */
.section-h {
  font-size: 1.5em;
  font-weight: 700;
  margin: 2em 0 1em 0;
  color: var(--text-primary);
  letter-spacing: -0.01em;
}
.section-h .kicker {
  display: block;
  font-size: 0.65em;
  color: var(--accent);
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  margin-bottom: 0.25em;
}

/* Builder cards */
.builder-grid {
  display: grid;
  gap: 1em;
  margin: 1em 0 2em 0;
}
.builder-card {
  border: 1px solid var(--border);
  border-radius: 12px;
  padding: 1.4em 1.6em;
  background: white;
  transition: border-color 0.2s, box-shadow 0.2s;
  position: relative;
}
.builder-card:hover {
  border-color: var(--accent-light);
  box-shadow: 0 4px 12px rgba(99, 102, 241, 0.08);
}
.builder-card.now {
  background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 100%);
  border: none;
  color: white;
}
.builder-card.now:hover {
  box-shadow: 0 6px 20px rgba(99, 102, 241, 0.25);
}
.builder-card .when {
  font-size: 0.75em;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--text-muted);
  margin-bottom: 0.4em;
}
.builder-card.now .when {
  color: rgba(255,255,255,0.85);
}
.builder-card .role {
  font-size: 1.2em;
  font-weight: 700;
  color: var(--text-primary);
  margin: 0 0 0.15em 0;
}
.builder-card.now .role {
  color: white;
}
.builder-card .where {
  font-size: 0.95em;
  color: var(--accent);
  font-weight: 600;
  margin-bottom: 0.7em;
}
.builder-card.now .where {
  color: #fde68a;
}
.builder-card .body {
  font-size: 0.95em;
  line-height: 1.6;
  color: var(--text-secondary);
}
.builder-card.now .body {
  color: rgba(255,255,255,0.92);
}
.builder-card .body strong {
  color: var(--text-primary);
  font-weight: 600;
}
.builder-card.now .body strong {
  color: white;
}
.builder-card .highlights {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5em;
  margin-top: 0.9em;
}
.builder-card .chip {
  background: rgba(99,102,241,0.08);
  color: var(--accent-dark);
  padding: 0.3em 0.7em;
  border-radius: 6px;
  font-size: 0.8em;
  font-weight: 600;
}
.builder-card.now .chip {
  background: rgba(255,255,255,0.18);
  color: white;
  backdrop-filter: blur(4px);
}
.builder-card .chip a {
  color: inherit;
  text-decoration: none;
}

/* Recent papers strip */
.recent-strip {
  display: grid;
  gap: 0;
  margin: 1em 0 2em 0;
}
.recent-row {
  display: grid;
  grid-template-columns: 70px 1fr auto;
  gap: 1em;
  padding: 0.8em 0;
  border-bottom: 1px solid var(--border);
  align-items: baseline;
}
.recent-row:last-child {
  border-bottom: none;
}
.recent-row .yr {
  font-size: 0.78em;
  font-weight: 700;
  color: var(--text-muted);
  letter-spacing: 0.05em;
}
.recent-row .ttl a {
  color: var(--text-primary);
  text-decoration: none;
  font-weight: 600;
  font-size: 0.98em;
  transition: color 0.15s;
}
.recent-row .ttl a:hover {
  color: var(--accent);
}
.recent-row .ttl .auths {
  display: block;
  color: var(--text-muted);
  font-size: 0.82em;
  font-weight: 400;
  margin-top: 0.15em;
}
.recent-row .vn {
  text-align: right;
  white-space: nowrap;
}

/* Tabs */
.tabs {
  margin: 1em 0 2em 0;
}
.tab-nav {
  display: flex;
  gap: 0;
  border-bottom: 2px solid var(--border);
  margin-bottom: 1.5em;
  flex-wrap: wrap;
}
.tab-nav button {
  background: none;
  border: none;
  padding: 0.7em 1.2em;
  font-size: 0.9em;
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
  font-size: 0.95em;
  color: var(--text-secondary);
  font-weight: 500;
  margin: 0 0 1.2em 0;
  font-style: italic;
}

/* Paper grid (in tabs) */
.paper-grid {
  display: grid;
  gap: 0;
}
.paper-row {
  display: grid;
  grid-template-columns: auto 1fr auto;
  gap: 1.2em;
  padding: 0.55em 0;
  border-bottom: 1px solid var(--border);
  align-items: center;
}
.paper-row:last-child { border-bottom: none; }
.paper-row .name { min-width: 130px; }
.paper-row .name a {
  font-weight: 600;
  font-size: 0.98em;
  color: var(--text-primary);
  text-decoration: none;
  transition: color 0.15s;
  white-space: nowrap;
}
.paper-row .name a:hover { color: var(--accent); }
.paper-row .desc {
  color: var(--text-secondary);
  font-size: 0.92em;
}
.paper-row .venue { text-align: right; }

/* Venue badges */
.venue-badge, .paper-row .venue span, .recent-row .vn span {
  display: inline-block;
  padding: 0.25em 0.65em;
  border-radius: 4px;
  font-size: 0.72em;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}
.venue-iclr    { background: #e0f2fe; color: #0369a1; }
.venue-neurips { background: #fce7f3; color: #be185d; }
.venue-colm    { background: #d1fae5; color: #047857; }
.venue-tmlr    { background: #fef3c7; color: #b45309; }
.venue-tacl    { background: #ede9fe; color: #6d28d9; }
.venue-aaai    { background: #fee2e2; color: #b91c1c; }
.venue-jmlr    { background: #e0e7ff; color: #4338ca; }
.venue-arxiv   { background: #f3f4f6; color: #4b5563; }
.venue-acl     { background: #dcfce7; color: #15803d; }
.venue-icml    { background: #dbeafe; color: #1d4ed8; }
.venue-emnlp   { background: #ccfbf1; color: #0f766e; }
.venue-aacl    { background: #fef9c3; color: #a16207; }
.venue-naacl   { background: #ffe4e6; color: #9f1239; }
.venue-procedia{ background: #e7e5e4; color: #44403c; }
.venue-oral, .venue-award {
  background: linear-gradient(90deg, #f59e0b, #ef4444);
  color: white;
}

/* CTA */
.cta {
  background: var(--bg-card);
  padding: 1.5em 2em;
  border-radius: 12px;
  border: 1px solid var(--border);
  text-align: center;
  margin: 2em 0 1em 0;
}
.cta strong { color: var(--accent); }
.cta a {
  color: var(--accent);
  text-decoration: none;
  font-weight: 600;
}
</style>

<h1 class="hero-title">Pierre Colombo</h1>
<div class="hero-subtitle">
  <span class="now">🚀 Member of Technical Staff · Cohere</span>
  <span class="past">ex-Founder Equall · ex-Associate Prof CentraleSupélec</span>
</div>
<p class="hero-text">
I'm a <strong>builder of AI labs, AI companies, and large open models</strong>. I currently train <strong>multimodal models</strong> at <a href="https://cohere.com/">Cohere</a>. Previously, I co-founded <a href="https://equall.ai/">Equall</a> (legal AI, SaulLM) and founded the <strong>NLP research group at CentraleSupélec</strong> from scratch — leading EuroLLM, EuroBERT, CroissantLLM, ColPali, and TowerLLM with 20+ researchers and \$6M+ in compute.
</p>

<div class="stats-banner">
  <div class="stat"><span class="num">6.8K+</span><span class="label">Citations</span></div>
  <div class="stat"><span class="num">35</span><span class="label">h-index</span></div>
  <div class="stat"><span class="num">48</span><span class="label">i10-index</span></div>
  <div class="stat"><span class="num">100+</span><span class="label">Papers</span></div>
  <div class="source">Source: <a href="https://scholar.google.com/citations?user=yPoMt8gAAAAJ&hl=fr">Google Scholar</a> · updated 2026</div>
</div>

<h2 class="section-h"><span class="kicker">Track record</span>What I've built</h2>

<div class="builder-grid">

  <div class="builder-card now">
    <div class="when">2025 — Now</div>
    <div class="role">Member of Technical Staff · Multimodal</div>
    <div class="where">Cohere</div>
    <div class="body">
    Training frontier <strong>multimodal models</strong> (vision-language) at Cohere. Working on the data, training, and evaluation stack for production-grade VLMs.
    </div>
    <div class="highlights">
      <span class="chip">VLM pretraining</span>
      <span class="chip">Multimodal data</span>
      <span class="chip">Production scale</span>
    </div>
  </div>

  <div class="builder-card">
    <div class="when">2023 — 2025</div>
    <div class="role">Co-Founder & Chief Science Officer</div>
    <div class="where">Equall · Paris / NYC</div>
    <div class="body">
    Co-founded Equall <strong>from zero</strong> — the first legal AI company built on a domain-specific LLM. <strong>Raised funding</strong>, hired the science team, built the legal data pipeline (500B+ tokens), trained the <strong>SaulLM family (7B → 141B)</strong> on a 512-GPU cluster, shipped the M&A due-diligence product to Big Law, and led the strategic pivot. Featured in <a href="https://www.lemondedudroit.fr/professions/337-legaltech/92756-ia-saul-instruct-un-llm-dedie-au-droit.html">Le Monde du Droit</a>.
    </div>
    <div class="highlights">
      <a class="chip" href="https://arxiv.org/abs/2403.03883">SaulLM-7B</a>
      <a class="chip" href="https://arxiv.org/abs/2407.19584">SaulLM-141B · NeurIPS 24</a>
      <span class="chip">512-GPU training</span>
      <span class="chip">Seed → Product</span>
    </div>
  </div>

  <div class="builder-card">
    <div class="when">2022 — 2025</div>
    <div class="role">Associate Professor · Founder of the NLP Group</div>
    <div class="where">CentraleSupélec · Université Paris-Saclay</div>
    <div class="body">
    <strong>Founded the NLP research group from scratch</strong>. Grew it to <strong>20+ researchers</strong> across 6 PhD students (now at Mistral, Meta FAIR, Reflection AI, Sword Health) and 3 MSc students. Secured <strong>\$6.1M in compute grants</strong> (Jean Zay, MareNostrum, Adastra) and <strong>\$1M industrial funding</strong>. Led EuroLLM, EuroBERT, CroissantLLM, ColPali, TowerLLM. Book Chair, ACL 2024. 700+ hours teaching across CentraleSupélec, Telecom Paris, EPFL, IP Paris.
    </div>
    <div class="highlights">
      <span class="chip">20+ researchers</span>
      <span class="chip">6 PhD advised</span>
      <span class="chip">\$6.1M compute</span>
      <span class="chip">\$1M industrial</span>
      <span class="chip">ACL 2024 Book Chair</span>
    </div>
  </div>

</div>

<h2 class="section-h"><span class="kicker">Recent · 2025–2026</span>What's hot off the press</h2>

<div class="recent-strip">

  <div class="recent-row">
    <div class="yr">ICLR 2026</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2507.00994">Should We Still Pretrain Encoders with Masked Language Modeling?</a>
      <span class="auths">H. Gisserot-Boukhlef, N. Boizard, M. Faysse, D.M. Alves, E. Malherbe, …, P. Colombo</span>
    </div>
    <div class="vn"><span class="venue-iclr">ICLR 26</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">ICML 2026</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2510.01149">ModernVBERT: Towards Smaller Visual Document Retrievers</a>
      <span class="auths">P. Teiletche, Q. Macé, M. Conti, A. Loison, G. Viaud, <b>P. Colombo</b>, M. Faysse</span>
    </div>
    <div class="vn"><span class="venue-icml">ICML 26</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">EMNLP 2025</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2505.24782">Context is Gold to find the Gold Passage: Evaluating and Training Contextual Document Embeddings</a>
      <span class="auths">M. Conti, M. Faysse, G. Viaud, A. Bosselut, C. Hudelot, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-oral">Oral · EMNLP 25</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">COLM 2025</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2503.05500">EuroBERT: Scaling Multilingual Encoders for European Languages</a>
      <span class="auths">N. Boizard, H. Gisserot-Boukhlef, D.M. Alves, A. Martins, …, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-colm">COLM 25</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">2026</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2602.05879">EuroLLM-22B: Technical Report</a>
      <span class="auths">M.M. Ramos, D.M. Alves, H. Gisserot-Boukhlef, J. Alves, P.H. Martins, …, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-arxiv">arXiv 26</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">2026</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2604.02045">BidirLM: From Text to Omnimodal Bidirectional Encoders by Adapting and Composing Causal LLMs</a>
      <span class="auths">N. Boizard, T. Deschamps-Berger, H. Gisserot-Boukhlef, C. Hudelot, …, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-arxiv">arXiv 26</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">2026</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2604.09497">BERT-as-a-Judge: A Robust Alternative to Lexical Methods for Efficient Reference-Based LLM Evaluation</a>
      <span class="auths">H. Gisserot-Boukhlef, N. Boizard, E. Malherbe, C. Hudelot, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-arxiv">arXiv 26</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">2025</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2512.18658">Does It Tie Out? Towards Autonomous Legal Agents in Venture Capital</a>
      <span class="auths"><b>P. Colombo</b>, M. Boudiaf, A. Sweet, M. Desa, H. Wang, K. Candra, …</span>
    </div>
    <div class="vn"><span class="venue-arxiv">arXiv 25</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">2025</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2510.21849">TowerVision: Understanding and Improving Multilinguality in Vision-Language Models</a>
      <span class="auths">A.G. Viveiros, P. Fernandes, S. Santos, S. Sannigrahi, E. Zaranis, …, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-arxiv">arXiv 25</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">2025</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2509.22193">When Does Reasoning Matter? A Controlled Study of Reasoning's Contribution to Model Performance</a>
      <span class="auths">N. Boizard, H. Gisserot-Boukhlef, K. El-Haddad, C. Hudelot, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-arxiv">arXiv 25</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">2025</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2506.04079">EuroLLM-9B: Technical Report</a>
      <span class="auths">P.H. Martins, J. Alves, P. Fernandes, N.M. Guerreiro, R. Rei, A. Farajian, …, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-arxiv">arXiv 25</span></div>
  </div>

  <div class="recent-row">
    <div class="yr">2025</div>
    <div class="ttl">
      <a href="https://arxiv.org/abs/2409.16235">EuroLLM: Multilingual Language Models for Europe</a>
      <span class="auths">P.H. Martins, P. Fernandes, J. Alves, N.M. Guerreiro, R. Rei, D.M. Alves, …, <b>P. Colombo</b></span>
    </div>
    <div class="vn"><span class="venue-procedia">Procedia 25</span></div>
  </div>

</div>

<h2 class="section-h"><span class="kicker">Research themes</span>What I work on</h2>

<p class="hero-text" style="margin-bottom: 1.2em;">
I build models and methods that are <strong>open</strong>, <strong>multilingual</strong>, and <strong>useful in the real world</strong>. Below are the threads — pick one to explore.
</p>

<div class="tabs">
  <div class="tab-nav">
    <button class="active" onclick="switchTab(event, 'multimodal')">🖼️ Multimodal</button>
    <button onclick="switchTab(event, 'llm')">🌍 Multilingual LLMs</button>
    <button onclick="switchTab(event, 'eval')">📊 Evaluation</button>
    <button onclick="switchTab(event, 'safe')">🛡️ Safe & Fair AI</button>
  </div>

  <div id="multimodal" class="tab-panel active">
    <h4>Vision-language models and document retrieval</h4>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2407.01449">ColPali</a></div>
        <div class="desc">SOTA document retrieval with vision-language — State of AI Report 2024</div>
        <div class="venue"><span class="venue-iclr">ICLR 25</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2510.01149">ModernVBERT</a></div>
        <div class="desc">Smaller visual document retrievers, distilled from ColPali</div>
        <div class="venue"><span class="venue-icml">ICML 26</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2510.21849">TowerVision</a></div>
        <div class="desc">Multilinguality in vision-language models</div>
        <div class="venue"><span class="venue-arxiv">arXiv 25</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2604.02045">BidirLM</a></div>
        <div class="desc">Omnimodal bidirectional encoders from causal LLMs</div>
        <div class="venue"><span class="venue-arxiv">arXiv 26</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://aclanthology.org/2021.emnlp-main.21/">MultimodalFusion</a></div>
        <div class="desc">Mutual dependency maximisation for multimodal fusion</div>
        <div class="venue"><span class="venue-oral">Oral · EMNLP</span></div>
      </div>
    </div>
  </div>

  <div id="llm" class="tab-panel">
    <h4>Open multilingual large language models</h4>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2602.05879">EuroLLM-22B</a></div>
        <div class="desc">Scaling EuroLLM to 22B for all EU languages</div>
        <div class="venue"><span class="venue-arxiv">arXiv 26</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2506.04079">EuroLLM-9B</a></div>
        <div class="desc">9B LLM competitive with LLaMA 3 on EU languages</div>
        <div class="venue"><span class="venue-arxiv">arXiv 25</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2503.05500">EuroBERT</a></div>
        <div class="desc">General-purpose encoder for European languages</div>
        <div class="venue"><span class="venue-colm">COLM 25</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2402.00786">CroissantLLM</a></div>
        <div class="desc">First bilingual French-English LLM</div>
        <div class="venue"><span class="venue-tmlr">TMLR 25</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2402.17733">TowerLLM</a></div>
        <div class="desc">GPT-4 translation quality with a 7B model</div>
        <div class="venue"><span class="venue-oral">Oral · COLM</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2403.03883">SaulLM-7B / 141B</a></div>
        <div class="desc">Pioneering LLM family for legal text</div>
        <div class="venue"><span class="venue-neurips">NeurIPS 24</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2402.12030">Universal Distillation</a></div>
        <div class="desc">Cross-tokenizer distillation for LLMs</div>
        <div class="venue"><span class="venue-tmlr">TMLR 25</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2211.05100">BLOOM</a></div>
        <div class="desc">176B open multilingual language model</div>
        <div class="venue"><span class="venue-jmlr">JMLR</span></div>
      </div>
    </div>
  </div>

  <div id="eval" class="tab-panel">
    <h4>Measuring what matters in NLP systems</h4>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2604.09497">BERT-as-a-Judge</a></div>
        <div class="desc">Robust alternative to lexical methods for LLM evaluation</div>
        <div class="venue"><span class="venue-arxiv">arXiv 26</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2509.22193">When Reasoning Matters</a></div>
        <div class="desc">Controlled study of reasoning's contribution to performance</div>
        <div class="venue"><span class="venue-arxiv">arXiv 25</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2505.24782">Context is Gold</a></div>
        <div class="desc">Evaluating and training contextual document embeddings</div>
        <div class="venue"><span class="venue-oral">Oral · EMNLP 25</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2310.10482">xCOMET</a></div>
        <div class="desc">Fine-grained translation evaluation</div>
        <div class="venue"><span class="venue-tacl">TACL</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2112.01589">InfoLM</a></div>
        <div class="desc">Information-theoretic generation metrics</div>
        <div class="venue"><span class="venue-award">🏆 Best Paper · AAAI 22</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2202.03799">Benchmarking</a></div>
        <div class="desc">New perspectives on NLP benchmarking</div>
        <div class="venue"><span class="venue-neurips">NeurIPS</span></div>
      </div>
    </div>
  </div>

  <div id="safe" class="tab-panel">
    <h4>Robust, fair, and safe NLP systems</h4>
    <div class="paper-grid">
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2303.16104">Hallucinations</a></div>
        <div class="desc">Hallucinations in large multilingual MT models</div>
        <div class="venue"><span class="venue-tacl">TACL</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2211.13527">OOD Detection</a></div>
        <div class="desc">Beyond Mahalanobis for textual OOD detection</div>
        <div class="venue"><span class="venue-neurips">NeurIPS</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://arxiv.org/abs/2310.14001">Attack Detection</a></div>
        <div class="desc">Stronger textual adversarial detectors</div>
        <div class="venue"><span class="venue-emnlp">EMNLP</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://aclanthology.org/2021.acl-long.511/">Disentanglement</a></div>
        <div class="desc">Fair generation via mutual information</div>
        <div class="venue"><span class="venue-oral">Oral · ACL</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://proceedings.mlr.press/v162/pichler22a.html">KNIFE</a></div>
        <div class="desc">Kernelized-neural differential entropy estimation</div>
        <div class="venue"><span class="venue-oral">Oral · ICML</span></div>
      </div>
      <div class="paper-row">
        <div class="name"><a href="https://proceedings.neurips.cc/paper_files/paper/2020/hash/2cfa3753d6a524711acb5fce38eeca1a-Abstract.html">Heavy-tailed</a></div>
        <div class="desc">Robust text classification</div>
        <div class="venue"><span class="venue-neurips">NeurIPS</span></div>
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

<div class="cta">
<strong>Let's build together. 🤝</strong> Open to collaborations on multimodal models, multilingual LLMs, evaluation, and applied AI.<br>
Reach me at <a href="mailto:colombo.pierre@gmail.com">colombo.pierre@gmail.com</a> · <a href="https://scholar.google.com/citations?user=yPoMt8gAAAAJ&hl=fr">Scholar</a> · <a href="https://www.linkedin.com/in/pierre-colombo/">LinkedIn</a>
</div>
