<h1 align="center">Screen Material</h1>

<h3 align="center">Description</h3>

<div align="center">Draw a material on a plane covering the whole screen. This can be used for post process materials or deferred rendering. When used for deferred rendering, the custom material gives you full control over the stylisation of your game. If you need some render targets to stay available for this pass, use a Clear pass somewhere after this one and add the required render targets. This will ensure that they do not get cleared automatically before.</div>

<h3 align="center">Parameters</h3>

| Name | Type | Choices | Description |
| :---- | :---- | ----- | :---- |
| MRT Set | Enum | Any declared MRT Set in the Render Stack. | The MRT Set on which you want to render the result. (Usually the main color and main depth). |
| Material | Material |  | The material used to render on the screen. |
