# LiberatorEngine
A game engine for creating high quality 3D scene


# Targets
- 


#features
## Math
- an in-house math lib

## Renderer
- data driven
- multi-threading rendering
- component-based
- very customized and friendly material system
- forward, deferred rendering switch
- skeleton animation
- billboard
- particle effect
- quadtree terrain
- instancing

  The renderer is totally data-driven, which allow you to modify the renderpath to config any combinated frames you want. e.g. 
reflection-refrection water, screen-based fog, bloom, volumetric light, SSAO, and even you can easily switch between
forward and defferred rendering. The engine also has a customized material system. Basically the material file is a xml, which 
composite of shader, variables, textures. There, you can pass whatever you want to the shader through the xml, even a RenderTarget
on the fly, which contain the drawed result based on your renderpath, and that is up to you. Togeter with the renderpath and material
system, you can config whatever frames, and can test a graphic algorithm efficiently with few little xml files.  
  The engine has some render component hard coded, such as mesh/skinned-mesh, billboard group, quadtree terrain, particles, so enjoy
it by few lines of codes.

***
## Editor 
The editor is designed to edit the scene, view the models, etc. Since the engine is entity-component based, so you can
modify component and material in the editor. Everything will be stream to a xml scene file, everything is persistent!!!

***

