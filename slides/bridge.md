## Where DataSHIELD stops

<div class="grid grid-cols-2 gap-8 mt-3">
<div>

For over a decade, DataSHIELD has let researchers ask **statistical questions** across hospitals &mdash; means, contingency tables, GLMs, survival curves &mdash; computed locally, with only **non-disclosive summaries** ever leaving.

<div class="mt-3" v-click>

But a single aggregate query can't express a **machine-learning model**. Neural networks, gradient-boosted trees and imaging models are learned over **many rounds** of back-and-forth.

</div>

</div>
<div v-click="2">

<div class="step-card" style="border-color: rgba(255,208,0,0.25);">

**dsFlower keeps the exact same trust model.**

- Data still **never leaves** the hospital
- Each site still computes **locally**
- The only thing that travels is now a **model update** instead of a summary statistic

</div>

<div class="mt-3" style="font-size: 0.9em; color: #c8b8a8;">

Federated learning, brought inside the DataSHIELD world.

</div>

</div>
</div>
