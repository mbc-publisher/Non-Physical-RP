<h1 align="center">Unpacking</h1>

<h3 align="center">Description</h3>

<div align="center">unpack the input value into a larger set of values. More options to come!</div>

<h3 align="center">Ports</h3>

<div align="center">

| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| Packed | **Input** | Float | None | Packed value. |
| X | **Output** | Float | None | Unpacked X value. |
| Y | **Output** | Float | None | Unpacked Y value. |
| Z | **Output** | Float | None | Unpacked Z value. |
| W | **Output** | Float | None | Unpacked W value. |
| Float2 | **Output** | Vector 2 | None | Unpacked Float2 vector. |
| Float3 | **Output** | Vector 3 | None | Unpacked Float3 vector. |
| Float4 | **Output** | Vector 4 | None | Unpacked Float4 vector. |
| Depth | **Output** | Float | None | Depth Value. |
| Normal | **Output** | Vector 3 | None | Normal Value (View Space). |

</div>

<h3 align="center">Options</h3>

| Name | Type | Choices | Description |
| :---- | :---- | :---- | :---- |
| Output State | Enum | •Expanded<br> •Collapsed | **Expanded:** Each channel is a separate output pin ( X, Y, Z, W, Depth).<br><br> **Collapsed:** The output is a vector ( vector2, vector3, vector4, Normal(vector3) & Depth(vector1)) |
| Mode | Enum | •DepthNormal<br> •F1x8y8z8a8\_F4<br> •F1x5y6z5\_F3<br> •F1x8y8\_F2 | **DepthNormal:** returns screen space Normal.<br><br> **Others:** The first name is the input value and how many bits are allocated for each channel of the output value (F1 \= Float1, x8 means 8 bit for the X channel of the output). The second name is the output value(F4 \= Float4). |

</div>
