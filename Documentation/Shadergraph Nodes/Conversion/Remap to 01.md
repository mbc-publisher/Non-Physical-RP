<h1 align="center">Remap to 01</h1>

<h3 align="center">Description</h3>

<div align="center">Remap either -1 to 1 or 0 to 100 values to 0 to 1. The only difference with Unity’s Remap node is that it’s a little bit less expensive as it requires no divisions.  
The difference is barely noticeable.</div>

<h3 align="center">Ports</h3>

<div align="center">

| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| In | **Input** | float | None | A value ranged between -1 to 1 or 0 to 100. |
| Out | **Output** | float | None | The value remaped to a 0 to 1 range. |

</div>

<h3 align="center">Options</h3>

<div align="center">

| Name | Type | Choices | Description |
| :---- | :---- | :---- | :---- |
| In Range | Enum | •-1 to 1<br> •0 to 100 | Specify the range of the input. |

</div>
