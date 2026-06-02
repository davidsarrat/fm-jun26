## What we're working with

<div class="grid grid-cols-2 gap-8 mt-2 items-center">
<div class="flex flex-col items-center gap-3">

<div class="flex gap-3">
  <img src="/ct-lung-1.png" style="width: 200px; border-radius: 10px; border: 1px solid rgba(255,255,255,0.12);" />
  <img src="/ct-lung-2.png" style="width: 200px; border-radius: 10px; border: 1px solid rgba(255,255,255,0.12);" />
</div>

<span style="font-family: 'Roboto Mono', monospace; font-size: 0.62em; color: #8a7d70;">Axial chest CT, lung window &middot; MosMedData (CC BY-NC-SA 4.0)</span>

</div>
<div>

Real medical images, not summary tables. A single chest CT is a **512 &times; 512 &times; N** volume that never leaves the hospital.

<div class="mt-3" v-click>

**Two paths, both federated:**

</div>

<div v-click>

- **Radiomics** &mdash; the server turns each scan into a feature table, then trains on those features
- **Direct image** &mdash; the model itself travels to the hospital and trains on the raw pixels

</div>

<div class="mt-3" v-click>

The hospital keeps the pixels. Only model updates come back.

</div>

</div>
</div>
