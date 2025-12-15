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

**Plain**
You notice what’s happening, choose what to do next, act, see what happens, and adjust your habits.

**Practical**
Absorb information, form a workable understanding, select an action based on expected results, then compare the outcome to goals to update expectations and refine habits.

**Formal**
An agent senses the environment to form a state estimate. It then predicts consequences and decides on an action (judgment). After acting, it compares outcomes to expectations, using any mismatch as error to update its policy.

**Elvish**
Cognition can be modeled as a closed-loop controller. Sensory streams are converted into beliefs about world states, often probabilistic and shaped by priors and context, which then parameterize generative predictions and action policies that balance goals, risk, and resource constraints. Actions perturb the environment, so perception and control continuously co-determine the incoming data. Feedback yields prediction errors at multiple levels (perceptual, model-based, value-based), and learning updates representations, dynamics models, and policies to reduce expected surprise or cost while improving effective control under uncertainty.

**Math**
At time $t$, the system receives an observation $o_t$ and infers a latent state $s_t$ (state estimation). The agent evaluates candidate actions using a dynamics model and/or value function, selecting control via a policy $a_t = \pi(s_t)$. After executing $a_t$, it receives new observations (and reward/cost $r_{t+1}$) and infers $s_{t+1}$. It computes prediction errors, e.g., a state/model error $e^s_t = s_{t+1} - f_\theta(s_t, a_t)$ and/or a reward prediction error $\delta_t = r_{t+1} + \gamma V(s_{t+1}) - V(s_t)$, and uses these signals to update parameters $\theta$ of the estimator, model, and policy. Over time, this reduces prediction error and improves $\mathbb{E}[\mathrm{Utility}]$.

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
