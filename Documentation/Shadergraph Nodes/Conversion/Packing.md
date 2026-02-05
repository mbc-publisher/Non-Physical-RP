<h1 align="center">Packing</h1>

<h3 align="center">Description</h3>

<div align="center">Pack the input values into a smaller value. More options to come!</div>

<h3 align="center">Ports</h3>

<div align="center">

| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| X | **Input** | Float | None | X value. |
| Y | **Input** | Float | None | Y value. |
| Z | **Input** | Float | None | Z value. |
| W | **Input** | Float | None | W value. |
| Depth | **Input** | Float | None | Depth Value. |
| Normal | **Input** | Vector 3 | ViewSpaceNormal | Normal Value (View Space). |
| Float2 | **Input** | Vector 2 | None | Float2 vector. |
| Float3 | **Input** | Vector 3 | None | Float3 vector. |
| Float4 | **Input** | Vector 4 | None | Float4 vector. |
| Packed | **Output** | Float | None | Result packed value. |

</div>

<h3 align="center">Options</h3>

<div align="center">

| Name | Type | Choices | Description |
| :---- | :---- | :---- | :---- |
| Input State | Enum | •Expanded<br> •Collapsed | **Expanded:** Each channel is a separate input pin ( X, Y, Z, W, Depth).<br><br> **Collapsed:** The input is a vector ( vector2, vector3, vector4, Normal(vector3) & Depth(vector1)) |
| Mode | Enum | •DepthNormal<br> •F4\_F1x8y8z8a8<br> •F3\_F1x5y6z5<br> •F2\_F1x8y8 | **DepthNormal:** requires screen space Normal.<br><br> **Others:** The first name is the input value(F4 \= Float4),  the second name is the output value and how many bits are allocated for each channel of the input value (F1 \= Float1, x8 means 8 bit for the X channel of the input.)  The total of bit indicates the precision of the output.  ( F1x8y8z8a8 is a 32 bit float, F1x5y6z5 is a 16 bit half). |

</div>
