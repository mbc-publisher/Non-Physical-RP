<h1 align="center">Shadow Casting</h1>

<h3 align="center">Description</h3>

<div align="center">Creates Shadow maps for eligible shadow casting lights.</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Max distance | Float | Range 0 \- ∞ | The maximum distance from the camera to render shadows. |
| Directionals Shadowmap Size | Enum | •256<br> •512<br> •1024<br> •2048<br> •4096<br> •8192<br> •16384<br> | The quality of the shadow map for each directional light. |
| Others Shadowmap Size | Enum | •256<br> •512<br> •1024<br> •2048<br> •4096<br> •8192<br> •16384<br> | The quality of the shadow map for 16 spot lights or . |
| Cascade Count | Int | Range 1 \- 4 | The number of shadow cascades for directional shadows. |
| Cascade 1 | Float | Range 0 \- 1 | The range covered by the cascade between the camera's near plane and the closest between the camera's far plane or the Shadows max distance. |
| Cascade 2 | Float | Range Cascade 1 \- 1 | The range covered by the cascade between the camera's near plane and the closest between the camera's far plane or the Shadows max distance. |
| Cascade 3 | Float | Range Cascade 2 \- 1 | The range covered by the cascade between the camera's near plane and the closest between the camera's far plane or the Shadows max distance. |
| Cascade Fade | Float | Range 0 \- 1 | The fade factor between cascade 4 and the end of the shadowmap range. |
| Directionals Softness Filter | Enum | •None<br> •PCF<br> •3x3<br> •PCF<br> •5x5<br> •PCF<br> •7x7<br> | The blur filter applied to the shadows of directional lights. |
| Others Softness Filter | Enum | •None<br> •PCF<br> •3x3<br> •PCF<br> •5x5<br> •PCF<br> •7x7<br> | The blur filter applied to the shadows of other lights. |
| Blending Mode | Enum | •Hard<br> •Soft<br> •Dither<br> | The blending mode between each shadow cascades. |
