---
layout: default
title: "Loop"
permalink: /loop/
parent: Argument
nav_order: 2
---

# Loop 
_Analogy and Metaphor_

---
## X Axis

### Plain
You notice what’s happening, choose what to do next, act, see what happens, and adjust your habits.

### Practical
Absorb information, form a workable understanding, select an action based on expected results, then compare the outcome to goals to update expectations and refine habits.

### Formal
An agent senses the environment to form a state estimate. It then predicts consequences and decides on an action (judgment). After acting, it compares outcomes to expectations, using any mismatch as error to update its policy.

### Elvish
Cognition can be modeled as a closed-loop controller. Sensory streams are converted into beliefs about world states, often probabilistic and shaped by priors and context, which then parameterize generative predictions and action policies that balance goals, risk, and resource constraints. Actions perturb the environment, so perception and control continuously co-determine the incoming data. Feedback yields prediction errors at multiple levels (perceptual, model-based, value-based), and learning updates representations, dynamics models, and policies to reduce expected surprise or cost while improving effective control under uncertainty.

### Math
At time $t$, each agent $i$ receives a local observation $o^i_t$ (including relevant price signals $p_t$) and infers an internal interpretation $s^i_t = \phi_{\theta_i}(o^i_{\le t}, p_{\le t})$. The agent selects an action via a policy $a^i_t = \pi_{\psi_i}(s^i_t)$ (subject to constraints). After executing $a^i_t$, it receives new observations $o^i_{t+1}$ (including updated prices $p_{t+1}$) and infers $s^i_{t+1} = \phi_{\theta_i}(o^i_{\le t+1}, p_{\le t+1})$. It computes discrepancy/feedback signals, e.g., an interpretive/model error $e^i_t = s^i_{t+1} - f_{\theta_i}(s^i_t, a^i_t)$ and profit/loss $\pi^i_{t+1} = \mathrm{rev}^i_{t+1} - \mathrm{cost}^i_{t+1}$ (optionally $\delta^i_t = \pi^i_{t+1} - \mathbb{E}t[\pi^i{t+1}]$), and uses these signals to update parameters $(\theta_i,\psi_i)$.

At time $t$, each agent $i$ receives a local observation $o_t^i$ (including relevant price signals $p_t$) and infers an internal interpretation
$$
s_t^i = \phi_{\theta_i}\!\left(o_{\le t}^i,\; p_{\le t}\right).
$$
The agent selects an action via a policy
$$
a_t^i = \pi_{\psi_i}\!\left(s_t^i\right)
$$
(subject to constraints). After executing $a_t^i$, it receives new observations $o_{t+1}^i$ (including updated prices $p_{t+1}$) and infers
$$
s_{t+1}^i = \phi_{\theta_i}\!\left(o_{\le t+1}^i,\; p_{\le t+1}\right).
$$
It computes discrepancy/feedback signals, e.g., an interpretive/model error
$$
e_t^i = s_{t+1}^i - f_{\theta_i}\!\left(s_t^i,\; a_t^i\right)
$$
and profit/loss
$$
\pi_{t+1}^i = \mathrm{rev}_{t+1}^i - \mathrm{cost}_{t+1}^i
$$
(optionally
$$
\delta_t^i = \pi_{t+1}^i - \mathbb{E}_t\!\left[\pi_{t+1}^i\right]
$$
), and uses these signals to update parameters $(\theta_i,\psi_i)$.


---
## Y Axis



---

<div class="urdu" lang="ur" dir="rtl">
  <div class="verses">
    <div class="misra">یارب وہ نہ سمجھے ہیں نہ سمجھیں گے مری بات</div>
    <div class="misra">دے اور دل ان کو جو نہ دے مجھ کو زباں اور</div>
    <div class="poet">— مرزا غالبؔ</div>
  </div>
</div>
