## Verified Apps from the Flower Hub

Flower Hub adds cryptographic app verification. It is the same govern-by-trust principle DataSHIELD already uses for approved functions, now applied to entire federated apps.

<div style="display: flex; flex-direction: column; gap: 8px; margin-top: 1em;">

<div v-click style="background: rgba(102,221,170,0.10); border: 1px solid rgba(102,221,170,0.15); border-radius: 10px; padding: 0.5em 1.2em;">
  <div style="display: flex; align-items: baseline; gap: 14px;">
    <span style="font-family: 'Roboto Mono', monospace; color: #66ddaa; font-weight: 600; font-size: 1.05em;">1</span>
    <span style="color: #e0d8d0;">The analyst requests an app by name.</span>
  </div>
</div>

<div v-click style="background: rgba(102,221,170,0.10); border: 1px solid rgba(102,221,170,0.15); border-radius: 10px; padding: 0.5em 1.2em;">
  <div style="display: flex; align-items: baseline; gap: 14px;">
    <span style="font-family: 'Roboto Mono', monospace; color: #66ddaa; font-weight: 600; font-size: 1.05em;">2</span>
    <span style="color: #e0d8d0;">Each hospital SuperNode pulls the signed bundle from the Flower Hub.</span>
  </div>
</div>

<div v-click style="background: rgba(102,221,170,0.10); border: 1px solid rgba(102,221,170,0.15); border-radius: 10px; padding: 0.5em 1.2em;">
  <div style="display: flex; align-items: baseline; gap: 14px;">
    <span style="font-family: 'Roboto Mono', monospace; color: #66ddaa; font-weight: 600; font-size: 1.05em;">3</span>
    <span style="color: #e0d8d0;">It checks the signature against reviewers that hospital trusts: biomedical, DataSHIELD, and privacy-preservation authorities.</span>
  </div>
</div>

<div v-click style="background: rgba(102,221,170,0.10); border: 1px solid rgba(102,221,170,0.15); border-radius: 10px; padding: 0.5em 1.2em;">
  <div style="display: flex; align-items: baseline; gap: 14px;">
    <span style="font-family: 'Roboto Mono', monospace; color: #66ddaa; font-weight: 600; font-size: 1.05em;">4</span>
    <span style="color: #e0d8d0;">It runs only if a trusted reviewer signed that exact version. Unsigned or untrusted apps are blocked by default.</span>
  </div>
</div>

</div>

<div class="mt-5" v-click style="color: #b8b0a8; font-size: 0.92em;">
A signature means <strong style="color:#e0d8d0;">reviewed and trusted</strong>. Alignment with DataSHIELD disclosure controls and secure aggregation is what each reviewer checks before signing.
</div>
