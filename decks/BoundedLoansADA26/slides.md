<!-- .slide: class="title-slide" -->
# The Effects of Present Bias and Loss Aversion over Loan Granting.
</section>

---
<!-- .slide: class="slide-heading" -->
## Research Questions

<section>
  <style>
    .rq-wrap {
      max-width: 1000px; margin: 0 auto;
      padding: clamp(8px, 2vw, 18px);
    }
    .rq-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: clamp(12px, 2.2vw, 18px);
    }
    .rq-card {
      position: relative;
      background: linear-gradient(180deg, #ffffff, #fbfdff);
      border: 1px solid #e6eaef;
      border-radius: 16px;
      padding: clamp(14px, 2.2vw, 22px) clamp(16px, 2.4vw, 26px);
      box-shadow: 0 6px 20px rgba(0,0,0,.06);
    }
    /* Number badge */
    .rq-badge {
      position: absolute; inset: -12px auto auto -12px;
      width: 40px; height: 40px; border-radius: 999px;
      display: grid; place-items: center;
      background: #0d5e3a; color: #fff; font-weight: 800;
      box-shadow: 0 8px 18px rgba(13,94,58,.25);
      font-size: 18px;
    }
    .rq-title {
      font-size: clamp(22px, 2.6vw, 30px);
      line-height: 1.2; margin: 0 0 6px 0; font-weight: 800;
      letter-spacing: .2px;
    }
    .rq-sub {
      color: #5b6573; font-size: clamp(16px, 1.8vw, 18px);
      line-height: 1.35; margin: 0;
    }
    /* Light accent bar */
    .rq-card::after {
      content: ""; position: absolute; inset: auto 0 0 0; height: 6px;
      background: linear-gradient(90deg, #0d5e3a 0%, #7fb18f 60%, #b9d7c8 100%);
      border-radius: 0 0 16px 16px; opacity: .85;
    }
    /* Fragments: bottom-to-top reveal */
    .rq-card[data-fragment-index="0"] { z-index: 3; }
    .rq-card[data-fragment-index="1"] { z-index: 2; }
    .rq-card[data-fragment-index="2"] { z-index: 1; }
    /* Dark-mode friendly tweak (optional) */
    :root.dark .rq-card { background:#0f141a; border-color:#2a3441; }
    :root.dark .rq-sub { color:#c7d1dd; }
    :root.dark .rq-card::after { opacity:.6; }
  </style>

  <div class="rq-wrap">
    <div class="rq-grid">
      <!-- Q3 -->
      <div class="rq-card fragment" data-fragment-index="2">
        <div class="rq-badge">3</div>
        <h3 class="rq-title">Can the deviation from rationality be reconciled?</h3>
        <p class="rq-sub">If biases exist, could incentive readjustments restore alignment with optimal lending?</p>
      </div>
      <!-- Q2 -->
      <div class="rq-card fragment" data-fragment-index="1">
        <div class="rq-badge">2</div>
        <h3 class="rq-title">Are we observing a systematic bias?</h3>
        <p class="rq-sub">Focus on <em>loss aversion</em> and <em>present bias</em> in loan-decision-making.</p>
      </div>
      <!-- Q1 -->
      <div class="rq-card fragment" data-fragment-index="0">
        <div class="rq-badge">1</div>
        <h3 class="rq-title">To what degree are loan officers rational decision makers?</h3>
        <p class="rq-sub">Benchmark observed choices against normative, information-consistent decisions.</p>
      </div>
    </div>
  </div>
</section>


---
<!-- .slide: class="slide-heading clear-logo" -->
## What does this research do?

<style>
  .reveal .clear-logo > h2{
    max-width: 82%;          /* right edge stops before the logo */
    margin-inline: auto;     /* stay centered */
    padding-top: 0.45em;     /* drop below the logo band */
  }
</style>

<section id="gif3cols">
  <style>
    #gif3cols .wrap{
      --side-gutter: clamp(20px, 3.5vw, 40px);
      --col-gap:     clamp(16px, 3vw, 28px);
      box-sizing: border-box;
      inline-size: 100%;
      max-inline-size: 1200px;          /* optional hard cap */
      margin-inline: auto;
      padding-inline: var(--side-gutter);
      /* Final safety against any 1px rounding */
      overflow: clip;
    }
    #gif3cols .grid{
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      column-gap: var(--col-gap);
      row-gap: var(--col-gap);
      align-items: center;
      justify-items: center;
      /* Don’t allow the grid to grow past its container */
      max-inline-size: 100%;
      overflow: clip;
      box-sizing: border-box;
    }
    #gif3cols .card{
      inline-size: 100%;    /* fill its grid cell only */
      aspect-ratio: 4 / 3;  /* equal visual height across columns */
      border-radius: 14px;
      background: #fff;
      box-shadow: 0 2px 12px rgba(0,0,0,.12);
      overflow: hidden;     /* in case GIF frames exceed */
      display: flex;
      align-items: center;
      justify-content: center;
    }
    #gif3cols .card img{
      display: block;
      inline-size: 100%;
      block-size: 100%;
      object-fit: contain;  /* use 'cover' to fill/crop instead */
      background: #fff;
    }
    @media (max-width: 900px){
      #gif3cols .grid{ grid-template-columns: repeat(2, minmax(0,1fr)); }
    }
    @media (max-width: 600px){
      #gif3cols .grid{ grid-template-columns: 1fr; }
    }
  </style>
  <div class="wrap">
    <div class="grid">
      <div class="card">
        <img src="./images/homer-simpson.gif" alt="Homer 1">
      </div>
      <div class="card">
        <img src="./images/homer-simpson-crayon.gif" alt="Homer 2">
      </div>
      <div class="card">
        <img src="./images/the-simpsons-homer-simpson.gif" alt="Homer 3">
      </div>
    </div>
  </div>
</section>

---
<!-- .slide: class="slide-heading clear-logo" -->
## Optimal Decisions Start at the First Line

<section>
  <!-- Funnel → Forked Outcomes (no title) -->
  <div class="smart-funnel" aria-label="First-line process funnel with forked outcomes">
    <div class="funnel">
      <div class="band band-1 fragment" data-fragment-index="2">
        <span>Can that deviation be reconciled?</span>
      </div>
      <div class="band band-2 fragment" data-fragment-index="1">
        <span>Biased decision makers influence the portfolio mix.</span>
      </div>
      <div class="band band-3 fragment" data-fragment-index="0">
        <span>Objective information input: hard &amp; soft information → loan decisions</span>
      </div>
      <div class="neck" aria-hidden="true"></div>
    </div>
    <div class="fork">
      <div class="lane lane-good">
        <div class="lane-track">
          <div class="pill">Aligned incentives → prudent lending</div>
          <div class="end-cap end-good" aria-hidden="true"></div>
        </div>
      </div>
      <div class="lane lane-bad">
        <div class="lane-track">
          <div class="pill">Misaligned incentives → excessive lending</div>
          <div class="pill">Credit risk materializes → bankruptcy</div>
          <div class="badge-loss" role="note" aria-label="30 percent of loans unrecovered post-bankruptcy">
            <strong>≈30%</strong><span> unrecovered<br>post-bankruptcy</span>
          </div>
          <div class="end-cap end-bad" aria-hidden="true"></div>
        </div>
      </div>
    </div>
  </div>
</section>

---
<!-- .slide: class="slide-heading clear-logo" -->
## The "Rational" Banking process

<div class="media-xy">
  <img data-src="./images/Figure1.png" class="img-sm" alt="Rational banking process diagram">
</div>

---
<!-- .slide: class="slide-heading clear-logo" -->
## Heuristics in the Banking Process (1/2)

<div class="media-xy">
  <img data-src="./images/Figure4.png" class="img-sm" alt="Heuristics in the banking process">
</div>

--
<!-- .slide: class="slide-heading clear-logo" -->
## Heuristics in the Banking Process (2/2)

<div class="media-xy">
  <img data-src="./images/Figure6.png" class="img-sm" alt="Heuristics in the banking process, part 2">
</div>

---
<!-- .slide: class="slide-heading" -->
## The Behavioral Value of a Loan Decision

<style>
  #bvalue, #vchoice { --ivey:#0d5e3a; --ivey2:#7fb18f; --blue:#0b3d5c; --ink:#5b6573; }
  #bvalue .row{ display:flex; gap:clamp(8px,1.4vw,16px); align-items:stretch;
    justify-content:center; max-width:1120px; margin:.4em auto 0; flex-wrap:wrap; }
  #bvalue .card{ position:relative; flex:1 1 0; min-width:230px;
    background:linear-gradient(180deg,#fff,#fbfdff); border:1px solid #e6eaef;
    border-radius:14px; padding:16px 16px 18px; box-shadow:0 6px 18px rgba(0,0,0,.06); }
  #bvalue .card .badge{ position:absolute; top:-15px; left:-15px; width:38px; height:38px;
    border-radius:999px; background:var(--ivey); color:#fff; display:grid; place-items:center;
    box-shadow:0 6px 14px rgba(13,94,58,.28); }
  #bvalue .card h4{ margin:.1em 0 .4em; font-size:clamp(15px,1.6vw,18px); font-weight:800; }
  #bvalue .card p{ margin:0; color:var(--ink); font-size:clamp(13px,1.35vw,15px); line-height:1.35; }
  #bvalue .card::after{ content:""; position:absolute; left:0; right:0; bottom:0; height:5px;
    border-radius:0 0 14px 14px; background:linear-gradient(90deg,var(--ivey),var(--ivey2)); }
  #bvalue .times{ align-self:center; font-size:26px; color:var(--ivey); font-weight:700; }
  #bvalue .foot{ text-align:center; color:#7a8694; font-size:clamp(12px,1.3vw,14px); margin-top:.9em; }
  @media (max-width:900px){ #bvalue .times{ display:none; } }
</style>

<p style="text-align:center; color:#5b6573; max-width:1000px; margin:.1em auto .5em;">For loan \(i\), the value of action \(a\in\{\text{Approve},\text{Reject}\}\) folds <strong>three behavioral channels</strong> into one utility value:</p>

<div style="text-align:center; margin:.4em auto .2em;">
\(\displaystyle U_{i,a,t}=\underbrace{w_{\gamma}(\hat p_i)}_{\text{weighting}}\;\underbrace{D(t_{a,R})}_{\text{timing}}\;\underbrace{v\!\big(x_{i,a,R,t}\big)}_{\text{value}}\;+\;\big[1-w_{\gamma}(\hat p_i)\big]\,D(t_{a,D})\,v\!\big(x_{i,a,D,t}\big)\)
</div>

<div id="bvalue">
  <div class="row">
    <div class="card">
      <div class="badge">\(w\)</div>
      <h4>Probability weighting</h4>
      <p>\(w_{\gamma}(p)=\dfrac{p^{\gamma}}{[\,p^{\gamma}+(1-p)^{\gamma}\,]^{1/\gamma}}\), on the <em>perceived</em> repayment \(\hat p_i=m(\Omega_i)\). Collateral overweighting enters here.</p>
    </div>
    <div class="times">×</div>
    <div class="card">
      <div class="badge">\(D\)</div>
      <h4>Present-biased timing</h4>
      <p>\(D(t)=\beta\delta^{t}\) with \(D(0)=1\). Present bias \(\beta\in(0,1]\), long-run patience \(\delta\in(0,1]\).</p>
    </div>
    <div class="times">×</div>
    <div class="card">
      <div class="badge">\(v\)</div>
      <h4>Reference-dependent value</h4>
      <p>\(v(x)=x^{\alpha}\) for \(x\ge0\), else \(-\lambda(-x)^{\alpha}\); \(\alpha\in(0,1]\), \(\lambda\ge1\). Payoffs \(x=c-r_t\).</p>
    </div>
  </div>
  <p class="foot">Evaluated within a satisficing consideration set \(S_t\subseteq A_t\) (De Clippel ancillary conditions).</p>
</div>

---
<!-- .slide: class="slide-heading" -->
## From Value to Choice — and the Treatment Lever

<style>
  #vchoice .note{ text-align:center; color:#5b6573; font-size:clamp(13px,1.4vw,16px);
    margin:.3em auto .7em; max-width:1000px; }
  #vchoice .levers{ display:flex; gap:clamp(10px,1.8vw,20px); justify-content:center;
    align-items:stretch; max-width:1080px; margin:0 auto; flex-wrap:wrap; }
  #vchoice .lever{ position:relative; flex:1 1 0; min-width:260px;
    background:linear-gradient(180deg,#fff,#fbfdff); border:1px solid #e6eaef;
    border-radius:14px; padding:16px 18px 18px; box-shadow:0 6px 18px rgba(0,0,0,.06); }
  #vchoice .lever .badge{ position:absolute; top:-15px; left:-15px; width:40px; height:40px;
    border-radius:999px; background:var(--blue); color:#fff; display:grid; place-items:center;
    box-shadow:0 6px 14px rgba(11,61,92,.28); }
  #vchoice .lever h4{ margin:.1em 0 .4em; font-size:clamp(15px,1.7vw,19px); font-weight:800; }
  #vchoice .lever p{ margin:0; color:var(--ink); font-size:clamp(13px,1.4vw,15px); line-height:1.4; }
  #vchoice .lever::after{ content:""; position:absolute; left:0; right:0; bottom:0; height:5px;
    border-radius:0 0 14px 14px; background:linear-gradient(90deg,var(--blue),#5b86a6); }
  #vchoice .result{ text-align:center; margin:.9em auto 0; font-weight:700; color:var(--ivey);
    font-size:clamp(14px,1.5vw,17px); }
</style>

<p style="text-align:center; color:#5b6573; max-width:1000px; margin:.1em auto .4em;">The officer approves when approval dominates rejection; observed choice follows a logit:</p>

<div style="text-align:center; margin:.4em auto .2em;">
\(\displaystyle \Pr(\text{Approve}_i)=\frac{\exp(\mu\,\Delta U_{i,t})}{1+\exp(\mu\,\Delta U_{i,t})},\qquad \Delta U_{i,t}=U_{i,\text{Approve},t}-U_{i,\text{Reject},t}\)
</div>

<div id="vchoice">
  <p class="note">Approve iff \(\Delta U_{i,t}>0\) &nbsp;·&nbsp; \(\mu\) = choice consistency &nbsp;·&nbsp; <strong>Ranking task:</strong> order loans by \(\Delta U_{i,t}\) (rank-order logit)</p>
  <div class="levers">
    <div class="lever">
      <div class="badge">\(D\)</div>
      <h4>Timing</h4>
      <p>A delayed bonus discounts the immediate gain: \(D(t)=\beta\delta^{t}\).</p>
    </div>
    <div class="lever">
      <div class="badge">\(\kappa\)</div>
      <h4>Loss exposure</h4>
      <p>Penalty \(\kappa_t>0\) turns a bad approval into a reference-point loss, \(x_{i,\text{Approve},D,t}=B_i-\kappa_t L_i-r_t<0\), activating \(v(x)=-\lambda(-x)^{\alpha}\).</p>
    </div>
  </div>
  <p class="result">→ deactivates present bias, with no change to true risk</p>
</div>

---
<!-- .slide: class="slide-heading" -->
## Experimental Design

<section data-background-color="transparent">
  <style>
    /* Segmented Toggle — Ivey-friendly */
    .seg-wrap {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 80%;
    }
    .seg-pill {
      display: inline-flex;
      border: 1px solid var(--seg-border, rgba(0,0,0,0.15));
      border-radius: 999px;
      overflow: hidden;
      box-shadow: 0 1px 6px rgba(0,0,0,0.06);
      backdrop-filter: saturate(1.1);
      font-weight: 600;
      letter-spacing: 0.2px;
    }
    .seg {
      padding: 14px 28px;
      min-width: 220px;
      text-align: center;
      user-select: none;
      transition: transform 220ms ease, background 180ms ease, color 180ms ease, box-shadow 180ms ease;
      background: var(--seg-bg, rgba(255,255,255,0.65));
      color: var(--seg-fg, #222);
    }
    .seg + .seg {
      border-left: 1px solid var(--seg-divider, rgba(0,0,0,0.08));
    }
    /* Keep fragments visible; only the active one gets emphasis */
    .seg.fragment { opacity: 1; }
    .seg.fragment.current-fragment {
      background: var(--ivey-green, #0d5e3a);
      color: #fff;
      box-shadow: inset 0 0 0 1px rgba(255,255,255,0.25), 0 4px 14px rgba(13,94,58,0.35);
      transform: scale(1.02);
    }
    /* Hover/press polish (optional) */
    .seg:hover { transform: translateY(-1px); }
    .seg:active { transform: translateY(0); }
    /* Title style (optional, matches Ivey minimalism) */
    .seg-title {
      text-align: center;
      margin-bottom: 18px;
      font-weight: 700;
      letter-spacing: 0.3px;
      opacity: 0.9;
    }
    @media (max-width: 880px) {
      .seg { min-width: 140px; padding: 12px 18px; }
    }
  </style>

  <div class="seg-wrap">
    <div>
      <div class="seg-title">Experiments:</div>
      <div class="seg-pill">
        <!-- Step 1 highlights LAB, Step 2 highlights FIELD -->
        <div class="seg fragment" data-fragment-index="1">Lab Experiment</div>
        <div class="seg fragment" data-fragment-index="2">Field Experiment</div>
      </div>
    </div>
  </div>
</section>

--
<!-- .slide: class="slide-heading" -->
## Experimental Design
<div class="seg-toggle" aria-label="Experiments">
  <div class="seg-pill">
    <div class="seg is-active">Lab Experiment</div>
    <div class="seg">Field Experiment</div>
  </div>
</div>

<table style="border-collapse:collapse; margin:auto;">
  <thead>
    <tr>
      <th style="border:1px solid #ccc; padding:6px;"></th>
      <th colspan="2" style="border:1px solid #ccc; padding:6px; text-align:center;">Time Delay</th>
    </tr>
    <tr>
      <th style="border:1px solid #ccc; padding:6px; text-align:left;">Incentive Adjustment</th>
      <th style="border:1px solid #ccc; padding:6px; text-align:center;">Yes</th>
      <th style="border:1px solid #ccc; padding:6px; text-align:center;">No</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border:1px solid #ccc; padding:6px;"><strong>Yes</strong></td>
      <td style="border:1px solid #ccc; padding:6px; text-align:center;">Time Delay | Incentive Adjustment</td>
      <td style="border:1px solid #ccc; padding:6px; text-align:center;">No Time Delay | Incentive Adjustment</td>
    </tr>
    <tr>
      <td style="border:1px solid #ccc; padding:6px;"><strong>No</strong></td>
      <td style="border:1px solid #ccc; padding:6px; text-align:center;">No Time Delay | Incentive Adjustment</td>
      <td style="border:1px solid #ccc; padding:6px; text-align:center;">No Time Delay | No Incentive Adjustment</td>
    </tr>
  </tbody>
</table>

--
<!-- .slide: class="slide-heading" -->
## Experimental Design
<div class="seg-toggle" aria-label="Experiments">
  <div class="seg-pill">
    <div class="seg is-active">Lab Experiment</div>
    <div class="seg">Field Experiment</div>
  </div>
</div>

<div class="r-stretch" style="display:flex; align-items:center; justify-content:center; overflow:auto;">
  <table style="border-collapse:collapse; margin:auto;">
    <thead>
      <tr>
        <th style="border:1px solid #ccc; padding:6px;">Subject Measure</th>
        <th style="border:1px solid #ccc; padding:6px;">Source</th>
      </tr>
    </thead>
    <tbody>
      <tr><td style="border:1px solid #ccc; padding:6px;">Risk Aversion</td>
          <td style="border:1px solid #ccc; padding:6px;">Holt and Laury, 2002</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">Short-term Impatience</td>
          <td style="border:1px solid #ccc; padding:6px;">Andreoni, 2012</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">Risk Seekingness</td>
          <td style="border:1px solid #ccc; padding:6px;">Eckel and Grossman, 2002</td></tr>
      <tr><td style="border:1px solid #ccc; padding:6px;">DOSPERT - Risk Taking</td>
          <td style="border:1px solid #ccc; padding:6px;">Blais and Weber, 2006</td></tr>
    </tbody>
  </table>
</div>

--
<!-- .slide: class="slide-heading" -->
## Experimental Design - A Decision Making Situation
<div class="seg-toggle" aria-label="Experiments">
  <div class="seg-pill">
    <div class="seg is-active">Lab Experiment</div>
    <div class="seg">Field Experiment</div>
  </div>
</div>

- Loan Officer Training in 5 minutes
- Decision making - rank from most to least chances of repayment (5 decisions)

<section>
<div class="panels">

  <div class="panel">
    <div class="panel-hd">CREDIT APPLICATION A</div>
    <div class="panel-bd">
      <table>
        <tr><td>Amount Requested</td><td><strong>$10,000.00</strong></td></tr>
        <tr><td>Term</td><td>36 periods</td></tr>
        <tr><td>Payment Frequency</td><td>Monthly <span style="padding:2px 6px; border:1px solid #c9ced6; border-radius:4px; background:#eef3f8;">X</span></td></tr>
        <tr><td>Installment (payment)</td><td><strong>$346.65</strong></td></tr>
        <tr><td>Purpose of Credit</td><td>Consumer</td></tr>
        <tr><td>Type of Collateral</td><td>Mortgage-backed</td></tr>
        <tr><td>Source of Income</td><td>Private employee (5 years)</td></tr>
        <tr><td>Score</td><td>AAA (950; positive bureau history – 10 years)</td></tr>
        <tr><td>Total Consolidated Risk</td><td><strong>$10,000.00</strong></td></tr>
      </table>
    </div>
  </div>

  <div class="panel">
    <div class="panel-hd">Payment Capacity Analysis</div>
    <div class="panel-bd">
      <table style="border-spacing:0 6px;">
        <thead>
          <tr>
            <th>Assets</th><th style="text-align:right;">Value</th>
            <th></th>
            <th>Liabilities</th><th style="text-align:right;">Value</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>Real Estate</td><td style="text-align:right;">$20,000.00</td><td></td><td>Secured Bank Debt</td><td style="text-align:right;">$19,120.89</td></tr>
          <tr><td>Other Assets</td><td style="text-align:right;">$10,000.00</td><td></td><td>Short-Term Liabilities</td><td style="text-align:right;">$953.75</td></tr>
        </tbody>
        <thead>
          <tr>
            <th>Income / Expense</th><th style="text-align:right;">Amount</th>
            <th></th>
            <th>Income / Expense</th><th style="text-align:right;">Amount</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>Income</td><td style="text-align:right;">$1,247.55</td><td></td><td>Financial Expenses</td><td style="text-align:right;">$459.80</td></tr>
          <tr><td>Family Expenses</td><td style="text-align:right;">$98.00</td><td></td><td>Net Savings</td><td style="text-align:right;"><strong>$689.75</strong></td></tr>
          <tr><td style="color:#5b6573;">Total Expenses</td><td style="text-align:right;">$557.80</td><td></td><td></td><td></td></tr>
        </tbody>
      </table>
    </div>
  </div>

</div>
</section>

--
<!-- .slide: class="slide-heading" -->
## Experimental Design
<div class="seg-toggle" aria-label="Experiments">
  <div class="seg-pill">
    <div class="seg">Lab Experiment</div>
    <div class="seg is-active">Field Experiment</div>
  </div>
</div>

--

<!-- .slide: class="slide-heading" -->
## Experimental Design
<div class="seg-toggle" aria-label="Experiments">
  <div class="seg-pill">
    <div class="seg">Lab Experiment</div>
    <div class="seg is-active">Field Experiment</div>
  </div>
</div>

<div class="vsteps-wrap">
  <ul class="vsteps">
    <li><span class="num">1</span>Loan Officers undergo a "regular" workshop.</li>
    <li><span class="num">2</span>Fill surveys (behavioral traits).</li>
    <li><span class="num">3</span>They have to make decision sets</li>
    <li><span class="num">4</span>Start an unrelated training.</li>
    <li><span class="num">5</span>HR provides Stimuli</li>
    <li><span class="num">6</span>They have to make decisions sets</li>
  </ul>
</div>

---
<!-- .slide: class="slide-heading" -->
## Preliminary Results

<!-- .slide: class="slide-heading" -->
<h2>Design & Sample Summary</h2>

<div style="max-width:900px; margin:0 auto; border:1px solid #c9ced6; border-radius:12px; overflow:hidden; box-shadow:0 2px 12px rgba(0,0,0,.06);">
  <div style="background:#0b3d5c; color:#fff; padding:10px 16px; font-weight:700; letter-spacing:.2px;">
    Study Setup
  </div>
  <div style="background:#f7f9fb;">
    <table style="width:100%; border-collapse:separate; border-spacing:0; font-size:1.02em;">
      <tbody>
        <tr>
          <th style="width:32%; text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Participants (n)</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;"><strong>42 loan officers</strong></td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Age range</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">25–45 years</td>
        </tr>
        <tr>
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Gender</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">17 male, 25 female</td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Experience (role)</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">2 months – 10 years</td>
        </tr>
        <tr>
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Context</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">During a scheduled training</td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Instruments</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">DOSPERT test; Holt–Laury risk test</td>
        </tr>
        <tr>
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Decision sets</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">Based on current bank standards, pre &amp; post stimuli</td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573;">Stimulus</th>
          <td style="padding:10px 14px;">HR announced a change to bonus calculation (vs. status quo)</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>


--

<div style="max-width:900px; margin:0 auto; border:1px solid #c9ced6; border-radius:12px; overflow:hidden; box-shadow:0 2px 12px rgba(0,0,0,.06);">
  <div style="background:#0b3d5c; color:#fff; padding:10px 16px; font-weight:700; letter-spacing:.2px;">
    Results & Interpretation
  </div>
  <div style="background:#f7f9fb;">
    <table style="width:100%; border-collapse:separate; border-spacing:0; font-size:1.02em;">
      <tbody>
        <tr>
          <th style="width:36%; text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Loan decision accuracy</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">
            <strong>↑ 46% → 53%</strong> when present bias was deactivated
          </td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Collective risk preferences</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">
            Shifted in the very short term, then converged back toward baseline
          </td>
        </tr>
        <tr>
          <th style="text-align:left; padding:10px 14px; color:#5b6573;">Statistical power</th>
          <td style="padding:10px 14px;">
            Study underpowered; ~<strong>290</strong> participants estimated for statistical significance
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</div>


--
<!-- .slide: class="slide-heading diagram closer" -->
# Better Decision Makers

<div class="media-xy">
  <img data-src="./images/Accuracy_2.png" class="img-sm" alt="Accuracy figure">
</div>

--
<!-- .slide: class="slide-heading diagram closer" -->
## Less willing to take risks (for a bit)

<div class="media-xy">
  <img data-src="./images/Risk_Preference_Trajectories.png" class="img-sm" alt="trajectories">
</div>

---
<!-- .slide: class="slide-heading" -->
## What the Simulations Show
<style>
  #simres{ --ivey:#0d5e3a; --blue:#0b3d5c; --ink:#5b6573; }
  #simres .wrap{ max-width:1120px; margin:.3em auto 0; border:1px solid #c9ced6;
    border-radius:14px; overflow:hidden; box-shadow:0 6px 20px rgba(0,0,0,.08); }
  #simres .hd{ background:var(--blue); color:#fff; padding:10px 16px; font-weight:700;
    display:flex; justify-content:space-between; align-items:center; gap:12px; flex-wrap:wrap; }
  #simres .hd small{ font-weight:500; opacity:.85; font-size:.74em; }
  #simres table{ width:100%; border-collapse:separate; border-spacing:0;
    font-size:clamp(13px,1.5vw,17px); background:#f7f9fb; }
  #simres th, #simres td{ padding:10px 14px; border-bottom:1px solid #e6eaef; text-align:left; }
  #simres thead th{ background:#eef3f7; color:var(--blue); font-weight:800; font-size:.9em; }
  #simres td.num, #simres th.num{ text-align:center; font-variant-numeric:tabular-nums; }
  #simres .cell{ font-weight:800; color:var(--ivey); }
  #simres .pb{ color:#b4532a; font-weight:700; }
  #simres .pat{ color:var(--ivey); font-weight:700; }
  #simres tr.target td{ background:#eafaf1; }
  #simres .foot{ text-align:center; color:#7a8694; font-size:clamp(11px,1.3vw,13px);
    margin:.7em auto 0; max-width:1040px; line-height:1.4; }
</style>
<div id="simres">
  <div class="wrap">
    <div class="hd"><span>Simulated profiles map onto the four treatments</span><small>one calibrated agent per profile · 100 choices each · 10,000 simulations</small></div>
    <table>
      <thead>
        <tr>
          <th>Condition</th>
          <th>Behavioral profile</th>
          <th class="num">Present bias \(\beta\)</th>
          <th class="num">Loss aversion \(\lambda\)</th>
          <th class="num">Risk-taking</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="cell">Control</td>
          <td>Risk-averse, <span class="pb">present-biased</span></td>
          <td class="num pb">0.30</td><td class="num">0.01</td><td class="num">54%</td>
        </tr>
        <tr>
          <td class="cell">Delay only</td>
          <td>Risk-averse, <span class="pat">patient</span></td>
          <td class="num pat">0.70</td><td class="num">0.01</td><td class="num">54%</td>
        </tr>
        <tr>
          <td class="cell">Incentive only</td>
          <td>Risk-seeking, <span class="pb">present-biased</span></td>
          <td class="num pb">0.10</td><td class="num">2.0</td><td class="num">59%</td>
        </tr>
        <tr class="target">
          <td class="cell">Delay + incentive</td>
          <td>Risk-averse, <span class="pat">patient</span>, loss-averse</td>
          <td class="num pat">0.80</td><td class="num">2.0</td><td class="num">58%</td>
        </tr>
      </tbody>
    </table>
  </div>
  <p class="foot">Risk-taking = share choosing the risky option across 100 simulated choices. Each treatment toggles present bias (via \(\beta\), the delay channel) and loss aversion (via \(\lambda\), the incentive channel); \(\alpha\) and \(\delta\) are held in the background.</p>
</div>

---
<!-- .slide: class="slide-heading" -->

## Thank you. 

