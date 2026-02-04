<h1 align="center">Get Render Texture</h1>

<h3 align="center">Description</h3>

<div align="center">Return an NPRP render texture. The render texture must have been written to previously and be kept active as long as you intend to use it.</div>

<h3 align="center">Ports</h3>

<div align="center">

| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| UV | **Input** | Vector 2 | MeshUV0 | The view direction in world space. |
| Out | **Output** | Vector 4 | None | The sampled value at UV coordinate of the chosen render texture. |

</div>

<h3 align="center">Options</h3>

<div align="center">

| Name | Type | Choices | Description |
| :---- | :---- | :---- | :---- |
| Render Texture | Enum | Tex\_Color Tex\_Albedo Tex\_Normal Tex\_Depth Tex\_DepthNormal Tex\_Specular Tex\_Emissive Tex\_LineData1 Tex\_LineData2 Tex\_00 Tex\_01 Tex\_02 Tex\_03 Tex\_04 Tex\_05 Tex\_06 Tex\_07 | Each entry corresponds to a possible NPRP render texture. |

</div>
