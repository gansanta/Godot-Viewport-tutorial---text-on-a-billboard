# Godot-Viewport-tutorial---text-on-3D-surface
Let's make a 2D scene at first. It will display an image, a title and a description.

1. Create a new Scene. Add a Node2D as a root node. Rename it as 'Scene2D'.
2. Select Scene2D node. Then add a ColorRect node. Rename it as 'Background'. In the Inspector tab, set its size as x:400, y:200. [Find the Control section, expand the Rect property, you will see the size with x and y slot.]
![img1-colorRect1.png](https://github.com/gansanta/Godot-Viewport-tutorial---text-on-3D-surface/blob/master/img1-colorRect1.png)
3. Select Scene2D. Now Add a Sprite node. Rename it as 'Icon'. We will add a picture to it. 
4. In the Scene tree, select the Icon node. In the Inspector tab, under 'Sprite' heading, you will now see texture as [empty]. We are going to fill it with Godot icon.
5. In the resource directory (res://), find the Godot icon as 'icon.png'. Drag it on the [empty] texture slot. You will now see the Godot icon on the screen. Drag it in the left side, as shown in the picture and leave it there.

6. 
