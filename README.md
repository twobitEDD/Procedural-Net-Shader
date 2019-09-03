## Procedural Unity ShaderGraph Net Sub Shader
This shader provides a black and white alpha map resembling a net without using any predefined textures as input.

## Screenshots
Sub Graph Preview | Usage Example
------------ | -------------
![Sub Graph Preview](/Examples/ShaderPreview.PNG) | ![Usage example](/Examples/UsageExample.PNG)

![Racket Example](/Examples/RacketExample.gif)
Note: The warping happening with tiling values != 0 can be used to counteract the stretching of the material that happens when the scale of the object changes.

<b>Built with</b>
- [Unity3D Shader Graph](https://unity.com/shader-graph)

## Features
Create a net of any size, density and thickness with this shader. The tiling parameter allows for offsetting any stretching caused by scaling the actual object itself.

## Prerequisites
**A Unity version supporting the HDRP/LWRP and ShaderGraph is needed to use this sub-shader!**

## Installation
* Download the .shadersubgraph file
* Save the file in your Project/Assets folder

## How to use?
* Create a new shader
* Select "Create Node"
* Under "Sub Graphs" select the Net shader
* Plug your exposed values into the input
* Plug the output into the alpha channel of the master node

**Important**
* If you want to use the shader as suggested, as an alpha map, you need to set the **Blend Mode** of the master node to **Transparent**
* The tiling value has to be at least 1 on each axis, otherwise the procedural image will be scaled by 0
