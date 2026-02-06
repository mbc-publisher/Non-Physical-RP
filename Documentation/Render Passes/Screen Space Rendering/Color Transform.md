<h1 align="center">Color Transform</h1>

<h3 align="center">Description</h3>

<div align="center">Lets you apply some common color transformation techniques. They are grouped in one pass to optimize the draw calls as much as possible. Each transformer can be toggled on or off.</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Post Exposure (Toggleable) | Float | Range 0 \- ∞ | Is added to the color. |
| Tone Mapper (Toggleable) | Enum | •ACES<br> •Neutral<br> •Reinhard<br> •Normalize<br> | Remap the values (usually HDR ones) between 0-1 (LDR) |
| Color Grading | Boolean |  | Enables Color Grading |
| Contrast (Color Grading) | Float | Range&#8239;\-100&#8239;\-&#8239;100 | Increase or decrease the contrast. |
| Color Filter (Color Grading) | Color |  | Multiply by that color. |
| Hue Shift (Color Grading) | Int | Range&#8239;\-180&#8239;\-&#8239;180 | Adjust the Hue. |
| Saturation (Color Grading) | Float | Range&#8239;\-100&#8239;\-&#8239;100 | Increase or decrease the contrast. |
| White Balance | Boolean |  | Enables White Balance |
| Temperature (White Balance) | Float | Range&#8239;\-100&#8239;\-&#8239;100 | Make the color warmer or colder. |
| Tint (White Balance) | Float | Range&#8239;\-100&#8239;\-&#8239;100 | shifts the green–magenta balance |
| Split Tonning | Boolean |  | Enables Split Tonning |
| Shadows (Split Tonning) | Color |  | The color tint applied to dark areas. |
| Highlights (Split Tonning) | Color |  | The color tint applied to bright areas. |
| Balance (Split Tonning) | Float | Range&#8239;\-100&#8239;\-&#8239;100 | Controls where the midpoint between shadows and highlights lies |
| Channel Mixer | Boolean |  | Enables Channel Mixer |
| Red (Channel Mixer) | Vector 3 |  | Lets you put the red value of the color in the red, green or blue channel non-exclusively and weighted as you wish. |
| Green (Channel Mixer) | Vector 3 |  | Lets you put the green value of the color in the red, green or blue channel non-exclusively and weighted as you wish. |
| Blue (Channel Mixer) | Vector 3 |  | Lets you put the blue value of the color in the red, green or blue channel non-exclusively and weighted as you wish. |
| Shadows Midtones Highlights | Boolean |  | Enables Shadows Midtones Highlights |
| Shadows (Shadows Midtones Highlights) | Color |  |  |
| Midtones (Shadows Midtones Highlights) | Color |  |  |
| Highlights (Shadows Midtones Highlights) | Color |  |  |
| Shadows Start (Shadows Midtones Highlights) | Float | Range&#8239;0&#8239;\-&#8239;1 | The start of the luminance range that represents the shadows. |
| Shadows End (Shadows Midtones Highlights) | Float | Range&#8239;0&#8239;\-&#8239;1 | The end of the luminance range that represents the shadows. |
| Highlights Start (Shadows Midtones Highlights) | Float | Range&#8239;0&#8239;\-&#8239;1 | The start of the luminance range that represents the highlights. |
| Highlights End (Shadows Midtones Highlights) | Float | Range&#8239;0&#8239;\-&#8239;1 | The end of the luminance range that represents the highlights. |

<h3 align="center">More Settings</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Main Color | Enum | Any Non-Depth Render Target | You can choose to override which color render target will be used for this pass. |
| Main Depth | Enum | Any Depth Render Target | You can choose to override which depth render target will be used for this pass. |
