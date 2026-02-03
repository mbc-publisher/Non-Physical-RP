<h3 align="center">NP Render Pipeline Asset</h3>

<h3 align="center">Description</h3>
<h3 align="center">NPRP’s Render pipeline asset. Must be set in the project's settings to take effect,
as any Unity Render Pipeline Asset.
</h3>

**Parameters**

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Render Scale | <span style="background:#1e40af;color:#bfdbfe;padding:2px 8px;border-radius:6px;font-size:0.85em;">Float</span> | Range 0.1 - 2 | The ratio of the rendering size vs the actual resolution. (1 is the same size, 2 is twice, 0.1 is 1/10). |
| Bicubic Rescaling | <span style="background:#6b21a8;color:#e9d5ff;padding:2px 8px;border-radius:6px;font-size:0.85em;">Enum</span> | Off · Up Only · Up And Down | Whether the bicubic filtering is used at all, only when scaling up, or when scaling up and down. |
| Type (Anti Aliasing) | <span style="background:#6b21a8;color:#e9d5ff;padding:2px 8px;border-radius:6px;font-size:0.85em;">Enum</span> | None · FXAA | The type of Antialiasing. None or FXAA (only option for now). |
| Quality (Anti Aliasing) | <span style="background:#6b21a8;color:#e9d5ff;padding:2px 8px;border-radius:6px;font-size:0.85em;">Enum</span> | Low · Medium · High | The quality of the anti-aliasing. |
| Fixed Threshold (Anti Aliasing) | <span style="background:#1e40af;color:#bfdbfe;padding:2px 8px;border-radius:6px;font-size:0.85em;">Float</span> | Range 0.0312 - 0.0833 | Sets a baseline brightness difference needed for FXAA to consider something an edge. |
| Relative Threshold (Anti Aliasing) | <span style="background:#1e40af;color:#bfdbfe;padding:2px 8px;border-radius:6px;font-size:0.85em;">Float</span> | Range 0.063 - 0.333 | Defines how big the local contrast must be relative to surrounding brightness before FXAA treats it as an edge. |
| Subpixel Blending (Anti Aliasing) | <span style="background:#1e40af;color:#bfdbfe;padding:2px 8px;border-radius:6px;font-size:0.85em;">Float</span> | Range 0 - 1 | Controls how strongly FXAA applies its sub-pixel anti-aliasing pass. |
| Enabled (Lighting) | <span style="background:#065f46;color:#bbf7d0;padding:2px 8px;border-radius:6px;font-size:0.85em;">Boolean</span> |  | Enable or disable lighting. |
| Max Dir Lights (Lighting) | <span style="background:#1e40af;color:#bfdbfe;padding:2px 8px;border-radius:6px;font-size:0.85em;">Float</span> | Range 0 - 8 | Maximum directional lights (does not dictate shadows). |
| Max Other Lights (Lighting) | <span style="background:#1e40af;color:#bfdbfe;padding:2px 8px;border-radius:6px;font-size:0.85em;">Float</span> | Range 0 - 64 | Maximum other lights (does not dictate shadows). |
| Render Stack | <span style="background:#6b21a8;color:#e9d5ff;padding:2px 8px;border-radius:6px;font-size:0.85em;">Enum</span> | Any available render stack | Choose a render stack to control order and passes of rendering. |
| LOD Fade Animation Duration | <span style="background:#1e40af;color:#bfdbfe;padding:2px 8px;border-radius:6px;font-size:0.85em;">Float</span> | Range 0 - 10 | How long it takes to gradually switch between LODs. |
| Use SRP Batcher | <span style="background:#065f46;color:#bbf7d0;padding:2px 8px;border-radius:6px;font-size:0.85em;">Boolean</span> |  | – |
| Use Dynamic Batching | <span style="background:#065f46;color:#bbf7d0;padding:2px 8px;border-radius:6px;font-size:0.85em;">Boolean</span> |  | – |
| Use Instancing | <span style="background:#065f46;color:#bbf7d0;padding:2px 8px;border-radius:6px;font-size:0.85em;">Boolean</span> |  | – |
| Use Lights Per Objects | <span style="background:#065f46;color:#bbf7d0;padding:2px 8px;border-radius:6px;font-size:0.85em;">Boolean</span> |  | – |
| Enable HDR | <span style="background:#065f46;color:#bbf7d0;padding:2px 8px;border-radius:6px;font-size:0.85em;">Boolean</span> |  | Lets you use HDR textures for rendering. |
| Default Shader | <span style="background:#92400e;color:#fde68a;padding:2px 8px;border-radius:6px;font-size:0.85em;">Shader</span> |  | The shader used when a new material is created. |
| Default Material | <span style="background:#92400e;color:#fde68a;padding:2px 8px;border-radius:6px;font-size:0.85em;">Material</span> |  | The material used on newly created objects. |
