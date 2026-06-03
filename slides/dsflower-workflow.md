## dsFlower Workflow

<div style="margin-top: 0.2em;">
<svg viewBox="0 0 810 340" style="width: 100%; max-height: 330px;">

  <defs>
    <linearGradient id="privGrad" x1="0%" y1="0%" x2="100%" y2="100%" spreadMethod="reflect">
      <stop offset="0%" stop-color="#00E5FF"/>
      <stop offset="20%" stop-color="#7B2FF7"/>
      <stop offset="40%" stop-color="#FF4D9D"/>
      <stop offset="50%" stop-color="#FFFFFF"/>
      <stop offset="60%" stop-color="#FF4D9D"/>
      <stop offset="80%" stop-color="#7B2FF7"/>
      <stop offset="100%" stop-color="#00E5FF"/>
      <animateTransform attributeName="gradientTransform" type="translate" values="-0.85 -0.85; 0.85 0.85; -0.85 -0.85" dur="3s" repeatCount="indefinite"/>
    </linearGradient>
  </defs>

  <!-- SuperNode nodes (top row) -->
  <g transform="translate(120,65)">
    <rect x="-80" y="-40" width="160" height="80" rx="14" :fill="$clicks>=1 ? 'rgba(157,78,221,0.16)' : 'rgba(136,204,255,0.08)'" :stroke="$clicks>=1 ? 'url(#privGrad)' : 'rgba(136,204,255,0.20)'" :stroke-width="$clicks>=1 ? 2 : 1"/>
    <text y="-4" text-anchor="middle" :fill="$clicks>=1 ? 'url(#privGrad)' : '#88ccff'" font-family="Roboto Mono" font-size="5" font-weight="500">SuperNode</text>
    <text y="14" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4" font-weight="500">Hospital A</text>
    <text y="28" text-anchor="middle" fill="#ffb366" font-family="Roboto Mono" font-size="2.8">own data</text>
  </g>

  <g transform="translate(350,65)">
    <rect x="-80" y="-40" width="160" height="80" rx="14" :fill="$clicks>=1 ? 'rgba(157,78,221,0.16)' : 'rgba(136,204,255,0.08)'" :stroke="$clicks>=1 ? 'url(#privGrad)' : 'rgba(136,204,255,0.20)'" :stroke-width="$clicks>=1 ? 2 : 1"/>
    <text y="-4" text-anchor="middle" :fill="$clicks>=1 ? 'url(#privGrad)' : '#88ccff'" font-family="Roboto Mono" font-size="5" font-weight="500">SuperNode</text>
    <text y="14" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4" font-weight="500">Hospital B</text>
    <text y="28" text-anchor="middle" fill="#ffb366" font-family="Roboto Mono" font-size="2.8">own data</text>
  </g>

  <g transform="translate(580,65)">
    <rect x="-80" y="-40" width="160" height="80" rx="14" :fill="$clicks>=1 ? 'rgba(157,78,221,0.16)' : 'rgba(136,204,255,0.08)'" :stroke="$clicks>=1 ? 'url(#privGrad)' : 'rgba(136,204,255,0.20)'" :stroke-width="$clicks>=1 ? 2 : 1"/>
    <text y="-4" text-anchor="middle" :fill="$clicks>=1 ? 'url(#privGrad)' : '#88ccff'" font-family="Roboto Mono" font-size="5" font-weight="500">SuperNode</text>
    <text y="14" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4" font-weight="500">Hospital C</text>
    <text y="28" text-anchor="middle" fill="#ffb366" font-family="Roboto Mono" font-size="2.8">own data</text>
  </g>

  <!-- Server-side annotation -->
  <text x="735" y="52" fill="#88ccff" font-family="Roboto Mono" font-size="3.5" text-anchor="middle">Local Training</text>
  <text x="735" y="64" fill="#b0b8c0" font-family="Roboto Mono" font-size="2.5" text-anchor="middle">+</text>
  <text x="735" y="76" :fill="$clicks>=1 ? 'url(#privGrad)' : '#b0b8c0'" font-family="Roboto Mono" :font-size="$clicks>=1 ? 3.5 : 3" text-anchor="middle" class="g-term" data-g="Trust profiles" style="cursor:pointer;">Privacy Controls</text>

  <!-- SuperLink node (bottom center) -->
  <g transform="translate(350,280)">
    <rect x="-100" y="-38" width="200" height="76" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.20)" stroke-width="1"/>
    <text y="-6" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6" font-weight="500">SuperLink</text>
    <text y="16" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4" font-weight="500">Analyst</text>
  </g>

  <!-- Aggregation label (right of SuperLink) -->
  <text x="470" y="276" fill="#88ccff" font-family="Roboto Mono" font-size="3.5" class="g-term" data-g="FedAvg / FedProx / FedOpt" style="cursor:pointer;">Federated Aggregation</text>
  <text x="470" y="290" fill="#b0b8c0" font-family="Roboto Mono" font-size="3">Orchestrator Role</text>

  <!-- Global model broadcast UP (yellow) -->
  <path d="M335,242 C260,185 125,145 105,105" fill="none" stroke="#ffaacc" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <path d="M335,242 L340,105" fill="none" stroke="#ffaacc" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <path d="M335,242 C400,185 535,145 565,105" fill="none" stroke="#ffaacc" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>

  <!-- Weight updates DOWN (green) -->
  <path d="M140,105 C170,155 305,195 365,242" fill="none" stroke="#88ccff" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <path d="M360,105 L365,242" fill="none" stroke="#88ccff" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <path d="M600,105 C570,155 435,195 365,242" fill="none" stroke="#88ccff" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>

  <!-- Label paths (unique IDs to avoid collision with slide 2) -->
  <path id="flQL" d="M82,118 C108,160 245,200 320,258" fill="none" stroke="none"/>
  <path id="flRL" d="M122,88 C148,135 280,172 348,225" fill="none" stroke="none"/>
  <path id="flQR" d="M352,218 C420,165 552,128 578,80" fill="none" stroke="none"/>
  <path id="flRR" d="M385,252 C455,205 588,165 622,115" fill="none" stroke="none"/>

  <!-- Labels -->
  <text fill="#ffaacc" font-family="Roboto Mono" font-size="3.5" text-anchor="middle"><textPath href="#flQL" startOffset="50%">global model</textPath></text>
  <text fill="#88ccff" font-family="Roboto Mono" font-size="3.5" text-anchor="middle"><textPath href="#flRL" startOffset="50%">weight updates</textPath></text>
  <text fill="#ffaacc" font-family="Roboto Mono" font-size="3.5" text-anchor="middle"><textPath href="#flQR" startOffset="50%">global model</textPath></text>
  <text fill="#88ccff" font-family="Roboto Mono" font-size="3.5" text-anchor="middle"><textPath href="#flRR" startOffset="50%">weight updates</textPath></text>

  <!-- Privacy origin info box (appears on click, under Privacy Controls) -->
  <foreignObject x="662" y="108" width="144" height="104" v-click="1">
    <div xmlns="http://www.w3.org/1999/xhtml" class="priv-info">
      <div class="priv-info-title">Protection starts at the node</div>
      <div class="priv-info-body">Privacy controls act on every weight update before it ever reaches the analyst's SuperLink.</div>
    </div>
  </foreignObject>

</svg>
</div>

Model weights flow via **gRPC/TLS**. Raw data stays on each hospital's server. Only weight deltas travel.

<style>
.priv-info {
  height: 100%;
  box-sizing: border-box;
  border-radius: 7px;
  padding: 6px 8px;
  background: linear-gradient(135deg, rgba(157,78,221,0.20), rgba(255,77,157,0.12));
  border: 1px solid rgba(255,120,200,0.5);
}
.priv-info-title {
  font-family: 'Roboto Mono', monospace;
  font-weight: 700;
  font-size: 8px;
  line-height: 1.2;
  margin-bottom: 4px;
  background: linear-gradient(135deg, #C77DFF, #FF4D9D);
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  color: transparent;
}
.priv-info-body {
  font-family: 'Montserrat', sans-serif;
  font-size: 6.5px;
  line-height: 1.4;
  color: #ece3f5;
}
</style>
