**Ray Generation Shader:**
  This file is responsible for shooting a ray into the scene for each pixel on the screen. It uses the camera’s position and orientation to figure out which direction the ray should travel, traces that ray through the scene, and stores the result so it can be displayed or used by later rendering steps.

**Closest-Hit Shader**
  This file runs when a ray hits an object in the scene. It determines what the surface looks like at the hit point (fetches vertex, material, and texture data from GPU buffers), computes lighting for that spot, and sends out extra rays to check shadows and reflections. It then returns the final color and surface information needed to produce the image.
