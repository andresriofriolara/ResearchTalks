<section class="title-slide">
A Dissection of Collateral’s Bounded Rationality
<div class="subtitle">Ivey Doctoral Research Seminaries Series | <em>November 14th, 2025</em></div>
</section>

---

## Why we care
- **How much in bank accounts**
    - Avg Canadian checking account balance
    - Avg credit dollar per checking account balance

---
## Who would you rather decide on your money?

<div class="cols" style="min-height:70vh; align-items:center; justify-items:center; gap:64px;">
  <img data-src="./images/einsten.jpg" style="max-height:60vh; width:auto;" alt="Einstein">
  <img data-src="./images/homer.webp" style="max-height:60vh; width:auto;" alt="Homer">
</div>

---
## Research Question

<div style="min-height:10vh; display:grid; place-items:center; text-align:center;">
  <h2>Perfectly Centered</h2>
  <p>How and to which magnitude can the effect of present bias be decreased in loan granting?</p>
</div>


---
## Banking process (Rational)

Figures from theoretical framework

---
## Banking process (Heuristics)

Figures from theoretical framework

---
## The Model

--
## Intertemporal Choice Component (Laibson, 1997)

$$U_t = u(c_t) + \beta \sum_{\tau = t+1}^{T} \delta^{\tau - t} u(c_\tau)$$

Where,

- $u(c_t)$ : instant utility from consumption $c_t$
- $\beta$ : present-bias parameter $\beta \in(0,1]$
- $\delta$ : discount factor $\delta\in(0,1)$
- $T$ : the time horizon

--

## Reference-Dependent Preferences (Koszegi and Rabin, 2006)

$$U(c \mid r) = m(c) + \sum_{k=1}^{K} \mu_k \left[ m_k(c_k) - m_k(r_k) \right]$$

Where,

- $c=(c^1,...,C^K)$ : vector over k dimensions
- $c^k$ : realized outcome in k dimension
- $m(c)$ : total consumption utility $\sum_{k=1}^{K} m_k(c_k)$
- $r^k$ : agent's rational outcome expectations on $c^k$
- $m^k(\cdot)$ : consumption utility function for k dimension
- $\mu_k(\cdot)$ : the gain-loss utility function*

--

## Gain-Loss Utility Function Capturing Reference Dependence (Koszegi and Rabin, 2006)

$$
\mu_k(x) = 
	\begin{cases}
		\eta_k x, & \text{if } x \geq 0 \quad \text{(gain)} \\
		\eta_k \lambda_k x, & \text{if } x < 0 \quad \text{(loss)}
	\end{cases}
$$

Where,

- $\eta_k$ : scale of sensitivity to gain/losses
- $\lambda_k$ : loss aversion parameter

--

## Adjusting the deviation-based structure with a CRRA form

$m^k(c^k)$ is replaced with $u(c^k)$

Giving:

$$
\mu_k(c_k,r_k) =
\begin{cases}
\eta_k\, x_k^{\alpha_k}, & \text{if } x_k \ge 0 \quad \text{(gain)}\\[6pt]
-\eta_k\,\lambda_k\, (-x_k)^{\gamma_k}, & \text{if } x_k < 0 \quad \text{(loss)}
\end{cases}
\qquad x_k=c_k-r_k.
$$

Where,
- $\eta_k>0$ : sensitivity factor
- $\lambda_k \ge 1$ : loss-aversion parameter
- $\alpha_k \in (0,1]$ : gains
- $\gamma_k \in (0,1]$ : losses

--
## decision rule


--
## frontier


---
## The Experimental Design

- Lab Experiment Proposed
- Field Experiment Proposed

--

## Lab Experiment

--

## Field Experiment

---

## Empirical Strategy

- **MLE**

---

## Preliminary Results

---

## Q&A