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
		\eta_k x, & \text{if } x \geq 0 \quad \text{(gain)}

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

$
\mu_k(c_k,r_k) =
\begin{cases}
  \eta_k\, x_k^{\alpha_k}, & \text{if } x_k \ge 0 \quad \text{(gain)}
  -\eta_k\,\lambda_k\, (-x_k)^{\gamma_k}, & \text{if } x_k < 0 \quad \text{(loss)}
\end{cases}
\qquad x_k=c_k-r_k.
$

Where,
- $\eta_k>0$ : sensitivity factor
- $\lambda_k \ge 1$ : loss-aversion parameter
- $\alpha_k \in (0,1]$ : gains
- $\gamma_k \in (0,1]$ : losses

--

## Hybrid Model (quasi-hyperbolic discounting with explicit risk preferences)

$$U_t = \sum_{k=1}^{K} \left[ \frac{(c_{t}^{k})^{1 - \rho}}{1 - \rho} + \mu_k(c_{t}^{k}, r_{t}^{k}) \right] + \beta \sum_{\tau = t+1}^{T} \delta^{\tau - t} \sum_{k=1}^{K} \left[ \frac{(c_{\tau} ^{k})^{1 - \rho}}{1 - \rho} + \mu_k(c_{\tau}^{k}, r_{\tau}^{k}) \right]$$

--

## A Final Adjustment

- $A_t$ : available menu
- $F(A_t)$ : feasible attention sets
- $S_t\subseteq(A_t)$ : consideration set endogenously chosen
- feasible utility path:
$$\tilde{U}_t = \max_{c_t \in S_t} \left[ u(c_t \mid r_t) + \beta \sum_{\tau = t+1}^{T} \delta^{\tau - t} \mathbb{E}_{S_\tau} \left[ u(c_\tau \mid r_\tau) \right] \right]$$

- $\Theta_t$ : a point given at time t
- $u(c_t \mid r_t) \geq \theta_t$ : satisfaction point
- Constrained to $c_t \in S_t \subseteq A_t$

$$U_t = \sum_{k=1}^{K} \left[ \frac{(c_{t}^{k})^{1 - \rho}}{1 - \rho} + \mu_k(c_{t}^{k}, r_{t}^{k}) \right] + \beta \sum_{\tau = t+1}^{T} \delta^{\tau - t} \sum_{k=1}^{K} \left[ \frac{(c_{\tau}^{k})^{1 - \rho}}{1 - \rho} + \mu_k(c_{\tau}^{k}, r_{\tau}^{k}) \right]$$

--
## The decision Rule

Utility function for each potential scenario:
- When Right:
  - $U_1$, when $\mathop{\mathbb{E}}(P_a)$ when customer expected probability $P_i$ is read as it landed above the threshold and that it was accepted.
  - $U_4$ , when $\mathop{\mathbb{E}}(P_b)$ of the expected repayment probability $P_i$, given by $(1-P_a)$ is read as it landed below the threshold and that it was rejected.

- When Wrong:
  - $U_3$ Type I Error
  - $U_2$ Type II Error

Each Scenario Probability of Accepting and rejecting given by:

$$\mathop{\mathbb{E}}\left[U|\text{Accept}\right]=P_aU_1+P_bU_2$$
$$\mathop{\mathbb{E}}\left[U|\text{Reject}\right]=P_aU_3+P_bU_4$$

In a multi-scenario task the decision maker will rank the utilities from the highest to the lowest.

---
## A Blur in the Perceived Feasibility Frontier

Add the images

--
## The effect of an Ancillary condition "d" (Clippel, Nd)

- $\Psi$ : bias (present bias)
- $\lambda$ : risk preference
- Decision set:

$$L=C(\{ x,y \}, \Psi, \lambda) \textnormal{ where, } (x,y)\in \mathbb{R}^2_+ $$

And the frontier:

$$y=\left(1-\left(\frac{x}{\psi}\right)^{1-\lambda}\right)^{1-\lambda}$$

-- 
## The Frontier perception shift and inter-temporal effect

- Distorded decision set:
$$\psi_t=\psi(\psi_{t-1},A_t)$$
- Inter-temporal effect of time dependency:
$$\text{where, } x\in [0,\psi_t] \text{ and, } \lambda \in (0,1)$$


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