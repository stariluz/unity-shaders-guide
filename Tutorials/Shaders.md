# Shaders in Unity
There are three main categories for shaders in unity:
1. Graphic shaders. Those that performe calculations to determine the color of the pixels on the screen.
2. Compute shaders. Compute calculations on the CPU, but these are out of the graphics pipeline.
3. Ray tracing shaders. They are focused on the lighting.

The Unity's Shaders are written in a Unity-specific language called ShaderLab. However, in Unity we can do shaders no-code with the Shaders Graph.

## Master stack.

A Master stack is the endpoint of every Shader Graph that defines the final surface appareance of a shader. The Shader Graphs should always contain only one.

The Master Stacks are made up of two contexts (Vertex and Fragment), wich contains Block nodes.

### Vertex Shader
Vertex shaders can manipulate the attributes of vertces, wich are your corner points of the polygons. It is part of the early steps in the graphic pipeline.

### Fragment (or pixel) shaders
Fragment shaders manage how the pixels between the vertices look. They are interpolated between the defined vertices. It is part of the rasterization step, where the image is calculated an the pixels between verticesare coloured.

> If you want your polygon to be completely red, you would define all vertices red. If you want for specific effects like a gradient between the vertices, you have to do that in the fragment shader.

Resources consulted.
[The surrican. Vertex shader vs Fragment Shader.](https://stackoverflow.com/a/4421289/18456344). Stack Overflow.
[Unity Manual. Master Stack](https://docs.unity3d.com/Packages/com.unity.shadergraph@10.5/manual/Master-Stack.html?utm_source=demand-gen&utm_medium=pdf&utm_campaign=asset-links-gmg-artist-expansion&utm_content=technical-artist-ebook). Unity.
