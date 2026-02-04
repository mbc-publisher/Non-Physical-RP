<h1 align="center">Bloom</h1>

<h3 align="center">Description</h3>

<div align="center">Emulate the glowing effect of lights or high luminosity points.</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Intensity | Float | Range 0 \- ∞ | The intensity of the blooming effect. |
| Threshold | Float | Range 0 \- ∞ | Limits the bloom to pixels whose values are above the threshold. |
| Threshold Knee | Float | Range 0 \- 1 | Control the smoothness of the transition for values close to the threshold. |
| Max Iterations | Int | Range 0 \- 16 | The maximum amount of bloom passes. (higher is more expensive). |
| Upsampling | Enum | •Billinear<br> •Bicubic<br> | The sampling method used when Compiling the render textures. |
| Scatter | Float | Range 0.5 \- 0.95 | How much light will scatter. |
| Ignore Render Scale | Boolean |  | If true, use the window resolution. If false, use the render target resolution. |

<h3 align="center">More Settings</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Main Color | Enum | Any Non-Depth Render Target | You can choose to override which color render target will be used for this pass. |
| Main Depth | Enum | Any Depth Render Target | You can choose to override which depth render target will be used for this pass. |
