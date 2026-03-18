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
<!-- .slide: class="slide-heading" -->
## Q&A