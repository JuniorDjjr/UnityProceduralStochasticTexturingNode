# Unity Procedural Stochastic Texturing Node for Shader Graph
Procedural stochastic texturing node for Unity's Shader Graph, to fix repeated tile patterns on tiled textures.  

**For terrain: https://github.com/JuniorDjjr/Unity-Procedural-Stochastic-Texture-Terrain-Shader**  

Just use this file as a custom function node for Shader Graph. Color and normal/bump versions map are separated.  

![](https://1.bp.blogspot.com/-nQy-BVqnTPM/XrnbfO7LctI/AAAAAAAAYOY/mAjoKityEYIA3fKWPGhHQ7LCDaPhVAniACK4BGAsYHg/w1175-h1170/warpunk-game-procedural-stochastic-terrain-shader-texturing-unity-urp.jpg)

**Limitation:** The UV is calculated locally at the object's UV position, so the edges of objects will not be seamless for the same texture. Someone more experienced than me can try UV randomation by world space, or you can try something like vertex color to define a mask where the effect is applied.

This solution can also be adapted into other games, such as [GTA San Andreas](https://github.com/JuniorDjjr/skygfx):  
![](https://www.mixmods.com.br/wp-content/uploads/2022/03/gta-sa-mod-skygfx-extended-stochastic-procedural-texture-tiling-fix-7201275.jpg)

From [rotoscope](https://www.reddit.com/user/rotoscope-/) adaptation, based on [Thomas Deliot and Eric Heitz paper](https://drive.google.com/file/d/1QecekuuyWgw68HU9tg6ENfrCTCVIjm6l/view), implemented by me (Junior_Djjr) for Unity shader graph.  
