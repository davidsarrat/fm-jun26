## dsFlower's Approach

<div style="margin-top: 0.2em;">
<svg viewBox="0 0 820 340" style="width: 100%; max-height: 320px;">

  <!-- Trusted reviewer -->
  <rect x="30" y="60" width="180" height="92" rx="14" fill="rgba(102,221,170,0.10)" stroke="rgba(102,221,170,0.30)" stroke-width="1.5"/>
  <text x="120" y="86" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="6.5" font-weight="600">Trusted reviewer</text>
  <text x="120" y="106" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.6">biomedical &middot; DataSHIELD</text>
  <text x="120" y="120" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.6">privacy authority</text>
  <text x="120" y="138" text-anchor="middle" fill="#b0b8c0" font-family="Roboto Mono" font-size="4">reviews &amp; signs apps</text>

  <!-- Flower Hub -->
  <rect x="330" y="50" width="170" height="112" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <text x="415" y="74" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6.5" font-weight="600">Flower Hub</text>
  <rect x="345" y="86" width="140" height="22" rx="5" fill="rgba(102,221,170,0.10)" stroke="rgba(102,221,170,0.25)"/>
  <text x="356" y="101" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.6">signed app</text>
  <circle cx="470" cy="97" r="5.5" fill="#66ddaa"/>
  <path d="M467.4,97 l1.8,1.9 l3.3,-3.7" stroke="#10221a" stroke-width="1.3" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
  <rect x="345" y="116" width="140" height="22" rx="5" fill="rgba(102,221,170,0.10)" stroke="rgba(102,221,170,0.25)"/>
  <text x="356" y="131" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.6">signed app</text>
  <circle cx="470" cy="127" r="5.5" fill="#66ddaa"/>
  <path d="M467.4,127 l1.8,1.9 l3.3,-3.7" stroke="#10221a" stroke-width="1.3" fill="none" stroke-linecap="round" stroke-linejoin="round"/>

  <!-- Hospital SuperNode -->
  <rect x="620" y="60" width="180" height="92" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <text x="710" y="86" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6" font-weight="600">Hospital SuperNode</text>
  <text x="710" y="106" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.6">verifies signature against</text>
  <text x="710" y="120" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.6">its trusted reviewers</text>

  <!-- reviewer -> hub -->
  <path d="M212,106 L328,106" fill="none" stroke="#66ddaa" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="270" y="99" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="4">signs</text>

  <!-- hub -> supernode -->
  <path d="M502,106 L618,106" fill="none" stroke="#88ccff" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="560" y="99" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="4">pull signed app</text>

  <!-- analyst -->
  <rect x="330" y="250" width="170" height="66" rx="14" fill="rgba(136,204,255,0.08)" stroke="rgba(136,204,255,0.22)" stroke-width="1.5"/>
  <text x="415" y="276" text-anchor="middle" fill="#88ccff" font-family="Roboto Mono" font-size="6" font-weight="600">Analyst</text>
  <text x="415" y="294" text-anchor="middle" fill="#e0d8d0" font-family="Roboto Mono" font-size="4.6">requests an app by name</text>

  <!-- analyst -> hub -->
  <path d="M415,248 L415,164" fill="none" stroke="#ffaacc" stroke-width="2.5" stroke-dasharray="8 6">
    <animate attributeName="stroke-dashoffset" from="0" to="-14" dur="0.8s" repeatCount="indefinite"/>
  </path>
  <text x="424" y="208" text-anchor="start" fill="#ffaacc" font-family="Roboto Mono" font-size="4">request</text>

  <!-- outcomes under supernode -->
  <text x="710" y="178" text-anchor="middle" fill="#66ddaa" font-family="Roboto Mono" font-size="4.4">&#10003; trusted signature &#8594; runs</text>
  <text x="710" y="192" text-anchor="middle" fill="#ff7878" font-family="Roboto Mono" font-size="4.4">&#10007; unsigned / untrusted &#8594; blocked</text>

</svg>
</div>

The pool grows from many publishers. Each hospital still runs only apps signed by reviewers it trusts, the same govern-by-trust principle as DataSHIELD's approved functions.
