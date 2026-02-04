<h1 align="center">Skybox</h1>

<h3 align="center">Description</h3>

<div align="center">Render the skybox</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| To Copy | Array / List | Any Render Target identified as copyable. | Will copy the content of those render targets to a copy buffer after the rendering of the Skybox. The copies will then be available to use for the next render passes. |

<h3 align="center">More Settings</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| Main Color | Enum | Any Non-Depth Render Target | You can choose to override which color render target will be used for this pass. |
| Main Depth | Enum | Any Depth Render Target | You can choose to override which depth render target will be used for this pass. |
