<h1 align="center">Get Lighting</h1>

<h3 align="center">Description</h3>

<div align="center">Provides lighting information in various ways to cover most of your stylisation needs.</div>

<h3 align="center">Ports</h3>

| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| Position WS | **Input** | Vector 3 | WorldSpacePosition | The position vector in world space. |
| Normal WS | **Input** | Vector 3 | WorldSpaceNormal |  The normal vector in world space. |
| Lightmap UV | **Input** | Vector 2 | MeshUV1 | The UV of the mesh used for the light maps (Usually UV1). |
| Range Multiplier | **Input** | Float | None | Multiply the intensity inside the range of [Other lights](#bookmark=id.83ssxkab8n2e) ( Default 1). |
| S\_ Size | **Input** | Float | None | The radius multiplier of the speculars. |
| S\_ Intensity | **Input** | Float | None | Opacity of the speculars. |
| S\_ Light Color Inf | **Input** | Float | None | How much the speculars color is multiplied by the light color. |
| S\_ View Inf | **Input** | Float | None | How much the view direction influences the direction of the speculars ( Default 0.5). |
| S\_ View Dir | **Input** | Vector 3 | WorldSpaceViewDirection | The view direction in world space. Used for the speculars. |
| S\_ Texture \[Optional\] | **Input** | Texture 2D | None | The texture (sprite sheet) used for the speculars ( the index is dictated by the lights parameters) |
| S\_ Tiles \[Optional\] | **Input** | Float | None | The tiles amount of the sprite sheet texture used for speculars. |
| Color Gradient \[Optional\] | **Input** | Gradient | None | A gradient used for the light / shadow banding. |
| Color Texture \[Optional\] | **Input** | Texture 2D | None | A texture gradient used for the light / shadow banding. (only the \[0x, 0.5y\] to \[1x, 0.5y\] values of the textures are currently used). |
| Speculars | **Output** | Vector 3 | None | The compilation of all the lights speculars. |
| Colors | **Output** | Vector 3 | None | The compilation of all the lights intensity and colors.(according to the chosen Light Sampling option) |
| Light Coverage | **Output** | Float | None | The compilation of all the light coverage, independent of light color and intensity. |

<h3 align="center">Options</h3>

| Name | Type | Choices | Description |
| :---- | :---- | :---- | :---- |
| Interpolation | Enum | Simple Radial | Changes how the light fades on the surface. **Simple:** the dot product,  **Radial:** distributed evenly on the normals curvature. Simple:                Radial: ![][image1]![][image2]![][image3]![][image4] |
| Range Attenuation | Enum | Physical Linear | How the light fades in the distance for [Other lights](#bookmark=id.83ssxkab8n2e). |
| Light Sampling | Enum | None Gradient Texture 2D | How the light fade value is used. **None:** as is (0-1 value). 
**Gradient:** uses it to sample a given gradient. **Texture 2D:** uses it to sample horizontally a given texture. |
| Specuar Mode | Enum | Point Texture 2D | The type of specular. **Point:** traditional. **Texture 2D:** Uses a sprite sheet to use a variety of artistic specular images. Per lights parameters are available on each light's settings.  ![][image5]![][image6] |

Other Lights: point lights and spot lights.
