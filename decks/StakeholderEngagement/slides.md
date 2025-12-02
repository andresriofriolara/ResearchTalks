<!-- .slide: class="title-slide" -->
# Counteractive Lobbying: Conceptual Replication in the Canadian Financial Regulation.
</section>

---
<!-- .slide: class="slide-heading" -->
## Motivation

- **Counteractive lobbying as an object of study**  
  - When one coalition lobbies, this can change the incentives of the opposing coalition to lobby the same decision-makers.  
  - This affects which interests are represented around a given policy conflict.

- **From Austen–Smith & Wright (AS&W) to RPAA**  
  - AS&W study counteractive lobbying for a single confirmation conflict in the U.S. Senate.  
  - This project asks whether their logic can be applied to Canadian financial regulation, using RPAA as the focal issue.

- **Why RPAA and the Canadian lobbying registry**  
  - RPAA and its regulations define a single, well-specified policy domain in retail payments.  
  - The federal lobbying registry provides administrative records on registrations and communications, including clients, public office holders, dates, and issue descriptions.  
  - These data can be used to construct measures of lobbying directed at specific political units.

- **Aim of the project**  
  - Use the RPAA case and the registry to implement AS&W-style lobbying measures and examine how their framework can structure an analysis of lobbying around Canadian financial regulation.

---
<!-- .slide: class="slide-heading" -->
## Research Question

> **Can the counteractive lobbying framework of Austen–Smith & Wright be translated to the RPAA setting using the Canadian federal lobbying registry to construct AS&W-style lobbying measures for political units?**

- **Targeting across institutions**  
  - How can we measure which institutions (Parliament, Finance Canada, Bank of Canada, FCAC, other departments) are most involved in RPAA-related lobbying?

- **Targeting across political units**  
  - How can we describe the distribution of lobbying intensity across individual political units (MPs, Senators, ministers, senior officials and staff)?

- **Two sides and their balance**  
  - How can we operationalise “pro-policy” and “anti-policy” sides (industry vs public-interest) in the registry, and under what conditions is it possible to study their interaction at the unit level?

- **Link to outcomes (for later stages)**  
  - How could these lobbying measures later be connected to votes, amendments, speeches, or regulatory decisions, once those outcomes are coded?


---
<!-- .slide: class="slide-heading" -->
## Theoretical Framework


---
<!-- .slide: class="slide-heading" -->
## Empirical Strategy

1. **Data backbone: registrations and communications**  
   - Use Office of the Commissioner of Lobbying (OCL) CSV files.  
   - **Registrations**: define clients, registration identifiers, subject codes, and text descriptions.  
   - **Communications**: define individual reported contacts between clients and Designated Public Office Holders (DPOHs), with dates and links to registrations.

2. **Issue definition: RPAA**  
   - Construct registration-level and communication-level text corpora by aggregating relevant text fields for each registration or communication.  
   - Define a **strict RPAA** indicator based on direct references to the Retail Payment Activities Act and its regulations.  
   - Define a **broad RPAA** indicator based on RPAA-related expressions (retail payments, payment service providers, payments modernisation, open banking, etc.), including all strict matches.  
   - Flag registrations and communications as RPAA-related according to these indicators.

3. **Actor universe and side classification**  
   - Define the RPAA actor universe as all clients that appear in at least one RPAA-related registration or communication.  
   - Classify clients into:  
     - **Industry / pro-policy side** (banks, payment service providers, fintech firms, industry associations),  
     - **Public-interest side** (consumer advocacy organisations, unions, NGOs with stated public-interest objectives),  
     - **Other / ambiguous** (governments, broad business associations, unclear cases).  
   - Apply keyword-based rules to organisation names and registration text, with scope for manual review.

4. **Mapping communications to political units**  
   - For RPAA-related communications, join to the DPOH table so each row becomes a **client–communication–DPOH event**.  
   - Classify DPOHs as:  
     - **Political units**: MPs, Senators, ministers, parliamentary secretaries, and clearly political staff,  
     - **Officials**: non-elected public servants (e.g., deputy ministers, directors, analysts).  
   - Define a political **unit** as a person–institution pair (e.g., “Name | House of Commons”, “Name | Finance Canada (FIN)”).  
   - This creates a set of political units analogous to AS&W’s senators.

5. **Lobbying measures and planned models**  
   - For each political unit \(i\), construct:  
     - \(L^P_i\): number of RPAA events where the client is on the industry (pro-policy) side.  
     - \(L^A_i\): number of RPAA events where the client is on the public-interest (anti-policy) side.  
     - \(L^T_i = L^P_i + L^A_i\): total RPAA-related events for unit \(i\).  
   - Derive additional variables:  
     - Net difference \(\Delta L_i = L^P_i - L^A_i\).  
     - Shares \(s^P_i = \frac{L^P_i}{L^P_i + L^A_i}\), \(s^A_i = \frac{L^A_i}{L^P_i + L^A_i}\) when both sides are present.  
     - Log-transformed and indicator versions (e.g., \(\log(1+L^P_i)\), indicator for any lobbying from each side).  
   - Attach simple structural controls based on DPOH metadata (MP/Senator vs staff, House of Commons vs Senate vs executive/regulators, membership in core financial institutions such as Finance Canada or the Bank of Canada).  
   - **Planned estimation approach:**  
     - When both sides are sufficiently active, estimate AS&W-style simultaneous equations in \((L^P_i, L^A_i)\), using side-specific variables as instruments as in the original paper.  
     - When the data do not support a two-sided system, use one-sided OLS specifications for \(L^P_i\), treating the AS&W equations as a conceptual benchmark.


---
<!-- .slide: class="slide-heading" -->
## Expected Results

- **Cross-side patterns**  
  - In a setting where both sides are active, the counteractive-lobbying logic implies that political units with higher lobbying from one side may also be attractive targets for the other side.  
  - This would be examined through the relationship between \(L^P_i\) and \(L^A_i\) at the unit level.

- **Targeting by predisposition and structure**  
  - The framework allows testing whether coalitions concentrate lobbying on units that are ex ante favourable, unfavourable, or neutral, based on indicators of predisposition.  
  - Unit-level lobbying measures can be related to structural variables such as institutional position, committee roles, and vulnerability measures.

- **Concentration of lobbying pressure**  
  - The distribution of \(L^T_i\) across political units can be used to assess whether RPAA-related lobbying is concentrated on a limited set of units or more evenly spread.  
  - Institutional aggregates can summarise how lobbying is distributed across Parliament, core financial regulators, and other institutions.

- **Methodological output**  
  - A reproducible path from registry data to AS&W-style measures \((L^P_i, L^A_i, L^T_i)\) defined at the political-unit level.  
  - Conditions under which two-sided estimation of a counteractive system is feasible, and conditions under which only one-sided descriptive analysis is possible.

- **Future extensions**  
  - Once outcome variables (votes, amendments, speeches, regulatory decisions) are merged to the same political units, the same measures can be used to study whether lobbying exposure is associated with observable policy behaviour.

---
<!-- .slide: class="slide-heading" -->
## Q&A