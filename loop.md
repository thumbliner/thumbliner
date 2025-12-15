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
You notice what’s happening, choose what to do next, act, see what happens, and learn.

### Practical
Absorb information, form a workable understanding, select an action based on expected results, then compare the outcome to goals to update expectations and refine habits.

### Formal
An agent senses the environment to form a state estimate. It then predicts consequences and decides on an action (judgment). After acting, it compares outcomes to expectations, using any mismatch as error to update its policy.

### Elvish
Cognition is closed-loop information processing: an agent perceives only a limited slice of the world, treats what it senses as local evidence, and also ingests compact “price-like” signals that summarize constraints and opportunities in a cost environment; it turns that evidence into beliefs about what is happening, uses a dynamic world model to form probabilistic expectation about what it should observe next and what its actions will cause, and then applies judgment to choose control actions that are feasible and norm-compliant given limits like capability, budgets, and risk rules; because acting changes the environment and therefore the next evidence, perception shapes belief, belief drives prediction, and prediction guides action rather than forming a one-way input–output mapping; after acting, the agent re-observes, computes expected surprise by comparing what its beliefs and policy implied should happen with what actually happened, treats mismatches as multi-level errors (perceptual, model-based, and value-based), and uses these feedback to update the parameters governing both interpretation and action to reduce systematic error and improve effective control under uncertainty.

### Math
At time 
$$t$$, each agent 
$$
i
$$
receives a local observation 
$$
o_t^i
$$
(including relevant price signals 
$$
p_t$$) and infers an internal interpretation
$$
s_t^i = \phi_{\theta_i}\!\left(o_{\le t}^i,\; p_{\le t}\right).
$$
The agent selects an action via a policy
$$
a_t^i = \pi_{\psi_i}\!\left(s_t^i\right)
$$
(subject to constraints). After executing 
$$
a_t^i
$$
, it receives new observations 
$$
o_{t+1}^i
$$
(including updated prices 
$$
p_{t+1}
$$
) and infers
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
), and uses these signals to update parameters 
$$
(\theta_i,\psi_i)
$$.


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
