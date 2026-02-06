<h1 align="center">Pack Lines Data</h1>

<h3 align="center">Description</h3>

<div align="center">Pack the Lines data into two float4 ready to be input into the corresponding render textures.</div>

<h3 align="center">Ports</h3>

<div align="center">

| Name | Direction | Type | Binding | Description |
| :---- | :---- | :---- | :---- | :---- |
| Outline color | **Input** | Vector&nbsp;4 | None | The color of the outline. Outlines appear when different contour IDs are neighbouring. |
| Inline Color | **Input** | Vector&nbsp;4 | None | The color of the lines inside the same ID. |
| Contour ID | **Input** | Float | None | The Value that drives contour lines. Values are between 1 and 255\. (0 means no lines). |
| Custom Line | **Input** | Float | None | A greyscale value between 0 and 1 that let you create lines that would not show-up with depth and normal sampling. |
| Contour Thickness | **Input** | Float | None | The thickness of the outline line. |
| Inline Thickness | **Input** | Float | None | The thickness of the lines inside the same ID. |
| Rotation | **Input** | Float | None | The rotation of the brush (Only used with brush lines). |
| Pressure | **Input** | Float | None | The pressure of the brush, it will simulate a harder press on the brush with a brush texture that has an opacity gradient.(Only used with brush lines). |
| Data1 | **Output** | Vector&nbsp;4 | None | All the data from Contour ID to pressure is packed in an 8 bit per channel Float4 for maximum compatibility. |
| Data2 | **Output** | Vector&nbsp;4 | None | The colors data are packed in an 8 bit per channel Float4 for maximum compatibility. This data is optional if you don't intent on using per material color |

</div>
