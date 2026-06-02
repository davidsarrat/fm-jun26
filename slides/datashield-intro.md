## DataSHIELD: data stays, answers travel

<div style="margin-top:0.3em;">
<svg viewBox="0 0 720 200" style="width:100%; max-height: 235px;">

  <!-- Hospital server + researcher (click 1) -->
  <g v-click="1">
    <rect x="30" y="35" width="210" height="135" rx="12" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.20)" stroke-width="1"/>
    <text x="135" y="55" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6" font-weight="500">Hospital server</text>
    <ellipse cx="135" cy="88" rx="32" ry="8" fill="rgba(255,179,102,0.15)" stroke="#ffb366" stroke-width="1"/>
    <path d="M103,88 V118 a32,8 0 0 0 64,0 V88" fill="rgba(255,179,102,0.10)" stroke="#ffb366" stroke-width="1"/>
    <text x="135" y="152" text-anchor="middle" fill="#ffb366" font-family="Roboto Mono" font-size="4.2">raw records stay here</text>

    <rect x="500" y="62" width="190" height="86" rx="12" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.12)" stroke-width="1"/>
    <circle cx="595" cy="92" r="9" fill="none" stroke="#e0d8d0" stroke-width="1.3"/>
    <path d="M580,113 C580,100 610,100 610,113" fill="none" stroke="#e0d8d0" stroke-width="1.3"/>
    <text x="595" y="138" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="5">Researcher</text>
  </g>

  <!-- Authorized access (click 2) -->
  <g v-click="2">
    <line x1="250" y1="105" x2="495" y2="105" stroke="rgba(102,221,170,0.30)" stroke-width="1" stroke-dasharray="3 3"/>
    <text x="372" y="100" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="4.4">authorized access</text>
  </g>

  <!-- Query up + aggregate down (click 3) -->
  <g v-click="3">
    <path d="M495,80 C420,55 320,55 248,70" fill="none" stroke="#FFD000" stroke-width="2.2" stroke-dasharray="7 5">
      <animate attributeName="stroke-dashoffset" from="0" to="-12" dur="0.8s" repeatCount="indefinite"/>
    </path>
    <text x="372" y="48" text-anchor="middle" fill="#FFD000" font-family="Roboto Mono" font-size="4.2">analysis request</text>
    <path d="M248,134 C320,150 420,150 495,130" fill="none" stroke="#66ddaa" stroke-width="2.2" stroke-dasharray="7 5">
      <animate attributeName="stroke-dashoffset" from="0" to="-12" dur="0.8s" repeatCount="indefinite"/>
    </path>
    <text x="372" y="170" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="4.2">aggregate result</text>
  </g>

</svg>
</div>

<div v-click="3" class="text-center" style="font-size:0.9em; color:#c8b8a8; margin-top:0.2em;">
<strong style="color:#66ddaa;">Only aggregate statistics leave the server</strong> &mdash; never individual-level records, and the originals can't be reconstructed.
</div>

<div v-click="4">
<div style="text-align:center; font-family:'Roboto Mono'; font-size:0.7em; color:#8a7d70; letter-spacing:0.06em; margin-top:0.7em;">ENFORCED BY DISCLOSURE CONTROL</div>
<div class="grid grid-cols-4 gap-3" style="margin-top:0.4em;">
  <div style="background:rgba(102,221,170,0.06); border:1px solid rgba(102,221,170,0.18); border-radius:8px; padding:0.55em;">
    <div style="font-family:'Roboto Mono'; color:#66ddaa; font-size:0.76em; font-weight:600;">Minimum count</div>
    <div style="font-size:0.64em; color:#b0b8c0; margin-top:0.2em;">No cell or subgroup below 3 is ever returned.</div>
  </div>
  <div style="background:rgba(102,221,170,0.06); border:1px solid rgba(102,221,170,0.18); border-radius:8px; padding:0.55em;">
    <div style="font-family:'Roboto Mono'; color:#66ddaa; font-size:0.76em; font-weight:600;">Approved functions</div>
    <div style="font-size:0.64em; color:#b0b8c0; margin-top:0.2em;">No raw-data access, no arbitrary code &mdash; only vetted functions run.</div>
  </div>
  <div style="background:rgba(102,221,170,0.06); border:1px solid rgba(102,221,170,0.18); border-radius:8px; padding:0.55em;">
    <div style="font-family:'Roboto Mono'; color:#66ddaa; font-size:0.76em; font-weight:600;">Model limits</div>
    <div style="font-size:0.64em; color:#b0b8c0; margin-top:0.2em;">Too many parameters per subject is blocked, so a model can't memorize people.</div>
  </div>
  <div style="background:rgba(102,221,170,0.06); border:1px solid rgba(102,221,170,0.18); border-radius:8px; padding:0.55em;">
    <div style="font-family:'Roboto Mono'; color:#66ddaa; font-size:0.76em; font-weight:600;">Anonymised plots</div>
    <div style="font-size:0.64em; color:#b0b8c0; margin-top:0.2em;">Graphs use k-nearest-neighbour centroids and added noise, never raw points.</div>
  </div>
</div>
</div>
