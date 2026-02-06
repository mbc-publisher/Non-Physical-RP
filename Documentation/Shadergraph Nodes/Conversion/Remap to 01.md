<h1 align="center">Remap to 01</h1>

<h3 align="center">Description</h3>

<div align="center">Remap either -1 to 1 or 0 to 100 values to 0 to 1. The only difference with Unity’s Remap node is that it’s a little bit less expensive as it requires no divisions.  
The difference is barely noticeable.</div>

<h3 align="center">Ports</h3>

<div align="center">

| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| XYZ | **Input** | Vector 3 | None | The XYZ channels.(or RGB). |
| W | **Input** | Float | None | The W channel. (or A). |
| Out | **Output** | Vector 4 | None | The resulting Vector4. |

</div>

<h3 align="center">Options</h3>

<div align="center">

| Name | Type | Choices | Description |
| :---- | :---- | :---- | :---- |
| In Range | Enum | •-1 to 1<br> •0 to 100 | Specify the range of the input. |

</div>
