<h1 align="center">Geometry</h1>

<h3 align="center">Description</h3>

<div align="center">Render Meshes and skeletal meshes based on chosen parameters.</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| MRT Sets | Array / List | Any declared MRT Set in the Render Stack. | Will render the geometry once for each set of multiple render targets (MRT). |
| To Copy | Array / List | Any Render Target identified as copyable. | Will copy the content of those render targets to a copy buffer after the rendering of geometry. The copies will then be available to use for the next render passes. |
| Layer mask | Enum | •Nothing<br> •Everything<br> •Default<br> •TransparentFX<br> •Ignore Raycast<br> •Water<br> •UI<br> •Any User defined<br> | Will render only the geometry corresponding to the selected layer masks. (Multiple choice Enum  (Bit Masking)). |
| Render queue | Enum | Opaque<br> Transparent<br> All<br> | Will render only the geometry whose material is of the selected render queue. |
| Sorting Criteria | Enum | •Nothing<br> •Everything<br> •Sorting Layer<br> •Render Queue<br> •Back To Front<br> •Quantized Front To Back<br> •Optimized State Changes<br> •Canva Order<br> •Render Priority<br> •Common Opaque<br> •Common Transparent<br> | Specify the order of rendering based on chosen criteria. (Multiple choice Enum  (Bit Masking)). **Tips:** To use Common Opaque or Common Transparent, First clear your selection using None. These two are multiselection presets but they do not remove the ones that should not be selected. |
