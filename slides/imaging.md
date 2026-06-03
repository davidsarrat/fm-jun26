## Vision

<div class="grid grid-cols-2 gap-8 mt-2 items-center">
<div class="flex flex-col items-center gap-3">

<div class="flex gap-3">
  <img src="/ct-lung-1.png" style="width: 200px; border-radius: 10px; border: 1px solid rgba(255,255,255,0.12);" />
  <img src="/ct-lung-2.png" style="width: 200px; border-radius: 10px; border: 1px solid rgba(255,255,255,0.12);" />
</div>

<span style="font-family: 'Roboto Mono', monospace; font-size: 0.62em; color: #ffffff;">Axial chest CT, lung window &middot; MosMedData (CC BY-NC-SA 4.0)</span>

</div>
<div>

These are the actual scans dsFlower trains on. A chest CT is a **512 &times; 512 &times; N** volume, and it never leaves the hospital.

<div class="mt-3" v-click>

**Three vision templates ship ready to run:**

<div class="grid grid-cols-1 gap-2 mt-2">
  <div class="step-card" style="padding: 0.55em 0.9em;"><strong>ResNet-18</strong> <span style="color:#FFD000;">&middot; image classification</span></div>
  <div class="step-card" style="padding: 0.55em 0.9em;"><strong>DenseNet-121</strong> <span style="color:#FFD000;">&middot; image classification</span></div>
  <div class="step-card" style="padding: 0.55em 0.9em;"><strong>U-Net 2D</strong> <span style="color:#FFD000;">&middot; segmentation</span></div>
</div>

</div>

<div class="mt-3" v-click>

The model travels to the hospital and trains on the raw pixels. Only updates come back.

</div>

<div class="mt-2" v-click style="font-size: 0.85em; color: #66ddaa;">

All three validated on real medical images.

</div>

</div>
</div>
