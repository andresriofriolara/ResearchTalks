<!-- .slide: class="title-slide" -->
# Hassle Vector: Predicting Internationalization Survival and Success.
</section>

---
<!-- .slide: class="slide-heading closer" -->
## What does this research do?

<div style="display:flex; justify-content:center; align-items:center; width:100%;">
  <img src="images/surface.png" alt="Hassle Space Surface" style="max-width:78%; height:auto; display:block;">
</div>

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
    .rq-card::after {
      content: ""; position: absolute; inset: auto 0 0 0; height: 6px;
      background: linear-gradient(90deg, #0d5e3a 0%, #7fb18f 60%, #b9d7c8 100%);
      border-radius: 0 0 16px 16px; opacity: .85;
    }
    .rq-card[data-fragment-index="0"] { z-index: 3; }
    .rq-card[data-fragment-index="1"] { z-index: 2; }
    .rq-card[data-fragment-index="2"] { z-index: 1; }
    :root.dark .rq-card { background:#0f141a; border-color:#2a3441; }
    :root.dark .rq-sub { color:#c7d1dd; }
    :root.dark .rq-card::after { opacity:.6; }
  </style>

  <div class="rq-wrap">
    <div class="rq-grid">
      <!-- Q3 -->
      <div class="rq-card fragment" data-fragment-index="2">
        <div class="rq-badge">3</div>
        <h3 class="rq-title">Does moving toward a relatively lower-hassle environment improve subsidiary outcomes?</h3>
        <p class="rq-sub">Test whether downward movement in hassle space is associated with lower exit hazard and higher profitability.</p>
      </div>
      <!-- Q2 -->
      <div class="rq-card fragment" data-fragment-index="1">
        <div class="rq-badge">2</div>
        <h3 class="rq-title">Does moving into a relatively higher-hassle environment worsen subsidiary outcomes?</h3>
        <p class="rq-sub">Test whether upward movement in hassle space is associated with higher exit hazard and lower profitability.</p>
      </div>
      <!-- Q1 -->
      <div class="rq-card fragment" data-fragment-index="0">
        <div class="rq-badge">1</div>
        <h3 class="rq-title">Does directional movement in hassle space help explain multinational subsidiary survival and profitability?</h3>
        <p class="rq-sub">The relevant empirical object is not host-country hassle in isolation, but the structured contrast between origin and host.</p>
      </div>
    </div>
  </div>
</section>

--
<!-- .slide: class="slide-heading" -->
## Hypotheses

<section>
  <style>
    .hyp-wrap{
      max-width: 1100px;
      margin: 0 auto;
      padding: clamp(8px, 2vw, 18px);
    }
    .hyp-grid{
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: clamp(16px, 2.4vw, 24px);
      align-items: stretch;
    }
    .hyp-card{
      position: relative;
      background: linear-gradient(180deg, #ffffff, #fbfdff);
      border: 1px solid #e6eaef;
      border-radius: 18px;
      padding: 24px 24px 22px 24px;
      box-shadow: 0 8px 24px rgba(0,0,0,.07);
      text-align: left;
    }
    .hyp-tag{
      display: inline-block;
      margin-bottom: 12px;
      padding: 6px 12px;
      border-radius: 999px;
      background: #0d5e3a;
      color: #fff;
      font-size: 15px;
      font-weight: 800;
      letter-spacing: .3px;
    }
    .hyp-title{
      margin: 0 0 10px 0;
      font-size: clamp(22px, 2.3vw, 30px);
      line-height: 1.2;
      font-weight: 800;
    }
    .hyp-text{
      margin: 0;
      font-size: clamp(17px, 1.55vw, 21px);
      line-height: 1.45;
      color: #2f3844;
    }
    .hyp-em{
      color: #0d5e3a;
      font-weight: 800;
    }
    .hyp-card::after{
      content: "";
      position: absolute;
      inset: auto 0 0 0;
      height: 6px;
      background: linear-gradient(90deg, #0d5e3a 0%, #7fb18f 60%, #b9d7c8 100%);
      border-radius: 0 0 18px 18px;
      opacity: .9;
    }
    @media (max-width: 900px){
      .hyp-grid{ grid-template-columns: 1fr; }
    }
    :root.dark .hyp-card{
      background: #0f141a;
      border-color: #2a3441;
    }
    :root.dark .hyp-text{
      color: #d3dbe5;
    }
  </style>

  <div class="hyp-wrap">
    <div class="hyp-grid">
      <div class="hyp-card fragment" data-fragment-index="0">
        <div class="hyp-tag">Hypothesis 1</div>
        <h3 class="hyp-title">Subsidiary Survival</h3>
        <p class="hyp-text">
          Greater hassle-space displacement between the origin country and the host country,
          captured by <span class="hyp-em">\( \Delta^+_{i,t} \)</span> and/or
          <span class="hyp-em">\( \Delta^-_{i,t} \)</span>,
          is associated with a lower probability of subsidiary survival,
          allowing for asymmetric effects between upward and downward moves in hassle space.
        </p>
      </div>
      <div class="hyp-card fragment" data-fragment-index="1">
        <div class="hyp-tag">Hypothesis 2</div>
        <h3 class="hyp-title">Subsidiary Profitability</h3>
        <p class="hyp-text">
          Greater hassle-space displacement between the origin country and the host country,
          captured by <span class="hyp-em">\( \Delta^+_{i,t} \)</span> and/or
          <span class="hyp-em">\( \Delta^-_{i,t} \)</span>,
          is associated with lower subsidiary profitability,
          again allowing for asymmetric effects between upward and downward moves in hassle space.
        </p>
      </div>
    </div>
  </div>
</section>

---

<!-- .slide: class="slide-heading" -->
## Q&A