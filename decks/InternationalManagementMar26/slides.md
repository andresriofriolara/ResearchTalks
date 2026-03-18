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
      font-size: clamp(10px, 1.05vw, 15px);
      line-height: 1.16;
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
    @media (max-width: 900px) {
      .rq-wrap { padding: 0 10px; }
      .rq-card { padding: 18px 18px 16px 24px; }
      .rq-title { font-size: clamp(10px, 1.05vw, 15px); }
    }
  </style>

  <div class="rq-wrap">
    <div class="rq-grid">
      <div class="rq-card fragment" data-fragment-index="2">
        <div class="rq-badge">3</div>
        <div class="rq-title">Does moving toward a relatively lower-hassle environment improve subsidiary outcomes?</div>
      </div>
      <div class="rq-card fragment" data-fragment-index="1">
        <div class="rq-badge">2</div>
        <div class="rq-title">Does moving into a relatively higher-hassle environment worsen subsidiary outcomes?</div>
      </div>
      <div class="rq-card fragment" data-fragment-index="0">
        <div class="rq-badge">1</div>
        <div class="rq-title">Does directional movement in hassle space help explain multinational subsidiary survival and profitability?</div>
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
        captured by <span class="hyp-em">Δ<sup>+</sup><sub>i,t</sub></span> and/or
        <span class="hyp-em">Δ<sup>−</sup><sub>i,t</sub></span>,
        is associated with a lower probability of subsidiary survival, allowing for asymmetric effects between upward and downward moves in hassle space.
      </p>
    </div>
    <div class="hyp-card">
      <div class="hyp-tag">Hypothesis 2</div>
      <h3 class="hyp-title">Subsidiary Profitability</h3>
      <p class="hyp-text">
        Greater hassle-space displacement between the origin country and the host country,
        captured by <span class="hyp-em">Δ<sup>+</sup><sub>i,t</sub></span> and/or
        <span class="hyp-em">Δ<sup>−</sup><sub>i,t</sub></span>,
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

<style>
  .reveal section.slide-heading .just-wrap{
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 18px;
  }
  .reveal section.slide-heading .just-grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
    align-items: start;
    justify-items: center;
  }
  .reveal section.slide-heading .just-card{
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: flex-start;
    overflow: visible;
  }
  .reveal section.slide-heading .just-card img{
    width: 66% !important;
    max-width: 66% !important;
    height: auto !important;
    max-height: none !important;
    object-fit: contain;
    display: block;
    margin: 0 auto;
  }
  @media (max-width: 900px){
    .reveal section.slide-heading .just-grid{
      grid-template-columns: 1fr;
    }
    .reveal section.slide-heading .just-card img{
      width: 42% !important;
      max-width: 42% !important;
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
      <div class="smart-card">
        <p>The literature usually models cross-country frictions as static host-country characteristics.</p>
      </div>
      <div class="smart-arrow">➜</div>
      <div class="smart-card">
        <p>The Hassle Factor has largely been used as a scalar country attribute.</p>
      </div>
      <div class="smart-arrow">➜</div>
      <div class="smart-card">
        <p>Firms evaluate host environments relative to their origin baseline.</p>
      </div>
    </div>
  </div>
</section>

---
<!-- .slide: class="slide-heading closer" -->
## The Hassle Factor

<style>
  .hf-wrap{
    max-width: 1100px;
    margin: 0 auto;
    padding: 6px 18px 0 18px;
  }
  .hf-grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
    align-items: stretch;
  }
  .hf-card{
    position: relative;
    background: linear-gradient(180deg, #ffffff, #fbfdff);
    border: 1px solid #e6eaef;
    border-radius: 18px;
    padding: 22px 22px 18px 22px;
    box-shadow: 0 6px 20px rgba(0,0,0,.06);
    text-align: left;
    min-height: 170px;
  }
  .hf-card.accent{
    background: linear-gradient(180deg, #f4fbf7, #eef8f2);
    border-color: #cfe3d8;
  }
  .hf-label{
    display: inline-block;
    margin-bottom: 10px;
    padding: 5px 11px;
    border-radius: 999px;
    background: #0d5e3a;
    color: #fff;
    font-size: 13px;
    font-weight: 800;
    letter-spacing: .3px;
  }
  .hf-title{
    margin: 0 0 8px 0;
    font-size: 20px;
    line-height: 1.15;
    font-weight: 800;
    color: #0b4f35;
  }
  .hf-text{
    margin: 0;
    font-size: 15px;
    line-height: 1.35;
    color: #2f3844;
  }
  .hf-card::after{
    content: "";
    position: absolute;
    inset: auto 0 0 0;
    height: 5px;
    background: linear-gradient(90deg, #0d5e3a 0%, #7fb18f 60%, #b9d7c8 100%);
    border-radius: 0 0 18px 18px;
    opacity: .9;
  }
  @media (max-width: 900px){
    .hf-grid{
      grid-template-columns: 1fr;
    }
    .hf-card{
      min-height: auto;
    }
  }
</style>

<div class="hf-wrap">
  <div class="hf-grid">
    <div class="hf-card">
      <div class="hf-label">Definition</div>
      <div class="hf-title">What it is</div>
      <p class="hf-text">
        A country-attractiveness and business-friction measure developed to capture how burdensome it is to conduct business across countries.
      </p>
    </div>
    <div class="hf-card">
      <div class="hf-label">Dimensions</div>
      <div class="hf-title">What it captures</div>
      <p class="hf-text">
        Eleven practical sources of business inconvenience, including safety, visas, transportation, hotels, hygiene, telecom, health risks, language, business facilitation, and climate.
      </p>
    </div>
    <div class="hf-card">
      <div class="hf-label">Construction</div>
      <div class="hf-title">How it is built</div>
      <p class="hf-text">
        A comparable country-year scalar score constructed from weighted indicators within a confirmatory-factor framework.
      </p>
    </div>
    <div class="hf-card accent">
      <div class="hf-label">Role in this paper</div>
      <div class="hf-title">Why it matters here</div>
      <p class="hf-text">
        The Hassle Factor provides the empirical raw material: each country-year score becomes the coordinate from which hassle space is later defined.
      </p>
    </div>
  </div>
</div>

--
<!-- .slide: class="slide-heading closer" -->
## The Hassle Vector

<style>
  .hv-wrap{
    max-width: 1100px;
    margin: 0 auto;
    padding: 6px 18px 0 18px;
  }
  .hv-grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
    align-items: stretch;
  }
  .hv-card{
    position: relative;
    background: linear-gradient(180deg, #ffffff, #fbfdff);
    border: 1px solid #e6eaef;
    border-radius: 18px;
    padding: 22px 22px 18px 22px;
    box-shadow: 0 6px 20px rgba(0,0,0,.06);
    text-align: left;
    min-height: 180px;
  }
  .hv-card.accent{
    background: linear-gradient(180deg, #f4fbf7, #eef8f2);
    border-color: #cfe3d8;
  }
  .hv-label{
    display: inline-block;
    margin-bottom: 10px;
    padding: 5px 11px;
    border-radius: 999px;
    background: #0d5e3a;
    color: #fff;
    font-size: 13px;
    font-weight: 800;
    letter-spacing: .3px;
  }
  .hv-title{
    margin: 0 0 8px 0;
    font-size: 20px;
    line-height: 1.15;
    font-weight: 800;
    color: #0b4f35;
  }
  .hv-text{
    margin: 0;
    font-size: 15px;
    line-height: 1.35;
    color: #2f3844;
  }
  .hv-eqn{
    margin-top: 10px;
    font-size: 17px;
    line-height: 1.25;
    color: #123524;
    font-weight: 700;
  }
  .hv-card::after{
    content: "";
    position: absolute;
    inset: auto 0 0 0;
    height: 5px;
    background: linear-gradient(90deg, #0d5e3a 0%, #7fb18f 60%, #b9d7c8 100%);
    border-radius: 0 0 18px 18px;
    opacity: .9;
  }
  @media (max-width: 900px){
    .hv-grid{
      grid-template-columns: 1fr;
    }
    .hv-card{
      min-height: auto;
    }
  }
</style>

<div class="hv-wrap">
  <div class="hv-grid">
    <div class="hv-card">
      <div class="hv-label">Coordinate</div>
      <div class="hv-title">Each country-year is a point in hassle space</div>
      <p class="hv-text">
        The Hassle Factor is no longer treated only as a scalar attribute, but as a coordinate in an abstract metric space.
      </p>
    </div>
    <div class="hv-card">
      <div class="hv-label">Comparison</div>
      <div class="hv-title">The relevant contrast is origin versus host</div>
      <p class="hv-text">
        For subsidiary <em>i</em>, the relevant empirical comparison is not the host country in isolation, but the difference between host and origin environments.
      </p>
    </div>
    <div class="hv-card">
      <div class="hv-label">Displacement</div>
      <div class="hv-title">The Hassle Vector is the signed difference</div>
      <p class="hv-text">
        It measures movement from the origin country to the host country in hassle space.
      </p>
      <div class="hv-eqn">
        Δ<sub>i,t</sub> = H<sub>h<sub>i</sub>,t</sub> − H<sub>o<sub>i</sub>,t</sub>
      </div>
    </div>
    <div class="hv-card accent">
      <div class="hv-label">Asymmetry</div>
      <div class="hv-title">The sign of movement matters</div>
      <p class="hv-text">
        The displacement is decomposed into two legs so the model distinguishes upward from downward movement in hassle space.
      </p>
      <div class="hv-eqn">
        Δ<sup>+</sup><sub>i,t</sub> = max(Δ<sub>i,t</sub>, 0)
        <br>
        Δ<sup>−</sup><sub>i,t</sub> = max(−Δ<sub>i,t</sub>, 0)
      </div>
    </div>
  </div>
</div>

---
<!-- .slide: class="slide-heading closer" -->
## Methods

<style>
  .m-wrap{
    max-width: 1100px;
    margin: 0 auto;
    padding: 6px 18px 0 18px;
  }
  .m-grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
    align-items: stretch;
  }
  .m-card{
    position: relative;
    background: linear-gradient(180deg, #ffffff, #fbfdff);
    border: 1px solid #e6eaef;
    border-radius: 18px;
    padding: 22px 22px 18px 22px;
    box-shadow: 0 6px 20px rgba(0,0,0,.06);
    text-align: left;
    min-height: 180px;
  }
  .m-card.accent{
    background: linear-gradient(180deg, #f4fbf7, #eef8f2);
    border-color: #cfe3d8;
  }
  .m-label{
    display: inline-block;
    margin-bottom: 10px;
    padding: 5px 11px;
    border-radius: 999px;
    background: #0d5e3a;
    color: #fff;
    font-size: 13px;
    font-weight: 800;
    letter-spacing: .3px;
  }
  .m-title{
    margin: 0 0 8px 0;
    font-size: 20px;
    line-height: 1.15;
    font-weight: 800;
    color: #0b4f35;
  }
  .m-text{
    margin: 0;
    font-size: 15px;
    line-height: 1.35;
    color: #2f3844;
  }
  .m-list{
    margin: 8px 0 0 18px;
    padding: 0;
    font-size: 15px;
    line-height: 1.35;
    color: #2f3844;
  }
  .m-list li{
    margin: 4px 0;
    text-align: left;
  }
  .m-card::after{
    content: "";
    position: absolute;
    inset: auto 0 0 0;
    height: 5px;
    background: linear-gradient(90deg, #0d5e3a 0%, #7fb18f 60%, #b9d7c8 100%);
    border-radius: 0 0 18px 18px;
    opacity: .9;
  }
  @media (max-width: 900px){
    .m-grid{
      grid-template-columns: 1fr;
    }
    .m-card{
      min-height: auto;
    }
  }
</style>

<div class="m-wrap">
  <div class="m-grid">
    <div class="m-card">
      <div class="m-label">Data</div>
      <div class="m-title">Sample and time coverage</div>
      <p class="m-text">
        The empirical analysis combines the TK panel of Japanese foreign subsidiaries with Hassle Factor country-year data for 2008–2018.
      </p>
    </div>
    <div class="m-card">
      <div class="m-label">Outcomes</div>
      <div class="m-title">Subsidiary exit and profitability</div>
      <ul class="m-list">
        <li>Discrete subsidiary survival / exit outcome</li>
        <li>Profitability proxied by log(1 + Revenue<sup>USD</sup><sub>i,t</sub>)</li>
      </ul>
    </div>
    <div class="m-card">
      <div class="m-label">Models</div>
      <div class="m-title">Hazard and profitability specifications</div>
      <ul class="m-list">
        <li>Discrete-time hazard model for exit</li>
        <li>Profitability regression for operating performance</li>
        <li>Key regressors: H<sub>host</sub>, Δ<sup>+</sup>, Δ<sup>−</sup>, controls, fixed effects, and duration terms</li>
      </ul>
    </div>
    <div class="m-card accent">
      <div class="m-label">Inference</div>
      <div class="m-title">Dependence is modeled in hassle-space-time</div>
      <p class="m-text">
        Inference relies on Conley-style robust standard errors, where dependence is defined over the metric space
        (Δ, t) rather than only over physical geography.
      </p>
    </div>
  </div>
</div>

---


<!-- .slide: class="slide-heading" -->
## Q&A