<h1 align="center">Get Global Illumination</h1>

<h3 align="center">Description</h3>

<div align="center">Return the baked global illumination or skydome if not applicable.</div>

<h3 align="center">Ports</h3>

<div align="center">
  
| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | ----- |
| Lightmap UV | **Input** | Vector 2 | MeshUV1 | The UV of the mesh used for the light maps (Usually UV1). |
| Normal WS | **Input** | Vector 3 | WorldSpaceNormal |  The normal vector in world space. |
| Position WS | **Input** | Vector 3 | WorldSpacePosition | The position vector in world space. |
| GI | **Output** | Vector 3 | None | Global Illumination. |

</div>
