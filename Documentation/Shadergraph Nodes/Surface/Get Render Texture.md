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
| Render Texture | Enum | •Tex\_Color<br> •Tex\_Albedo<br> •Tex\_Normal<br> •Tex\_Depth<br> •Tex\_DepthNormal<br> •Tex\_Specular<br> •Tex\_Emissive<br> •Tex\_LineData1<br> •Tex\_LineData2<br> •Tex\_00<br> •Tex\_01<br> •Tex\_02<br> •Tex\_03<br> •Tex\_04<br> •Tex\_05<br> •Tex\_06<br> •Tex\_07<br> | Each entry corresponds to a possible NPRP render texture. |

</div>
