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

At time 
𝑡
t, each agent 
𝑖
i receives a local observation 
𝑜
𝑡
𝑖
o
t
i
	​

 (including relevant price signals 
𝑝
𝑡
p
t
	​

) and infers an internal interpretation 
𝑠
𝑡
𝑖
=
𝜙
𝜃
𝑖
(
𝑜
≤
𝑡
𝑖
,
𝑝
≤
𝑡
)
s
t
i
	​

=ϕ
θ
i
	​

	​

(o
≤t
i
	​

,p
≤t
	​

). The agent selects an action via a policy 
𝑎
𝑡
𝑖
=
𝜋
𝜓
𝑖
(
𝑠
𝑡
𝑖
)
a
t
i
	​

=π
ψ
i
	​

	​

(s
t
i
	​

) (subject to constraints). After executing 
𝑎
𝑡
𝑖
a
t
i
	​

, it receives new observations 
𝑜
𝑡
+
1
𝑖
o
t+1
i
	​

 (including updated prices 
𝑝
𝑡
+
1
p
t+1
	​

) and infers 
𝑠
𝑡
+
1
𝑖
=
𝜙
𝜃
𝑖
(
𝑜
≤
𝑡
+
1
𝑖
,
𝑝
≤
𝑡
+
1
)
s
t+1
i
	​

=ϕ
θ
i
	​

	​

(o
≤t+1
i
	​

,p
≤t+1
	​

). It computes discrepancy/feedback signals, e.g., an interpretive/model error 
𝑒
𝑡
𝑖
=
𝑠
𝑡
+
1
𝑖
−
𝑓
𝜃
𝑖
(
𝑠
𝑡
𝑖
,
𝑎
𝑡
𝑖
)
e
t
i
	​

=s
t+1
i
	​

−f
θ
i
	​

	​

(s
t
i
	​

,a
t
i
	​

) and profit/loss 
𝜋
𝑡
+
1
𝑖
=
r
e
v
𝑡
+
1
𝑖
−
c
o
s
t
𝑡
+
1
𝑖
π
t+1
i
	​

=rev
t+1
i
	​

−cost
t+1
i
	​

 (optionally 
𝛿
𝑡
𝑖
=
𝜋
𝑡
+
1
𝑖
−
𝐸
𝑡
[
𝜋
𝑡
+
1
𝑖
]
δ
t
i
	​

=π
t+1
i
	​

−E
t
	​

[π
t+1
i
	​

]), and uses these signals to update parameters 
(
𝜃
𝑖
,
𝜓
𝑖
)
(θ
i
	​

,ψ
i
	​

).

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
