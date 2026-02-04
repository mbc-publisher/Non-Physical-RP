### NP Render Stack {#np-render-stack}

**Description**

The render stack that gives you the most freedom and control over your rendering pipeline. Set up your render targets, whether or not they get a copy, when they get a copy, when shadows are casted, are you going with a deferred, forward, bit of both? Customise how your MRTs are set, used and much more.

**Parameters**

| Name | Type | Choices | Description |
| :---- | :---- | :---- | :---- |
| Global Render targets | Array / List |  | Render targets which can be shared across the render passes. Two render passes are default and can’t be deleted, the Main Color and the Main Depth. These 2 will persist until the end of each frame. |
| MRT Sets | Array / List |  | Sets of multiple render targets that can be rendered to at the same time in the same drawcall. |
| Render Passes | Array / List |  | The passes that drive your rendering in a top to bottom order. No order is hardcoded so if your specific artistic Idea requires the transparents to be rendered before the opaques then you can do so. |
