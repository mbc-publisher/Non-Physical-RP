<h1 align="center">Get Reflection</h1>

<h3 align="center">Description</h3>

<div align="center">Return the baked reflection or skydome if not applicable.</div>

<h3 align="center">Ports</h3>

<div align="center">
  
| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| View Direction | **Input** | Vector 3 | WorldSpaceViewDirection | The view direction in world space. |
| Normal | **Input** | Vector 3 | WorldSpaceNormal | The normal vector in world space. |
| Roughness | **Input** | Float | None | 0 is glossy, 1 is rough. |
| Metalness | **Input** | Float | None | 0 is not a metal, 1 is fully metallic. |
| Reflection | **Output** | Vector 3 | None | Output the resulting reflection. |

</div>
