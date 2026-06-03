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

A chest CT is a **512 &times; 512 &times; N** volume, far too large and too sensitive to move. dsFlower ships three vision templates for medical imaging, each validated on real medical images.

<div class="mt-3" v-click>

<div class="grid grid-cols-1 gap-2">
  <div class="step-card" style="padding: 0.55em 0.9em;"><strong>ResNet-18</strong> <span style="color:#FFD000;">&middot; image classification</span></div>
  <div class="step-card" style="padding: 0.55em 0.9em;"><strong>DenseNet-121</strong> <span style="color:#FFD000;">&middot; image classification</span></div>
  <div class="step-card" style="padding: 0.55em 0.9em;"><strong>U-Net 2D</strong> <span style="color:#FFD000;">&middot; segmentation</span></div>
</div>

</div>

<div class="mt-3" v-click>

Training runs inside each hospital. Only model updates leave; the images never do.

</div>

</div>
</div>
