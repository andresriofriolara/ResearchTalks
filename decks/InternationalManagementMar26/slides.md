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
<!-- .slide: class="slide-heading closer" -->
## Research Questions

<section>
  <style>
    .rq-wrap {
      max-width: 1120px;
      margin: 0 auto;
      padding: 0 18px;
    }
    .rq-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 18px;
    }
    .rq-card {
      position: relative;
      background: linear-gradient(180deg, #ffffff, #fbfdff);
      border: 1px solid #e6eaef;
      border-radius: 16px;
      padding: 22px 26px 20px 34px;
      box-shadow: 0 6px 20px rgba(0,0,0,.06);
    }
    .rq-badge {
      position: absolute;
      top: -10px;
      left: -10px;
      width: 38px;
      height: 38px;
      border-radius: 999px;
      display: grid;
      place-items: center;
      background: #0d5e3a;
      color: #fff;
      font-weight: 800;
      box-shadow: 0 8px 18px rgba(13,94,58,.25);
      font-size: 18px;
    }
    .rq-title {
      margin: 0;
      font-size: clamp(13px, 1.35vw, 20px);
      line-height: 1.18;
      font-weight: 800;
      letter-spacing: 0;
      color: #0b4f35;
      word-break: normal;
      overflow-wrap: break-word;
      hyphens: auto;
    }
    .rq-card::after {
      content: "";
      position: absolute;
      inset: auto 0 0 0;
      height: 5px;
      background: linear-gradient(90deg, #0d5e3a 0%, #7fb18f 60%, #b9d7c8 100%);
      border-radius: 0 0 16px 16px;
      opacity: .85;
    }
    .rq-card[data-fragment-index="0"] { z-index: 3; }
    .rq-card[data-fragment-index="1"] { z-index: 2; }
    .rq-card[data-fragment-index="2"] { z-index: 1; }
    :root.dark .rq-card {
      background: #0f141a;
      border-color: #2a3441;
    }
    :root.dark .rq-title {
      color: #e5edf5;
    }
    @media (max-width: 900px) {
      .rq-wrap { padding: 0 10px; }
      .rq-card { padding: 18px 18px 16px 24px; }
      .rq-title { font-size: clamp(13px, 1.8vw, 18px); }
    }
  </style>

  <div class="rq-wrap">
    <div class="rq-grid">
      <div class="rq-card fragment" data-fragment-index="2">
        <div class="rq-badge">3</div>
        <h3 class="rq-title">Does moving toward a relatively lower-hassle environment improve subsidiary outcomes?</h3>
      </div>
      <div class="rq-card fragment" data-fragment-index="1">
        <div class="rq-badge">2</div>
        <h3 class="rq-title">Does moving into a relatively higher-hassle environment worsen subsidiary outcomes?</h3>
      </div>
      <div class="rq-card fragment" data-fragment-index="0">
        <div class="rq-badge">1</div>
        <h3 class="rq-title">Does directional movement in hassle space help explain multinational subsidiary survival and profitability?</h3>
      </div>
    </div>
  </div>
</section>

--
<!-- .slide: class="slide-heading closer" -->
## Hypotheses

<div class="hyp-wrap">
  <div class="hyp-grid">
    <div class="hyp-card">
      <div class="hyp-tag">Hypothesis 1</div>
      <h3 class="hyp-title">Subsidiary Survival</h3>
      <p class="hyp-text">
        Greater hassle-space displacement between the origin country and the host country,
        captured by <span class="hyp-em">\( \Delta^+_{i,t} \)</span> and/or
        <span class="hyp-em">\( \Delta^-_{i,t} \)</span>,
        is associated with a lower probability of subsidiary survival, allowing for asymmetric effects between upward and downward moves in hassle space.
      </p>
    </div>
    <div class="hyp-card">
      <div class="hyp-tag">Hypothesis 2</div>
      <h3 class="hyp-title">Subsidiary Profitability</h3>
      <p class="hyp-text">
        Greater hassle-space displacement between the origin country and the host country,
        captured by <span class="hyp-em">\( \Delta^+_{i,t} \)</span> and/or
        <span class="hyp-em">\( \Delta^-_{i,t} \)</span>,
        is associated with lower subsidiary profitability, again allowing for asymmetric effects between upward and downward moves in hassle space.
      </p>
    </div>
  </div>
</div>

<style>
  .hyp-wrap{
    max-width: 1100px;
    margin: 0 auto;
    padding: 8px 18px;
  }
  .hyp-grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 22px;
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
    font-size: clamp(20px, 2vw, 28px);
    line-height: 1.2;
    font-weight: 800;
    color: #0b4f35;
  }
  .hyp-text{
    margin: 0;
    font-size: clamp(15px, 1.25vw, 19px);
    line-height: 1.42;
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
  :root.dark .hyp-title{
    color: #e5edf5;
  }
  :root.dark .hyp-text{
    color: #d3dbe5;
  }
</style>

---
<!-- .slide: class="slide-heading closer" -->
## Justification

<section>
  <style>
    .just-wrap{
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 18px;
    }
    .just-grid{
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 18px;
      align-items: start;
      justify-items: center;
    }
    .just-card{
      width: 100%;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      overflow: visible;
    }
    .just-card img{
      width: auto;
      height: auto;
      max-width: 100%;
      max-height: 34vh;
      object-fit: contain;
      display: block;
      margin: 0 auto;
    }
    @media (max-width: 900px){
      .just-grid{
        grid-template-columns: 1fr;
      }
      .just-card img{
        max-height: 28vh;
      }
    }
  </style>

  <div class="just-wrap">
    <div class="just-grid">
      <div class="just-card">
        <img src="images/similar.png" alt="Related literature or conceptual similarity figure">
      </div>
      <div class="just-card">
        <img src="images/cited.png" alt="Citation or literature motivation figure">
      </div>
    </div>
  </div>
</section>

--
<!-- .slide: class="slide-heading closer" -->
## Why a Hassle Vector?

<section>
  <style>
    .smart-wrap{
      max-width: 1180px;
      margin: 0 auto;
      padding: clamp(10px, 2vw, 18px);
    }
    .smart-flow{
      display: grid;
      grid-template-columns: 1fr auto 1fr auto 1fr;
      gap: 14px;
      align-items: center;
    }
    .smart-card{
      min-height: 210px;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 22px 20px;
      border-radius: 22px;
      background: linear-gradient(180deg, #ffffff, #f7fbf9);
      border: 1px solid #dfe7e2;
      box-shadow: 0 8px 24px rgba(0,0,0,.06);
    }
    .smart-card p{
      margin: 0;
      font-size: clamp(21px, 2.0vw, 28px);
      line-height: 1.28;
      font-weight: 800;
      color: #123524;
    }
    .smart-arrow{
      font-size: clamp(34px, 3vw, 48px);
      font-weight: 900;
      color: #0d5e3a;
      line-height: 1;
      opacity: .9;
    }
    @media (max-width: 980px){
      .smart-flow{
        grid-template-columns: 1fr;
      }
      .smart-arrow{
        transform: rotate(90deg);
        justify-self: center;
      }
      .smart-card{
        min-height: 140px;
      }
    }
    :root.dark .smart-card{
      background: #0f141a;
      border-color: #2a3441;
    }
    :root.dark .smart-card p{
      color: #e5edf5;
    }
  </style>

  <div class="smart-wrap">
    <div class="smart-flow">
      <div class="smart-card fragment" data-fragment-index="0">
        <p>The literature usually models cross-country frictions as static host-country characteristics.</p>
      </div>
      <div class="smart-arrow fragment" data-fragment-index="1">➜</div>
      <div class="smart-card fragment" data-fragment-index="1">
        <p>The Hassle Factor has largely been used as a scalar country attribute.</p>
      </div>
      <div class="smart-arrow fragment" data-fragment-index="2">➜</div>
      <div class="smart-card fragment" data-fragment-index="2">
        <p>Firms evaluate host environments relative to their origin baseline.</p>
      </div>
    </div>
  </div>
</section>

---

<!-- .slide: class="slide-heading" -->
## Q&A