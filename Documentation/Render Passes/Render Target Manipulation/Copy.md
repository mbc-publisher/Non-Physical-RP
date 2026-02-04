<h1 align="center">Copy</h1>

<h3 align="center">Description</h3>

<div align="center">Copy the content of the render target(s) to a copy buffer so the content of those can be accessible while writing to them later. Similar to the copy color option in Unity’s rendering pipelines.</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| To Copy | Array / List | Any Render Target identified as copyable. | Will copy the content of those render targets to a copy buffer after the rendering of geometry. The copies will then be available to use for the next render passes.
