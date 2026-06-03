## dsFlower's Approach

<div style="margin-top: 0.2em;">
<svg viewBox="0 0 920 400" style="width: 100%; max-height: 340px;">

  <!-- Trusted reviewer -->
  <rect x="20" y="50" width="215" height="115" rx="14" fill="rgba(102,221,170,0.10)" stroke="rgba(102,221,170,0.30)" stroke-width="1.5"/>
  <circle cx="123" cy="72" r="7" fill="none" stroke="#66ddaa" stroke-width="1.6"/>
  <line x1="128" y1="77" x2="134" y2="83" stroke="#66ddaa" stroke-width="1.8" stroke-linecap="round"/>
  <text x="127" y="106" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="6" font-weight="600">Trusted reviewer</text>
  <text x="127" y="122" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4">biomedical / DataSHIELD</text>
  <text x="127" y="134" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="4">privacy authority</text>

  <!-- Flower Hub -->
  <rect x="360" y="40" width="200" height="165" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <text x="460" y="72" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="7" font-weight="600">Flower Hub</text>
  <rect x="375" y="92" width="170" height="30" rx="6" fill="rgba(212,160,23,0.16)" stroke="rgba(212,160,23,0.5)" stroke-width="1.2"/>
  <circle cx="393" cy="107" r="6" fill="#d4a017"/>
  <path d="M390.2,107 l1.8,1.9 l3.3,-3.7" stroke="#1a1206" stroke-width="1.3" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
  <text x="407" y="110" fill="#e0d8d0" font-family="Roboto Mono" font-size="5">@app v1.2.0</text>
  <rect x="375" y="128" width="170" height="28" rx="6" fill="rgba(102,221,170,0.16)" stroke="rgba(102,221,170,0.45)" stroke-width="1.2"/>
  <path d="M389,142 h10 M389,146 h7" stroke="#66ddaa" stroke-width="1.4" stroke-linecap="round"/>
  <text x="407" y="146" fill="#e0d8d0" font-family="Roboto Mono" font-size="5">signatures</text>
  <text x="460" y="182" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="4">signed bundle + signatures</text>

  <!-- Hospital node / SuperNode -->
  <rect x="700" y="50" width="215" height="115" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <rect x="799" y="62" width="16" height="16" rx="2" fill="none" stroke="#88ccff" stroke-width="1.5"/>
  <line x1="807" y1="65" x2="807" y2="75" stroke="#88ccff" stroke-width="1.4" stroke-linecap="round"/>
  <line x1="802" y1="70" x2="812" y2="70" stroke="#88ccff" stroke-width="1.4" stroke-linecap="round"/>
  <text x="807" y="106" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="5.6" font-weight="600">Hospital SuperNode</text>
  <text x="807" y="122" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4">DataSHIELD server</text>
  <text x="807" y="134" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="4">verifies signature</text>
  <text x="807" y="186" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="4.4">&#10003; trusted &#8594; accept</text>
  <text x="807" y="199" text-anchor="middle" fill="#ff7878" font-family="Roboto Mono" font-size="4.4">&#10007; untrusted &#8594; reject</text>

  <!-- Analyst -->
  <rect x="355" y="300" width="210" height="90" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <circle cx="460" cy="320" r="5" fill="none" stroke="#88ccff" stroke-width="1.5"/>
  <path d="M451,334 a9,9 0 0 1 18,0" fill="none" stroke="#88ccff" stroke-width="1.5"/>
  <text x="460" y="358" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6" font-weight="600">Analyst</text>
  <text x="460" y="374" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4">picks the app to run</text>

  <!-- reviewer -> hub (signs) -->
  <path d="M235,108 L358,108" fill="none" stroke="#66ddaa" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="296" y="101" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="3.8">reviews &amp; signs</text>

  <!-- hub -> supernode (delivers signed app) -->
  <path d="M562,108 L698,108" fill="none" stroke="#88ccff" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="630" y="101" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="3.8">signed app + sigs</text>

  <!-- analyst -> hub (browse / choose) -->
  <path d="M460,298 L460,209" fill="none" stroke="#FFD000" stroke-width="2.2" stroke-dasharray="7 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-13" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="468" y="256" text-anchor="start" fill="#FFD000" font-family="Roboto Mono" font-size="3.8">browse / choose</text>

  <!-- analyst -> supernode (request to run) -->
  <path d="M555,300 L704,168" fill="none" stroke="#ffaacc" stroke-width="2.2" stroke-dasharray="7 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-13" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="560" y="292" text-anchor="start" fill="#ffaacc" font-family="Roboto Mono" font-size="3.8">request to run</text>

</svg>
</div>

The pool grows from many publishers. Each hospital still runs only apps signed by reviewers it trusts, the same govern-by-trust principle as DataSHIELD's approved functions.
