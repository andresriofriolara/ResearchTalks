<!-- .slide: class="title-slide" -->
# Counteractive Lobbying: Conceptual Replication in the Canadian Financial Regulation.
</section>

---
<!-- .slide: class="slide-heading" -->
## Motivation

<div class="panels">

  <div class="panel">
    <div class="panel-hd">Counteractive lobbying</div>
    <div class="panel-bd">
      <ul>
        <li><strong>Counteractive lobbying as an object of study</strong></li>
        <ul>
          <li>When one coalition lobbies, this can change the incentives of the opposing coalition to lobby the same decision-makers.</li>
          <li>This affects which interests are represented around a given policy conflict.</li>
        </ul>
        <li><strong>From Austen–Smith &amp; Wright (AS&amp;W) to RPAA</strong></li>
        <ul>
          <li>AS&amp;W 94' study counteractive lobbying for a single confirmation conflict in the U.S. Senate.</li>
        </ul>
      </ul>
    </div>
  </div>

  <div class="panel">
    <div class="panel-hd">RPAA settings</div>
    <div class="panel-bd">
      <ul>
        <li><strong>RPAA and the Canadian lobbying registry</strong></li>
        <ul>
          <li>RPAA and its regulations define a single, well-specified policy domain in retail payments.</li>
          <li>The federal lobbying registry provides administrative records on registrations and communications, including clients, public office holders, dates, and issue descriptions.</li>
        </ul>
        <li><strong>Why should it work...</strong></li>
        <ul>
          <li>Use the RPAA case and the registry to implement AS&amp;W 94'-style lobbying measures.</li>
          <li>Examine how their framework can structure an analysis of lobbying around Canadian financial regulation.</li>
        </ul>
      </ul>
    </div>
  </div>

</div>

---
<!-- .slide: class="slide-heading" -->
## Research Question

### Can the counteractive lobbying framework of Austen–Smith &amp; Wright be replicated through the RPAA setting using the Canadian federal lobbying registry?

--

<div class="vsteps-wrap">
  <ul class="vsteps">
    <li>
      <div class="num">1</div>
      <strong>Targeting across institutions</strong><br>
      How can we measure which institutions (Parliament, Finance Canada, Bank of Canada, FCAC, other departments) are most involved in RPAA-related lobbying?
    </li>
    <li>
      <div class="num">2</div>
      <strong>Targeting across political units</strong><br>
      How can we describe the distribution of lobbying intensity across individual political units (MPs, Senators, ministers, senior officials and staff)?
    </li>
    <li>
      <div class="num">3</div>
      <strong>Two sides and their balance</strong><br>
      How can we operationalise “pro-policy” and “anti-policy” sides (industry vs public-interest) in the registry, and under what conditions is it possible to study their interaction at the unit level?
    </li>
    <li>
      <div class="num">4</div>
      <strong>Link to outcomes (for later stages)</strong><br>
      How could these lobbying measures later be connected to votes, amendments, speeches, or regulatory decisions, once those outcomes are coded?
    </li>
  </ul>
</div>

---
<!-- .slide: class="slide-heading" -->
## Theoretical Framework

<div class="seg-toggle">
  <div class="seg-pill">
    <div class="seg is-active">AS&amp;W (1994)</div>
    <div class="seg">Debate &amp; Rejoinder (1996)</div>
  </div>
</div>

<div class="cols">
  <div>
    <h3>Counteractive lobbying – Austen–Smith &amp; Wright (1994)</h3>
    <ul>
      <li>Two opposing coalitions, one legislator with a prior and costly auditing.</li>
      <li>Lobbying is strategic information under competition.</li>
      <li>Evidence: Bork nomination; senator-level counts of pro/anti lobbying are broadly consistent with these patterns.</li>
    </ul>
  </div>

  <div>
    <h3>Debate and rejoinder (Baumgartner &amp; Leech 1996; AS&amp;W 1996)</h3>
    <ul>
      <li><strong>Baumgartner &amp; Leech (1996):</strong>
        <ul>
          <li>Argue that the evidence is ambiguous and that other mechanisms (indirect lobbying, coalition maintenance, dynamics) could generate similar patterns.</li>
          <li>Question the measurement strategy and cross-sectional design.</li>
        </ul>
      </li>
      <li><strong>Austen–Smith &amp; Wright (1996):</strong>
        <ul>
          <li>Emphasise that the interaction between opponent lobbying and predisposition is the core test.</li>
          <li>Show that alternative assumptions about priors still produce similar counteractive patterns.</li>
          <li>Stress that analysis must be at the coalition–legislator level.</li>
        </ul>
      </li>
    </ul>
  </div>
</div>

---
**Who gets lobbied? Allies and institutional structure**  
- Kollman (1997): groups often lobby allies on key committees; institutional structure shapes targeting.  
- Awad (2020): groups lobby allies as intermediaries who set agendas and build coalitions.  
- Implication: lobbying of friendly legislators can reflect counteractive defence or ally-centred persuasion, depending on context and opponent activity.


**Modern empirical lobbying: access, influence, and channels**  
- Access and connections:  
  - Revolving-door and network studies show that lobbyists with government connections earn access rents; both connections and expertise are rewarded.  
  - Lobbying concentrates where access is most valuable.  
- Real effects of lobbying:  
  - Lobbying by interest groups can shift public funding priorities (e.g., disease-group lobbying and NIH allocations).  
  - Corporate philanthropy can act as tax-exempt lobbying, partly outside formal registries.  
- Political wins and markets:  
  - Political influence feeds into product-market competition; lobbying is one margin of broader strategic rivalry.



---
<!-- .slide: class="slide-heading" -->
## Empirical Strategy

<div class="smart-funnel">
  <div class="funnel">
    <div class="band band-1">
      <strong>1. Data backbone: registrations and communications</strong><br>
      Use Office of the Commissioner of Lobbying (OCL) CSV files.
    </div>
    <div class="band band-2">
      <strong>Registrations</strong><br>
      Define clients, registration identifiers, subject codes, and text descriptions.
    </div>
    <div class="band band-3">
      <strong>Communications</strong><br>
      Define individual reported contacts between clients and Designated Public Office Holders (DPOHs), with dates and links to registrations.
    </div>
    <div class="neck"></div>
  </div>
</div>

--

<div class="smart-funnel">
  <div class="funnel">
    <div class="band band-1">
      <strong>2. Issue definition: RPAA</strong><br>
      Construct registration-level and communication-level text corpora by aggregating relevant text fields for each registration or communication.
    </div>
    <div class="band band-2">
      <strong>Strict RPAA indicator</strong><br>
      Define a strict RPAA indicator based on direct references to the Retail Payment Activities Act and its regulations.
    </div>
    <div class="band band-3">
      <strong>Broad RPAA indicator</strong><br>
      Define a broad RPAA indicator based on RPAA-related expressions (retail payments, payment service providers, payments modernisation, open banking, etc.), including all strict matches.
    </div>
    <div class="band band-3">
      <strong>RPAA flags</strong><br>
      Flag registrations and communications as RPAA-related according to these indicators.
    </div>
    <div class="neck"></div>
  </div>
</div>

--

<div class="smart-funnel">
  <div class="funnel">
    <div class="band band-1">
      <strong>3. Actor universe and side classification</strong><br>
      Define the RPAA actor universe as all clients that appear in at least one RPAA-related registration or communication.
    </div>
    <div class="band band-2">
      <strong>Side classification</strong><br>
      Classify clients into three sides for the RPAA issue.
    </div>
    <div class="band band-3">
      <strong>Client categories</strong>
      <ul>
        <li><strong>Industry / pro-policy side</strong>: banks, payment service providers, fintech firms, industry associations.</li>
        <li><strong>Public-interest side</strong>: consumer advocacy organisations, unions, NGOs with stated public-interest objectives.</li>
        <li><strong>Other / ambiguous</strong>: governments, broad business associations, unclear cases.</li>
      </ul>
    </div>
    <div class="band band-3">
      <strong>Implementation</strong><br>
      Apply keyword-based rules to organisation names and registration text, with scope for manual review.
    </div>
    <div class="neck"></div>
  </div>
</div>

--

<div class="smart-funnel">
  <div class="funnel">
    <div class="band band-1">
      <strong>4. Mapping communications to political units</strong><br>
      For RPAA-related communications, join to the DPOH table so each row becomes a <strong>client–communication–DPOH event</strong>.
    </div>
    <div class="band band-2">
      <strong>DPOH classification</strong>
      <ul>
        <li><strong>Political units</strong>: MPs, Senators, ministers, parliamentary secretaries, and clearly political staff,</li>
        <li><strong>Officials</strong>: non-elected public servants (e.g., deputy ministers, directors, analysts).</li>
      </ul>
    </div>
    <div class="band band-3">
      <strong>Political unit definition</strong><br>
      Define a political <strong>unit</strong> as a person–institution pair (e.g., “Name | House of Commons”, “Name | Finance Canada (FIN)”).
    </div>
    <div class="band band-3">
      <strong>Analogy to AS&amp;W</strong><br>
      This creates a set of political units analogous to AS&amp;W’s senators.
    </div>
    <div class="neck"></div>
  </div>
</div>

--

<div class="smart-funnel">
  <div class="funnel">
    <div class="band band-1">
      <strong>5. Lobbying measures and planned models</strong><br>
      For each political unit $i$, construct:
      <ul>
        <li>$L^P_i$: number of RPAA events where the client is on the industry (pro-policy) side.</li>
        <li>$L^A_i$: number of RPAA events where the client is on the public-interest (anti-policy) side.</li>
        <li>$L^T_i = L^P_i + L^A_i$: total RPAA-related events for unit $i$.</li>
      </ul>
    </div>
    <div class="band band-2">
      <strong>Derive additional variables</strong><br>
      <ul>
        <li>Net difference $\Delta L_i = L^P_i - L^A_i$.</li>
        <li>Shares $s^P_i = \frac{L^P_i}{L^P_i + L^A_i}$, $s^A_i = \frac{L^A_i}{L^P_i + L^A_i}$ when both sides are present.</li>
        <li>Log-transformed and indicator versions (e.g., $\log(1+L^P_i)$, indicator for any lobbying from each side).</li>
      </ul>
    </div>
    <div class="band band-3">
      <strong>Structural controls</strong><br>
      Attach simple structural controls based on DPOH metadata (MP/Senator vs staff, House of Commons vs Senate vs executive/regulators, membership in core financial institutions such as Finance Canada or the Bank of Canada).
    </div>
    <div class="band band-3">
      <strong>Planned estimation approach</strong><br>
      <ul>
        <li>When both sides are sufficiently active, estimate AS&amp;W-style simultaneous equations in $(L^P_i, L^A_i)$, using side-specific variables as instruments as in the original paper.</li>
        <li>When the data do not support a two-sided system, use one-sided OLS specifications for $L^P_i$, treating the AS&amp;W equations as a conceptual benchmark.</li>
      </ul>
    </div>
    <div class="neck"></div>
  </div>
</div>

---
<!-- .slide: class="slide-heading" -->
## Expected Results

<div class="g62-wrap">
  <div class="g62">
    <div class="g62-card">
      <div class="g62-num">1</div>
      <strong>Cross-side patterns</strong><br>
      In a setting where both sides are active, the counteractive-lobbying logic implies that political units with higher lobbying from one side may also be attractive targets for the other side. This would be examined through the relationship between $L^P_i$ and $L^A_i$ at the unit level.
    </div>
    <div class="g62-card">
      <div class="g62-num">2</div>
      <strong>Targeting by predisposition and structure</strong><br>
      The framework allows testing whether coalitions concentrate lobbying on units that are ex ante favourable, unfavourable, or neutral, based on indicators of predisposition.
    </div>
    <div class="g62-card">
      <div class="g62-num">3</div>
      <strong>Concentration of lobbying pressure</strong><br>
      The distribution of $L^T_i$ across political units can be used to assess whether RPAA-related lobbying is concentrated on a limited set of units or more evenly spread. Institutional aggregates can summarise how lobbying is distributed across Parliament, core financial regulators, and other institutions.
    </div>
  </div>
</div>

--
<!-- .slide: class="slide-heading" -->
## Expected Results

<div class="g62-wrap">
  <div class="g62">
    <div class="g62-card">
      <div class="g62-num">4</div>
      <strong>Methodological output</strong><br>
      A reproducible path from registry data to AS&amp;W-style measures $(L^P_i, L^A_i, L^T_i)$ defined at the political-unit level. Conditions under which two-sided estimation of a counteractive system is feasible, and conditions under which only one-sided descriptive analysis is possible.
    </div>
    <div class="g62-card">
      <div class="g62-num">5</div>
      <strong>Future extensions</strong><br>
      Once outcome variables (votes, amendments, speeches, regulatory decisions) are merged to the same political units, the same measures can be used to study whether lobbying exposure is associated with observable policy behaviour.
    </div>
  </div>
</div>

---
<!-- .slide: class="slide-heading" -->
## Q&A