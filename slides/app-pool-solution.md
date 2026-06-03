## Possible dsFlower approach

<div style="margin-top: 0.1em;">
<svg viewBox="0 0 940 410" style="width: 100%; max-height: 420px;">

  <!-- Trusted reviewer -->
  <rect x="38" y="58" width="212" height="118" rx="14" fill="rgba(102,221,170,0.10)" stroke="rgba(102,221,170,0.30)" stroke-width="1.5"/>
  <circle cx="140" cy="82" r="7" fill="none" stroke="#66ddaa" stroke-width="1.7"/>
  <line x1="145" y1="87" x2="151" y2="93" stroke="#66ddaa" stroke-width="1.9" stroke-linecap="round"/>
  <text x="144" y="116" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="5" font-weight="600">Trusted reviewer</text>
  <text x="144" y="131" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="3.9">biomedical / DataSHIELD</text>
  <text x="144" y="142" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="3.5">privacy authority</text>

  <!-- Flower Hub -->
  <rect x="372" y="42" width="205" height="176" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <text x="474" y="72" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6" font-weight="600">Flower Hub</text>
  <text x="474" y="89" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="3.5">signed apps</text>

  <rect x="388" y="98" width="170" height="24" rx="5" fill="rgba(102,221,170,0.14)" stroke="rgba(102,221,170,0.40)"/>
  <text x="403" y="114" fill="#e0d8d0" font-family="Roboto Mono" font-size="4">logreg</text>
  <circle cx="543" cy="110" r="4.5" fill="#66ddaa"/>
  <path d="M540.8,110 l1.5,1.6 l2.8,-3.2" stroke="#10221a" stroke-width="1.1" fill="none" stroke-linecap="round" stroke-linejoin="round"/>

  <rect x="388" y="126" width="170" height="24" rx="5" fill="rgba(102,221,170,0.14)" stroke="rgba(102,221,170,0.40)"/>
  <text x="403" y="142" fill="#e0d8d0" font-family="Roboto Mono" font-size="4">u-net</text>
  <circle cx="543" cy="138" r="4.5" fill="#66ddaa"/>
  <path d="M540.8,138 l1.5,1.6 l2.8,-3.2" stroke="#10221a" stroke-width="1.1" fill="none" stroke-linecap="round" stroke-linejoin="round"/>

  <rect x="388" y="154" width="170" height="24" rx="5" fill="rgba(102,221,170,0.14)" stroke="rgba(102,221,170,0.40)"/>
  <text x="403" y="170" fill="#e0d8d0" font-family="Roboto Mono" font-size="4">resnet</text>
  <circle cx="543" cy="166" r="4.5" fill="#66ddaa"/>
  <path d="M540.8,166 l1.5,1.6 l2.8,-3.2" stroke="#10221a" stroke-width="1.1" fill="none" stroke-linecap="round" stroke-linejoin="round"/>

  <text x="474" y="196" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="3.5">growing pool</text>

  <!-- Hospital node / SuperNode -->
  <rect x="698" y="58" width="204" height="118" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <rect x="792" y="72" width="16" height="16" rx="2" fill="none" stroke="#88ccff" stroke-width="1.6"/>
  <line x1="800" y1="75" x2="800" y2="85" stroke="#88ccff" stroke-width="1.5" stroke-linecap="round"/>
  <line x1="795" y1="80" x2="805" y2="80" stroke="#88ccff" stroke-width="1.5" stroke-linecap="round"/>
  <text x="800" y="116" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="5" font-weight="600">Hospital SuperNode</text>
  <text x="800" y="131" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="3.9">DataSHIELD server</text>
  <text x="800" y="142" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="3.5">verifies signature</text>
  <text x="800" y="190" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="3.8">&#10003; trusted &#8594; accept</text>
  <text x="800" y="206" text-anchor="middle" fill="#ff7878" font-family="Roboto Mono" font-size="3.8">&#10007; untrusted &#8594; reject</text>

  <!-- Analyst -->
  <rect x="372" y="315" width="205" height="85" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <circle cx="474" cy="333" r="5" fill="none" stroke="#88ccff" stroke-width="1.6"/>
  <path d="M465,347 a9,9 0 0 1 18,0" fill="none" stroke="#88ccff" stroke-width="1.6"/>
  <text x="474" y="372" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="5" font-weight="600">Analyst</text>
  <text x="474" y="386" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="3.8">picks the app to run</text>

  <!-- reviewer -> hub (signs) -->
  <path d="M252,120 L370,120" fill="none" stroke="#66ddaa" stroke-width="2.5" stroke-dasharray="9 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-15" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="311" y="110" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="3.5">reviews &amp; signs</text>

  <!-- hub -> supernode (delivers signed app) -->
  <path d="M579,120 L696,120" fill="none" stroke="#88ccff" stroke-width="2.5" stroke-dasharray="9 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-15" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="637" y="110" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="3.5">pulled app</text>

  <!-- analyst -> hub (browse / choose) -->
  <path d="M474,313 L474,220" fill="none" stroke="#FFD000" stroke-width="2.2" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="483" y="244" text-anchor="start" fill="#FFD000" font-family="Roboto Mono" font-size="3.5">browse / choose</text>

  <!-- analyst -> supernode (request to run) -->
  <path d="M575,322 L705,178" fill="none" stroke="#ffaacc" stroke-width="2.2" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="648" y="264" text-anchor="start" fill="#ffaacc" font-family="Roboto Mono" font-size="3.5">request to run</text>

</svg>
</div>

<div style="text-align:center; color:#b8b0a8; font-size:0.9em; margin-top:0.2em;">
The pool grows from many publishers, while each node runs only apps signed by reviewers it trusts.
</div>
