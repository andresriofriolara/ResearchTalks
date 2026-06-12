<!-- .slide: class="title-slide" -->
# The Effects of Present Bias and Loss Aversion over Loan Granting.

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
<!-- .slide: class="slide-heading closer" -->
## What does this research do?

<section id="paper-roadmap">
  <style>
    #paper-roadmap .wrap{
      max-width: 1050px;
      margin: 0 auto;
      padding: clamp(8px, 2vw, 18px);
    }
    #paper-roadmap .grid{
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: clamp(14px, 2.5vw, 24px);
    }
    #paper-roadmap .card{
      background: #fff;
      border: 1px solid #e6eaef;
      border-radius: 12px;
      box-shadow: 0 4px 16px rgba(0,0,0,.07);
      padding: clamp(16px, 2.2vw, 24px);
      min-height: 230px;
    }
    #paper-roadmap .num{
      width: 34px;
      height: 34px;
      border-radius: 999px;
      display: grid;
      place-items: center;
      background: #0d5e3a;
      color: #fff;
      font-weight: 800;
      margin-bottom: 12px;
    }
    #paper-roadmap h3{
      margin: 0 0 8px 0;
      font-size: clamp(20px, 2.1vw, 26px);
      line-height: 1.15;
    }
    #paper-roadmap p{
      margin: 0;
      color: #536071;
      font-size: clamp(16px, 1.65vw, 18px);
      line-height: 1.35;
    }
    @media (max-width: 900px){
      #paper-roadmap .grid{ grid-template-columns: 1fr; }
    }
  </style>
  <div class="wrap">
    <div class="grid">
      <div class="card">
        <div class="num">1</div>
        <h3>Builds the mechanism</h3>
        <p>Models lending decisions with reference-dependent valuation, probability weighting, quasi-hyperbolic discounting, and bounded attention.</p>
      </div>
      <div class="card">
        <div class="num">2</div>
        <h3>Tests the channel</h3>
        <p>Uses lab and field designs where incentive readjustments alter timing, loss exposure, and the perceived value of approval.</p>
      </div>
      <div class="card">
        <div class="num">3</div>
        <h3>Interprets preliminary evidence</h3>
        <p>Finds mechanism-consistent descriptive movement, while emphasizing limited power and the need for cautious causal interpretation.</p>
      </div>
    </div>
  </div>
</section>

---
<!-- .slide: class="slide-heading closer" -->
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
          <div class="pill">Credit risk materializes → bank bears losses</div>
          <div class="badge-loss" role="note" aria-label="Default risk creates an incentive for careful lending">
            <strong>Risk</strong><span> concentration<br>and exposure</span>
          </div>
          <div class="end-cap end-bad" aria-hidden="true"></div>
        </div>
      </div>
    </div>
  </div>
</section>

---
<!-- .slide: class="slide-heading closer" -->
## Why mortgage lending is the object of study

- The paper isolates lending decision-making by assuming one asset class: mortgages.
- Collateral is treated as a key information channel in loan granting.
- The central behavioral channel is not that collateral mechanically changes true repayment risk.
- The question is whether collateral changes the officer's perceived repayment probability and decision weight.

---
<!-- .slide: class="slide-heading closer" -->
## Financial Intermediation Toy Model

<div class="media-xy">
  <img data-src="./images/Figure1.png" class="img-sm" alt="Financial intermediation toy model baseline">
</div>

---
<!-- .slide: class="slide-heading diagram closer" -->
## Maturity Gap-Driven Modification

<div class="media-xy">
  <img data-src="./images/Figure2.png" class="img-sm" alt="Financial intermediation toy model with maturity gap modification and collateral influence">
</div>

--
<!-- .slide: class="slide-heading diagram closer" -->
## Conceptual Framework at the Bank Level

<div class="media-xy">
  <img data-src="./images/Figure3.png" class="img-sm" alt="Conceptual framework at a bank level">
</div>

--
<!-- .slide: class="slide-heading diagram closer" -->
## Individual Decision-Maker Channel

<div class="media-xy">
  <img data-src="./images/Figure4.png" class="img-sm" alt="Conceptual framework for the individual decision-maker">
</div>

---
<!-- .slide: class="slide-heading closer" -->
## The Behavioral Model

$$
\Omega_i
\longrightarrow
\hat p_i
\longrightarrow
w_{\gamma}(\hat p_i)
\longrightarrow
U_{i,a,t}
$$

- The loan officer observes loan information $\Omega_i$.
- That information forms a perceived repayment probability $\hat p_i$.
- Probability weighting and time-discounted reference-dependent valuation generate the behavioral value of each action.

--
<!-- .slide: class="slide-heading" -->
## Information and Perceived Risk

$$
\Omega_i=\{S_i,PMT_i,L_i,V^{asset}_i,Z_i\}
$$

$$
p_i=\Pr(R_i=1),
\qquad
\hat p_i=\Pr(R_i=1\mid \Omega_i)
$$

$$
\hat p_i=m(\Omega_i)
$$

- $p_i$ is the true repayment probability.
- $\hat p_i$ is the officer's perceived repayment probability.
- Collateral overweighting enters through $\hat p_i$, not by mechanically changing true risk.

--
<!-- .slide: class="slide-heading" -->
## Reference-Adjusted Payoffs

For each action-state pair $(a,s)$:

$$
x_{i,a,s,t}=c_{i,a,s,t}-r_t
$$

$$
v(x)=
\begin{cases}
x^{\alpha}, & x\geq 0,\\[4pt]
-\lambda(-x)^{\alpha}, & x<0
\end{cases}
$$

$$
\alpha\in(0,1],
\qquad
\lambda\geq 1
$$

$\alpha$ captures diminishing sensitivity. $\lambda$ captures loss aversion. $\beta$ is reserved for present bias.

--
<!-- .slide: class="slide-heading" -->
## Outcome Regions Are Not Primitive Utilities

<section>
  <style>
    .rw-matrix {
      max-width: 900px; margin: 0 auto; font-size: clamp(18px, 2vw, 24px);
    }
    .rw-matrix table {
      border-collapse: separate; border-spacing: 0; width: 100%;
      box-shadow: 0 6px 20px rgba(0,0,0,.08); border-radius: 12px; overflow: hidden;
    }
    .rw-matrix th, .rw-matrix td {
      padding: 14px 16px; text-align: center; vertical-align: middle;
      border: 1px solid #e5e7eb; background: #fff;
    }
    .rw-matrix thead th {
      background: #f8fafc; font-weight: 700;
    }
    .rw-matrix .stub { background: #f8fafc; font-weight: 700; width: 22%; }
    .rw-matrix .right { background: #ecfdf5; }
    .rw-matrix .wrong { background: #fef2f2; }
    .rw-matrix .tag {
      display: inline-block; padding: 2px 8px; border-radius: 999px; font-size: 0.85em;
      background: #e5e7eb; font-weight: 700;
    }
    .rw-matrix .right .tag { background: #34d39922; }
    .rw-matrix .wrong .tag { background: #f8717122; }
    .rw-matrix small { display:block; opacity:.85; margin-top:4px; line-height:1.1; }
  </style>

  <div class="rw-matrix">
    <table>
      <thead>
        <tr>
          <th class="stub"></th>
          <th><strong>Repay</strong></th>
          <th><strong>Default</strong></th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th class="stub">Approve</th>
          <td class="right">
            <span class="tag">\(v_1\)</span>
            <small>Approval of a good loan</small>
          </td>
          <td class="wrong">
            <span class="tag">\(v_2\)</span>
            <small>Approval of a bad loan</small>
          </td>
        </tr>
        <tr>
          <th class="stub">Reject</th>
          <td class="wrong">
            <span class="tag">\(v_3\)</span>
            <small>Rejection of a good loan</small>
          </td>
          <td class="right">
            <span class="tag">\(v_4\)</span>
            <small>Rejection of a bad loan</small>
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</section>

Each region is valued through the same behavioral value function $v(x)$.

--
<!-- .slide: class="slide-heading" -->
## Probability Weighting and Timing

$$
w_{\gamma}(p)=
\frac{p^{\gamma}}
{\left[p^{\gamma}+(1-p)^{\gamma}\right]^{1/\gamma}},
\qquad
\gamma>0
$$

$$
D(t)=
\begin{cases}
1, & t=0,\\[4pt]
\beta\delta^t, & t>0
\end{cases}
$$

$$
\beta\in(0,1],
\qquad
\delta\in(0,1]
$$

Present bias changes the valuation of delayed compensation without changing the true risk of the loan.

--
<!-- .slide: class="slide-heading" -->
## Approval and Rejection Values

$$
U_{i,\mathrm{Approve},t}
=
w_{\gamma}(\hat p_i)
D(t_{\mathrm{Approve},R})
v(x_{i,\mathrm{Approve},R,t})
+
\left[1-w_{\gamma}(\hat p_i)\right]
D(t_{\mathrm{Approve},D})
v(x_{i,\mathrm{Approve},D,t})
$$

$$
U_{i,\mathrm{Reject},t}
=
w_{\gamma}(\hat p_i)
D(t_{\mathrm{Reject},R})
v(x_{i,\mathrm{Reject},R,t})
+
\left[1-w_{\gamma}(\hat p_i)\right]
D(t_{\mathrm{Reject},D})
v(x_{i,\mathrm{Reject},D,t})
$$

--
<!-- .slide: class="slide-heading" -->
## Decision Rule and Ranking

$$
\Delta U_{i,t}
=
U_{i,\mathrm{Approve},t}
-
U_{i,\mathrm{Reject},t}
$$

Approve when $\Delta U_{i,t}>0$; reject when $\Delta U_{i,t}<0$.

$$
\Pr(\mathrm{Approve}_i)
=
\frac{\exp\left(\mu \Delta U_{i,t}\right)}
{1+\exp\left(\mu \Delta U_{i,t}\right)}
$$

For ranking tasks, loans are ordered from highest to lowest $\Delta U_{i,t}$.

--
<!-- .slide: class="slide-heading" -->
## Rank-Order Logit Representation

If the observed ranking is $i_1 \succ i_2 \succ \cdots \succ i_J$:

$$
\Pr(i_1 \succ i_2 \succ \cdots \succ i_J)
=
\prod_{j=1}^{J}
\frac{
\exp\left(\mu \Delta U_{i_j,t}\right)
}{
\sum_{\ell=j}^{J}
\exp\left(\mu \Delta U_{i_\ell,t}\right)
}
$$

The approval and ranking tasks are generated by the same latent behavioral valuation process.

--
<!-- .slide: class="slide-heading" -->
## Incentive Structure

Let $B_i$ be the bonus and $\kappa_t$ the degree to which inaccurate approval is penalized.

$$
c_{i,\mathrm{Approve},R,t}=B_i
$$

$$
c_{i,\mathrm{Approve},D,t}=B_i-\kappa_t L_i
$$

$$
c_{i,\mathrm{Reject},R,t}=0,
\qquad
c_{i,\mathrm{Reject},D,t}=0
$$

In the unadjusted condition, $\kappa_t=0$. In the incentive-adjusted condition, $\kappa_t>0$.

--
<!-- .slide: class="slide-heading" -->
## Bounded Attention and Satisficing

- $A_t$: available menu of loan-action prospects
- $F(A_t)$: feasible family of attention sets
- $S_t\subseteq A_t$: consideration set
- $z\in S_t$: loan-action prospect

$$
U_t(z)\geq \theta_t
\Rightarrow
\textnormal{stop}
$$

$$
W_t=
\max_{S_t\in F(A_t)}
\left\{
\max_{z\in S_t}
\left[U_t(z)-\mathcal{C}(S_t)\right],
\;
D(1)\mathbb{E}\left[W_{t+1}\mid S_t\right]
\right\}
$$

--
<!-- .slide: class="slide-heading" -->
## Objective and Perceived Frontiers

$$
\mathcal{F}_t
=
\left\{
(q_1,q_2):
q_2=
\left[
1-
\left(
\frac{q_1}{\psi_t}
\right)^{1-\lambda_f}
\right]^{1-\lambda_f},
\;
q_1\in[0,\psi_t]
\right\}
$$

$$
\lambda_f\in(0,1),
\qquad
\psi_t=\psi(\psi_{t-1},I_t)
$$

The perceived frontier is:

$$
\widetilde{\mathcal{F}}_t
=
\widetilde{\mathcal{F}}_t(\Psi,I_t,\Omega_i),
\qquad
\Psi=(\alpha,\lambda,\gamma,\beta,\delta,\mu)
$$

--
<!-- .slide: class="slide-heading" -->
## Treatment Mapping

<table style="border-collapse:collapse; margin:auto;">
  <thead>
    <tr>
      <th style="border:1px solid #ccc; padding:6px;">Condition</th>
      <th style="border:1px solid #ccc; padding:6px;">Model implication</th>
    </tr>
  </thead>
  <tbody>
    <tr><td style="border:1px solid #ccc; padding:6px;">Baseline</td>
        <td style="border:1px solid #ccc; padding:6px;">$t=0,\;D(t)=1,\;\kappa_t=0$</td></tr>
    <tr><td style="border:1px solid #ccc; padding:6px;">Delayed payment</td>
        <td style="border:1px solid #ccc; padding:6px;">$t>0,\;D(t)=\beta\delta^t$</td></tr>
    <tr><td style="border:1px solid #ccc; padding:6px;">Incentive adjustment</td>
        <td style="border:1px solid #ccc; padding:6px;">$\kappa_t>0$</td></tr>
    <tr><td style="border:1px solid #ccc; padding:6px;">Combined condition</td>
        <td style="border:1px solid #ccc; padding:6px;">$t>0,\;D(t)=\beta\delta^t,\;\kappa_t>0$</td></tr>
  </tbody>
</table>

--
<!-- .slide: class="slide-heading" -->
## Hypotheses

**H1:** Risk preferences and behavioral distortions moderate the effect of present-biased incentives on loan decisions.

**H2:** Incentive readjustments reshape effective indifference curves in the short term by changing reference-adjusted payoff, loss exposure, and compensation timing.

---
<!-- .slide: class="slide-heading closer" -->
## Optimal Choice Frontier With Distortions

<div class="media-xy">
  <img data-src="./images/Figure6.png" class="img-sm" alt="Optimal choice frontier in set S universe with distortions">
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
	      <td style="border:1px solid #ccc; padding:6px; text-align:center;">Time Delay | No Incentive Adjustment</td>
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
	      <tr><td style="border:1px solid #ccc; padding:6px;">DOSPERT risk profile</td>
	          <td style="border:1px solid #ccc; padding:6px;">Weber et al., 2002</td></tr>
	      <tr><td style="border:1px solid #ccc; padding:6px;">Holt-Laury risk task</td>
	          <td style="border:1px solid #ccc; padding:6px;">Holt and Laury, 2002</td></tr>
	      <tr><td style="border:1px solid #ccc; padding:6px;">Demographic controls</td>
	          <td style="border:1px solid #ccc; padding:6px;">Age, gender, education, income, role tenure, banking tenure</td></tr>
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

- Holt-Laury and DOSPERT are completed before the loan task.
- Participants complete a short loan-officer training.
- Incentive condition is disclosed before the decision set.
- Participants rank five loan profiles from strongest to weakest granting case.

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

- Preliminary field experiment with a local bank during scheduled officer training.
- $N=42$ loan officers.
- Pre-treatment and post-treatment loan decisions used matched-risk profiles.
- No consequential payoffs; the treatment was presented as a bonus-structure readjustment.

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
	    <li><span class="num">1</span>Scheduled loan-officer workshop.</li>
	    <li><span class="num">2</span>Envelope 1: five loan decisions.</li>
	    <li><span class="num">3</span>DOSPERT and socio-demographic survey.</li>
	    <li><span class="num">4</span>HR announces bonus-structure stimulus.</li>
	    <li><span class="num">5</span>Envelope 2: matched-risk loan decisions.</li>
	    <li><span class="num">6</span>Holt-Laury, disclosure, acknowledgement.</li>
	    <li><span class="num">7</span>Follow-up Holt-Laury at training end.</li>
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
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Education</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">Approximately 81% with at least a university degree</td>
        </tr>
        <tr>
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Experience (role)</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">2 months – 10 years</td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Context</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">During a scheduled training</td>
        </tr>
        <tr>
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Instruments</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">DOSPERT test; Holt–Laury risk test</td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Decision sets</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">Pre &amp; post stimulus profiles with matched risk characteristics</td>
        </tr>
        <tr>
          <th style="text-align:left; padding:10px 14px; color:#5b6573;">Stimulus</th>
          <td style="padding:10px 14px;">HR announced a bonus calculation readjustment</td>
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
            <strong>46% → 53%</strong> after the incentive-readjustment stimulus
          </td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Inference</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">
            Descriptive movement is mechanism-consistent, but not conclusive causal evidence
          </td>
        </tr>
        <tr>
          <th style="text-align:left; padding:10px 14px; color:#5b6573; border-bottom:1px solid #e6eaef;">Risk posture</th>
          <td style="padding:10px 14px; border-bottom:1px solid #e6eaef;">
            Holt scores move immediately after the stimulus, then return toward baseline
          </td>
        </tr>
        <tr style="background:#ffffff;">
          <th style="text-align:left; padding:10px 14px; color:#5b6573;">Statistical power</th>
          <td style="padding:10px 14px;">
            Preliminary study underpowered; approximately <strong>290</strong> participants required
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</div>


--
<!-- .slide: class="slide-heading diagram closer" -->
# Descriptive Accuracy Movement

<div class="media-xy">
  <img data-src="./images/Accuracy_2.png" class="img-sm" alt="Accuracy figure">
</div>

--
<!-- .slide: class="slide-heading diagram closer" -->
## Incentive Readjustment by Risk Quartile

<div class="media-xy">
  <img data-src="./images/Adjustment_E1.png" class="img-sm" alt="Predicted probability by incentive readjustment and risk quartile">
</div>

--
<!-- .slide: class="slide-heading diagram closer" -->
## Short-Term Movement in Revealed Risk Posture

<div class="media-xy">
  <img data-src="./images/Risk_Preference_Trajectories.png" class="img-sm" alt="trajectories">
</div>

---
<!-- .slide: class="slide-heading" -->
## Empirical Strategy and Diagnostics

**From the field experiment**
- Loan-decision accuracy before and after the stimulus
- DOSPERT profile
- Baseline Holt-Laury risk score
- Holt-score trajectory across three moments
- Gender, age, education, income, loan-officer tenure, banking tenure

--

## Accuracy Pre-Post Specification

$$
Accuracy_{it}
=
\theta_0
+
\theta_1 Post_t
+
\theta_2 Dospert_i
+
\theta_3 Holt_{i,0}
+
\theta_4(Post_t \times Dospert_i)
+
\theta_5(Post_t \times Holt_{i,0})
+
\varepsilon_{it}
$$

Because the model includes interactions, $\theta_1$ is conditional on $Dospert_i=0$ and $Holt_{i,0}=0$.

<table style="border-collapse:collapse; margin:auto;">
  <tbody>
    <tr><td style="border:1px solid #ccc; padding:6px;">$Post_t$</td><td style="border:1px solid #ccc; padding:6px;">$\hat\theta_1=-0.172,\;p=0.241$</td></tr>
    <tr><td style="border:1px solid #ccc; padding:6px;">$Post_t\times Dospert_i$</td><td style="border:1px solid #ccc; padding:6px;">$\hat\theta_4=-0.223,\;p=0.168$</td></tr>
    <tr><td style="border:1px solid #ccc; padding:6px;">$Post_t\times Holt_{i,0}$</td><td style="border:1px solid #ccc; padding:6px;">$\hat\theta_5=0.214,\;p=0.276$</td></tr>
    <tr><td style="border:1px solid #ccc; padding:6px;">Model fit</td><td style="border:1px solid #ccc; padding:6px;">$F=1.216,\;p=0.309,\;\text{adjusted }R^2=0.013$</td></tr>
  </tbody>
</table>

--

## Holt-Score Trajectory Models

$$
HoltScore_{it}
=
\alpha_0
+
\alpha_1 Timepoint_t
+
\alpha_2 Dospert_i
+
X_i'\Gamma
+
u_{it}
$$

- $Timepoint_t$: $\hat\alpha_1=0.001,\;p=0.963$
- $Timepoint_t\times Dospert_i$: $\hat\alpha=-0.065,\;p=0.462$
- Gender, time as a loan officer, time in banking, and the age-45 category are statistically associated with Holt scores.
- Mixed-effects model: officer random-intercept variance $0.051$; residual variance $0.023$.

--

## Interpretation of Field Evidence

- Average accuracy moved from $46\%$ to $53\%$ after the stimulus.
- The movement is directionally consistent with $H_1$.
- Holt-score trajectories are directionally consistent with $H_2$.
- Inferential models do not reach conventional statistical significance.
- The study is preliminary, mechanism-consistent field evidence rather than definitive causal identification.

--

## Simulation Diagnostics

The appendix evaluates whether the behavioral model can generate non-degenerate choices and where lending mistakes concentrate.

$$
\Psi=(\alpha,\lambda,\gamma,\beta,\delta,\mu)
$$

- Parameter recovery is feasible in some regions and unstable in others.
- The hardest saved-run parameters to recover are $\gamma$ and $\beta$.
- The loan-problem simulation uses $10{,}000$ loan problems and $200$ simulated decision-makers.
- Mistakes concentrate near the repayment threshold $\rho=0.70$.

--

## Simulation Interpretation

- High-error regions differ by incentive regime.
- The most problematic simulated loans often combine high collateral values with repayment probabilities near the acceptance cutoff.
- The simulations support the computational plausibility of the mechanism.
- They also explain why the preliminary field sample of $42$ officers is underpowered for precise structural identification.

---
<!-- .slide: class="slide-heading" -->
## Q&A
