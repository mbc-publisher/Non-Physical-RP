<h1 align="center">Get Lighting</h1>

<h3 align="center">Description</h3>

<div align="center">Provides lighting information in various ways to cover most of your stylisation needs.</div>

<h3 align="center">Ports</h3>

| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| Position WS | **Input** | Vector 3 | WorldSpacePosition | The position vector in world space. |
| Normal WS | **Input** | Vector 3 | WorldSpaceNormal |  The normal vector in world space. |
| Lightmap UV | **Input** | Vector 2 | MeshUV1 | The UV of the mesh used for the light maps (Usually UV1). |
| Range Multiplier | **Input** | Float | None | Multiply the intensity inside the range of *Other lights ( Default 1). |
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

<div align="center">
  
| Name | Type | Choices | Description |
| :---- | :---- | :---- | :---- |
| Interpolation | Enum | •Simple<br> •Radial | Changes how the light fades on the surface.<br> **Simple:** the dot product,<br>  **Radial:** distributed evenly on the normals curvature.<br> Simple:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Radial:<br> <img width="128" height="128" alt="image7" src="https://github.com/user-attachments/assets/591cbf36-065f-449f-b80d-d5dde6eb8dcc" /> <img width="128" height="128" alt="image4" src="https://github.com/user-attachments/assets/a7106edc-e7fc-4ecb-847a-c2d6ece1cf49" /><br> <img width="128" height="128" alt="image1" src="https://github.com/user-attachments/assets/9f9bc907-7cc2-4021-9cb4-a439cc89b4ff" /> <img width="128" height="128" alt="image9" src="https://github.com/user-attachments/assets/167c88eb-02f2-4109-8231-e6201bbbb194" />|
| Range Attenuation | Enum | •Physical<br> •Linear | How the light fades in the distance for *Other lights. |
| Light Sampling | Enum | •None<br> •Gradient<br> •Texture 2D | How the light fade value is used.<br> **None:** as is (0-1 value).<br> **Gradient:** uses it to sample a given gradient.<br> **Texture 2D:** uses it to sample horizontally a given texture. |
| Specuar Mode | Enum | •Point<br> •Texture 2D | The type of specular.<br><br> **Point:** traditional.<br><img width="128" height="128" alt="image10" src="https://github.com/user-attachments/assets/9538236e-70c1-4402-97f9-11c3839a7c6b" /><br><br> **Texture 2D:** Uses a sprite sheet to use a variety of artistic specular images.<br><img width="128" height="128" alt="image5" src="https://github.com/user-attachments/assets/89b6bda0-4a01-4ed8-b361-82741d729aee" /><br><br> Per lights parameters are available on each light's settings.|

</div>

*Other lights: Point lights and spot lights.
