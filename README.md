# Godot-Viewport-tutorial---text-on-3D-surface

1. Create a 2D scene at first. It will contain an icon, a title and a description. See the image below.
![img01-2Dscene.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img01-2Dscene.png)


2. Create another 3D scene. Save it as a billboard scene. It will contain a screen, a Viewport that will have the 2D scene we created earlier. See the screenshot below.
![img02-billboard.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img02-billboard.png)

Important things about Viewport:
  1) Set viewport width = 3x of ColorRect width; Viewport Height = 2x of ColorRect Height. In my 2D scene, the ColorRect size was x=300, y=100. So here I set Viewport width=900, height=200. If you don't follow this ratio, your billboard will show only a black screen!
  2) Also turn VFlip on.
  
  ![img04-viewport1.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img04-viewport1.png)
  
  3) Put the Viewport the first on the hierarchy. Otherwise sometimes it will throw an error.
  4) The screen is a mesh instance. Set its mesh size as: x=10, y=6, z=1. Later you can try with different values.
 ![img03-meshsize.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-a-billboard/blob/master/img03-meshsize.png)
