### NPRP Render Target {#nprp-render-target}

**Description**

Render texture wrapper. Describes a render target that can be shared across the render passes. 2 render targets (main color and main depth) are mandatory and can’t be deleted. These 2 stay active until the end of the frame. Any other user defined render targets will be cleared and discarded as soon as the last render pass using them is over. If you need to delay the discarding of a render target to use it in a pass where it's not specifically assigned ( Screen Material pass for exemple), you can do so using a clear pass after.

**Parameters**

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Format | Enum | ARGB32 Depth  ARGBHalf Shadowmap  RGB565  ARGB4444  ARGB1555  Default  ARGB2101010  DefaultHDR  ARGB64  ARGBFloat  RGFloat  RGHalf  RFloat  RHalf  R8  ARGBInt  RGInt  RInt  BGRA32  RGB111110Float  RG32 RGBAUShort RG16 BGRA10101010\_XR BGR101010\_XR R16 | See Unity’s [Documentation on Render Texture Formats](https://docs.unity3d.com/6000.2/Documentation/ScriptReference/RenderTextureFormat.html) |
| Filtering | Enum | Point Billinear Trilinear | **Point:** Texture pixels become blocky up close. **Bilinear:** Texture samples are averaged. **Trilinear:** Texture samples are averaged and also blended between mipmap levels. |
| Color Space | Enum | Default Linear SRGB | **Default:** color space conversion based on project settings. **Linear:** Render texture contains linear (non-color) data; don't perform color conversions on it. **sRGB:** Render texture contains sRGB (color) data, perform Linear\<-\>sRGB conversions. |
| Assigned RT | Enum | UNDEFINED Color Albedo Normal Depth DepthNormal Specular Emissive LineData1 LineData2 RT\_00 RT\_01 RT\_02 RT\_03 RT\_04 RT\_05 RT\_06 RT\_07 | If not UNDEFINED, maps this render target to its correspondence in Shader Graph. |
| To Copy | Boolean |  | Marks this render target as copyable. If so, the copy is the one accessible in Shader Graph via the Get Render texture node. |
| Copy Scale | Float | Range 0.01 \- 1 | The relative size of the Copy. |
| Clear Mode | Enum | White Black Clear Camera Custom | The color mode applied when cleared. (Non-Depth render target). |
| Clear Value | Float |  | The value applied when cleared. (Depth render target). |
| Clear Color | Color |  | The custom color applied when cleared when Clear Mode is set to Custom. (Non-Depth render target) |


