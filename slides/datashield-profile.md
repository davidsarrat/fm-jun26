## DataSHIELD on its own

<div class="grid grid-cols-2 gap-6" style="margin-top:1.5em;">

  <div>
    <div style="font-family:'Roboto Mono'; color:#66ddaa; font-size:0.78em; font-weight:700; letter-spacing:0.1em; margin-bottom:0.8em; text-align:center;">STRENGTHS</div>

    <div v-click="1" class="trait" style="border-color:rgba(102,221,170,0.28); background:rgba(102,221,170,0.06);">
      <svg viewBox="0 0 24 24" width="20" height="20"><circle cx="12" cy="12" r="10" fill="none" stroke="#66ddaa" stroke-width="2"/><path d="M7.5 12.5l3 3 6-6.5" fill="none" stroke="#66ddaa" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
      <div>
        <div class="trait-label" style="color:#66ddaa;">Privacy-preservation expertise</div>
        <div class="trait-sub">A decade of disclosure control: minimum cell counts, approved functions, only non-disclosive summaries leave. Raw data never leaves the site.</div>
      </div>
    </div>

    <div v-click="2" class="trait" style="border-color:rgba(102,221,170,0.28); background:rgba(102,221,170,0.06);">
      <svg viewBox="0 0 24 24" width="20" height="20"><circle cx="12" cy="12" r="10" fill="none" stroke="#66ddaa" stroke-width="2"/><path d="M7.5 12.5l3 3 6-6.5" fill="none" stroke="#66ddaa" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
      <div>
        <div class="trait-label" style="color:#66ddaa;">Institutional trust and adoption</div>
        <div class="trait-sub">Years embedded in biomedical institutions: ethics-board, legal and data-custodian approval already secured across hospital networks and consortia.</div>
      </div>
    </div>
  </div>

  <div>
    <div style="font-family:'Roboto Mono'; color:#ff6b6b; font-size:0.78em; font-weight:700; letter-spacing:0.1em; margin-bottom:0.8em; text-align:center;">GAPS</div>

    <div v-click="3" class="trait" style="border-color:rgba(255,107,107,0.28); background:rgba(255,107,107,0.06);">
      <svg viewBox="0 0 24 24" width="20" height="20"><circle cx="12" cy="12" r="10" fill="none" stroke="#ff6b6b" stroke-width="2"/><path d="M8.5 8.5l7 7M15.5 8.5l-7 7" fill="none" stroke="#ff6b6b" stroke-width="2" stroke-linecap="round"/></svg>
      <div>
        <div class="trait-label" style="color:#ff6b6b;">Built for simple statistical studies</div>
        <div class="trait-sub">Designed for classical epidemiology: means, contingency tables, GLMs. The engine runs one-shot aggregate queries, not heavy or iterative computation.</div>
      </div>
    </div>

    <div v-click="4" class="trait" style="border-color:rgba(255,107,107,0.28); background:rgba(255,107,107,0.06);">
      <svg viewBox="0 0 24 24" width="20" height="20"><circle cx="12" cy="12" r="10" fill="none" stroke="#ff6b6b" stroke-width="2"/><path d="M8.5 8.5l7 7M15.5 8.5l-7 7" fill="none" stroke="#ff6b6b" stroke-width="2" stroke-linecap="round"/></svg>
      <div>
        <div class="trait-label" style="color:#ff6b6b;">No machine-learning tools</div>
        <div class="trait-sub">No engine to train a model over many rounds: no parameter exchange, no aggregation strategies, no neural networks, gradient-boosted trees or imaging.</div>
      </div>
    </div>
  </div>

</div>

<div v-click="5" class="text-center" style="margin-top:1.3em; font-size:0.9em; color:#c8b8a8;">
The strengths took a decade of institutional trust to earn. The gaps are engineering, and that is exactly what a federated-learning framework provides.
</div>

<style scoped>
.trait {
  display: flex;
  gap: 0.7em;
  align-items: flex-start;
  border: 1px solid;
  border-radius: 10px;
  padding: 0.8em 0.9em;
  margin-bottom: 0.8em;
}
.trait svg { flex: 0 0 auto; margin-top: 0.1em; }
.trait-label {
  font-family: 'Roboto Mono', monospace;
  font-size: 0.92em;
  font-weight: 600;
  margin-bottom: 0.25em;
}
.trait-sub {
  font-size: 0.72em;
  color: #b0b8c0;
  line-height: 1.4;
}
</style>
