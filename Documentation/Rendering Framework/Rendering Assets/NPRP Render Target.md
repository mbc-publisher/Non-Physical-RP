<h3 align="center">### NPRP Render Target {#nprp-render-target}</h3>

<h3 align="center">**Description**</h3>

<h3 align="center">Render texture wrapper. Describes a render target that can be shared across the render passes. 2 render targets (main color and main depth) are mandatory and can’t be deleted. These 2 stay active until the end of the frame. Any other user defined render targets will be cleared and discarded as soon as the last render pass using them is over. If you need to delay the discarding of a render target to use it in a pass where it's not specifically assigned ( Screen Material pass for exemple), you can do so using a clear pass after.</h3>

<h3 align="center">**Parameters**</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Format | Enum | • ARGB32<br> • Depth<br> • ARGBHalf<br> • Shadowmap<br>  • RGB565<br>  • ARGB4444<br>  • ARGB1555<br>  • Default<br>  • ARGB2101010<br>  • DefaultHDR<br>  • ARGB64<br>  • ARGBFloat<br>  • RGFloat<br>  • RGHalf<br>  
• RFloat<br>  • RHalf<br>  • R8<br>  • ARGBInt<br>  • RGInt<br>  RInt<br>  • BGRA32<br>  • RGB111110Float<br>  • RG32<br> • RGBAUShort<br> • RG16<br> • BGRA10101010\_XR<br> • BGR101010\_XR<br> • R16<br> | See Unity’s [Documentation on Render Texture Formats](https://docs.unity3d.com/6000.2/Documentation/ScriptReference/RenderTextureFormat.html) |
| Filtering | Enum | • Point<br> • Billinear<br> • Trilinear<br> | **Point:** Texture pixels become blocky up close. **Bilinear:** Texture samples are averaged. **Trilinear:** Texture samples are averaged and also blended between mipmap levels. |
| Color Space | Enum | • Default<br> • Linear<br> • SRGB<br> | **Default:** color space conversion based on project settings. **Linear:** Render texture contains linear (non-color) data; don't perform color conversions on it. **sRGB:** Render texture contains sRGB (color) data, perform Linear\<-\>sRGB conversions. |
| Assigned RT | Enum | • UNDEFINED<br> • Color<br> • Albedo<br> • Normal<br> • Depth<br> • DepthNormal<br> • Specular<br> • Emissive<br> • LineData1<br> • LineData2<br> • RT\_00<br> • RT\_01<br> • RT\_02<br> • RT\_03<br> • RT\_04<br> • RT\_05<br> • RT\_06<br> • RT\_07<br> | If not UNDEFINED, maps this render target to its correspondence in Shader Graph. |
| To Copy | Boolean |  | Marks this render target as copyable. If so, the copy is the one accessible in Shader Graph via the Get Render texture node. |
| Copy Scale | Float | Range 0.01 \- 1 | The relative size of the Copy. |
| Clear Mode | Enum | • White<br> • Black<br> • Clear<br> • Camera<br> • Custom<br> | The color mode applied when cleared. (Non-Depth render target). |
| Clear Value | Float |  | The value applied when cleared. (Depth render target). |
| Clear Color | Color |  | The custom color applied when cleared when Clear Mode is set to Custom. (Non-Depth render target) |
