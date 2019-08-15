# Godot-Viewport-tutorial---text-on-a-billboard

1. In Godot, create a 2D scene at first. It will contain a colorRect as Background, a sprite as the Icon, a label as the Name and another label as the Description node. See the image below.
![img01-2Dscene.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img01-2Dscene.png)


2. Create another 3D scene. Save it as a billboard scene. It will contain a spatial node as the Billboard, a viewport, a Scene2D instance of the 2D scene we have created earlier, and a 3D MeshInstance as a Screen. See the screenshot below.
![img02-billboard.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img02-billboard.png)

Important things about Viewport:
  1) Set viewport width = 3x of ColorRect width; Viewport Height = 2x of ColorRect Height. In my 2D scene, the ColorRect size was x=300, y=100. So here I set Viewport width=900, height=200. If you don't follow this ratio, your billboard will show only a black screen!
  2) Also turn VFlip on.
  
  ![img04-viewport1.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img04-viewport1.png)
  
  3) Put the Viewport the first on the hierarchy. Otherwise sometimes it will throw an error.
  4) The screen is a mesh instance. Set its mesh size as: x=10, y=6, z=1. Later you can try with different values.
 ![img03-meshsize.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img03-meshsize.png)
 
 5) While Screen node selected, find the Geometry in the GeometryInstance in the Inspector tab. Expand it. Find the Material Override property and choose new spatial material. Then click on it again.
![img05-screen.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img05-screen.png)

6) New Spatial Material will open with lots of properties. Scroll down below and find Resource and set Local to Scene as on. Otherwise you won't be able to select the Viewport as a texture.
![img06-screen2.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img06-screen2.png)

7) Now scroll up and find Albedo. Expand it and find the texture. In the texture menu, select New ViewportTexture. A dialogbox will ask you to pick up a viewport. Pick the viewport and you are done. See the image.
![img07-screen3.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img07-screen3.png)

You have got your wonderful Godot billboard.
