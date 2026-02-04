<h1 align="center">NP Render Pipeline Asset</h1>

<h3 align="center">Description</h3>
<div align="center">NPRP’s Render pipeline asset. Must be set in the project's settings to take effect,
as any Unity Render Pipeline Asset.
</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Render Scale | Float | Range 0.1 \- 2 | The ratio of the rendering size vs the actual resolution. (1 is the same size, 2 is twice and 0.1 is 1/10). |
| Bicubic Rescaling | Enum | •Off<br> •Up Only<br> •Up And Down<br> | Whether the bicubic filtering is used at all, only when scaling back up or when scaling un and down. |
| Type (Anti Aliasing) | Enum | •None<br> •FXAA<br> | The Type of Antialiasing. None or FXAA (only option for now) |
| Quality  (Anti Aliasing) | Enum | •Low<br> •Medium<br> •High<br> | The quality of the anti aliasing. |
| Fixed Threshold (Anti Aliasing) | Float | Range 0.0312 \- 0.0833 | Sets a baseline brightness difference needed for FXAA to consider something an edge. |
| Relative Threshold (Anti Aliasing) | Float | Range 0.063 \- 0.333 | Defines how big the local contrast must be, relative to surrounding brightness, before FXAA treats it as an edge. |
| Subpixel Blending (Anti Aliasing) | Float | Range 0 \- 1 | Controls how strongly FXAA applies its sub-pixel anti-aliasing pass, which smooths shimmering and fine detail aliasing. |
| Enabled (Lighting) | Boolean |  | Enable or disable the lighting. |
| Max Dir Lights (Lighting) | Float | Range 0 \- 8 | The maximum amount of directional lights. Does not directly dictate the maximum or directional shadows. |
| Max Other Lights (Lighting) | Float | Range 0 \- 64 | The maximum amount of other lights. Does not directly dictate the maximum or other shadows. |
| Render Stack | Enum | Any available Render Stack in your project. | Choose a render stack in your project that will control the order and passes of rendering. |
| LOD Fade Animation Duration | Float | Range 0 \- 10 | How long it takes to gradually switch between LODs. |
| Use SRP Batcher | Boolean |  | – |
| Use Dynamic Batching | Boolean |  | – |
| Use Instancing | Boolean |  | – |
| Use Lights Per Objects | Boolean |  | – |
| Enable HDR | Boolean |  | Lets you use HDR textures for rendering. |
| Default Shader | Shader |  | The shader that is used when a new material is created. |
| Default Material | Material |  | The material used on newly created objects. |
