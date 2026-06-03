## dsFlower's Approach

<div style="margin-top: 0.2em;">
<svg viewBox="0 0 800 380" style="width: 100%; max-height: 330px;">

  <!-- Trusted reviewer -->
  <rect x="20" y="45" width="185" height="105" rx="14" fill="rgba(102,221,170,0.10)" stroke="rgba(102,221,170,0.30)" stroke-width="1.5"/>
  <circle cx="108" cy="70" r="7" fill="none" stroke="#66ddaa" stroke-width="1.6"/>
  <line x1="113" y1="75" x2="119" y2="81" stroke="#66ddaa" stroke-width="1.8" stroke-linecap="round"/>
  <text x="112" y="104" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="7" font-weight="600">Trusted reviewer</text>
  <text x="112" y="120" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.3">biomedical / DataSHIELD</text>
  <text x="112" y="133" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="4.3">privacy authority</text>

  <!-- Flower Hub -->
  <rect x="300" y="35" width="200" height="150" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <text x="400" y="68" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="8" font-weight="600">Flower Hub</text>
  <rect x="320" y="88" width="160" height="30" rx="6" fill="rgba(212,160,23,0.16)" stroke="rgba(212,160,23,0.5)" stroke-width="1.2"/>
  <circle cx="338" cy="103" r="6" fill="#d4a017"/>
  <path d="M335.2,103 l1.8,1.9 l3.3,-3.7" stroke="#1a1206" stroke-width="1.3" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
  <text x="352" y="106" fill="#e0d8d0" font-family="Roboto Mono" font-size="5">@app v1.2.0</text>
  <rect x="320" y="124" width="160" height="28" rx="6" fill="rgba(102,221,170,0.16)" stroke="rgba(102,221,170,0.45)" stroke-width="1.2"/>
  <path d="M334,138 h10 M334,142 h7" stroke="#66ddaa" stroke-width="1.4" stroke-linecap="round"/>
  <text x="352" y="142" fill="#e0d8d0" font-family="Roboto Mono" font-size="5">signatures</text>
  <text x="400" y="172" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="4">signed app bundle + signatures</text>

  <!-- Hospital SuperNode -->
  <rect x="595" y="45" width="185" height="105" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <rect x="679" y="60" width="16" height="16" rx="2" fill="none" stroke="#88ccff" stroke-width="1.5"/>
  <line x1="687" y1="63" x2="687" y2="73" stroke="#88ccff" stroke-width="1.4" stroke-linecap="round"/>
  <line x1="682" y1="68" x2="692" y2="68" stroke="#88ccff" stroke-width="1.4" stroke-linecap="round"/>
  <text x="687" y="104" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6.2" font-weight="600">Hospital SuperNode</text>
  <text x="687" y="120" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.3">verifies signature</text>
  <text x="687" y="133" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="4.3">vs its trusted reviewers</text>
  <text x="687" y="166" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="4.8">&#10003; trusted &#8594; accept</text>
  <text x="687" y="180" text-anchor="middle" fill="#ff7878" font-family="Roboto Mono" font-size="4.8">&#10007; untrusted &#8594; reject</text>

  <!-- Analyst -->
  <rect x="300" y="255" width="200" height="85" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <circle cx="400" cy="272" r="5" fill="none" stroke="#88ccff" stroke-width="1.5"/>
  <path d="M391,286 a9,9 0 0 1 18,0" fill="none" stroke="#88ccff" stroke-width="1.5"/>
  <text x="400" y="312" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6.5" font-weight="600">Analyst</text>
  <text x="400" y="328" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.4">requests an app by name</text>

  <!-- reviewer -> hub -->
  <path d="M207,95 L298,95" fill="none" stroke="#66ddaa" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="252" y="88" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="4">reviews &amp; signs</text>

  <!-- hub -> supernode -->
  <path d="M502,95 L593,95" fill="none" stroke="#88ccff" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="547" y="88" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="4">pull signed app</text>

  <!-- analyst -> hub -->
  <path d="M400,253 L400,187" fill="none" stroke="#ffaacc" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="409" y="222" text-anchor="start" fill="#ffaacc" font-family="Roboto Mono" font-size="4">request</text>

</svg>
</div>

The pool grows from many publishers. Each hospital still runs only apps signed by reviewers it trusts, the same govern-by-trust principle as DataSHIELD's approved functions.
