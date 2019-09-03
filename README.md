## Procedural Unity ShaderGraph Net Sub Shader
This shader provides a black and white alpha map resembling a net without using any predefined textures as input.

## Screenshots
[Sub Graph Preview](https://i.imgur.com/gpTS6PV.png)
[Usage example](https://i.imgur.com/UyPPI1w.png)

[Racket Example](https://gfycat.com/browncooldeer)

## Tech/framework used
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
