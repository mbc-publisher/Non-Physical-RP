<h1 align="center">Lines</h1>

<h3 align="center">Description</h3>

<div align="center">Draw lines. Either Inverse hull, Sobel like or Brush.</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Line Data 1 | Enum | Any Non-Depth Render Target | The render target used to store Line Data 1\. |
| Line Data 2 | Enum | Any Non-Depth Render Target | The render target used to store Line Data 2\. |
| Depth Normal | Enum | Any Non-Depth Render Target | The render target used to store the Depth Normal. |
| Line Type | Enum | •Inverse Hull<br> •Expand<br> •Brush<br> | **Inverse Hull:** Rerender the geometry with flipped face.  **Expand:** Uses multiple passes to expand the width of the lines **Brush:** Renders lines as brush strokes. |
| Render Scale | Float | Range 0 \- 1 | Sets the size of the line detection texture. This greatly affects performance. For brush lines it can also be used as a means to space out the brush (similar to the spacing option in photoshop). |
| Depth Fade (Toggleable) | Float | Range 0 \- ∞ | Makes the line thinner with distance. |
| Contour Thickness | Float | Range 0 \- 1 | Drives the thickness of contour lines. |
| Inner Thickness | Float | Range 0 \- 1 | Drives the thickness of Inner lines. |
| Min Line Length | Float | Range 0 \- 4 | (⚠Incoming Feature⚠) Removes lines that are too short and noisy. |
| Depth Threshold | Float | Range 0 \- 1 | Dictates the threshold for changes in depth to make a line. |
| Normal Threshold | Float | Range 0 \- 1 | Dictates the threshold for changes in the normal to make a line. |
| Custom Threshold | Float | Range 0 \- 1 | Dictates the threshold for changes in the custom lines buffer to make a line. |
| Detect Direction | Boolean |  | If enabled, it rotates the brush stroke to follow the curvature of the mesh. |
| Rotation | Float | Range \-180 \- 180 | Apply a global additional rotation to the brush. |
| Brush Texture | Texture 2D |  | The texture of the brush stroke. Can be a sprite sheet. Greyscales can be used to emulate brush pressure. |
| Tiles | Vector2 Int |  | The Tiles of the Brush Texture. ( (1,1) if not a sprite sheet. |
| Texture Index | Int | Range 0 \- (Tiles.x \* Tiles.y \- 1\) | The index of the Brush in the Brush Texture. |
| Contour Color | Color |  | Color Multiplier for contour lines. (Does not support HDR yet) |
| Inner Color | Color |  | Color Multiplier for Inner lines. (Does not support HDR yet) |

<h3 align="center">More Settings</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Main Color | Enum | Any Non-Depth Render Target | You can choose to override which color render target will be used for this pass. |
| Main Depth | Enum | Any Depth Render Target | You can choose to override which depth render target will be used for this pass. |
