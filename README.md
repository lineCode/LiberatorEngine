# LiberatorEngine
A 3D game engine for creating high quality 3D scene. I spend 1 year to write the game engine during the last year of my college, and also reconstruct it few times. The name comes from a song called Liberator, by Epic score. Because the song sound like battle of nightfall.Since it was the last fight in the cage, i would unlock it once i finish it and be free. Anyway i'll rename it if i think out a better one. Hopefully, i finished it before the end of college. And i use it as my graduation thesis but unfortunately, i cant get full mark. <br>
If you're not Chinese, please skip the section below. <br>

<pre>
 事实上是上机演示前没准备好，那个老师的关注点不对啦。 引擎特性多也写了很多优化，最后能让人看到的只有一个编辑器和用编辑器做
出来的一个场景demo。 那老师也是了解过3D的东西的，还问有没有实现光照阴影啊、AA啊，既然是一个引擎怎么可能没有这些呢，都是最
基本的好不好，引擎的重点都不在这。那个老师名下有个”创新班”，不过貌似只做web,app，所以我也不想去他那个班。那老师有歧视，
只要不是他那个班的都不给优。那老师本身SB又倚老卖老，还说”你们做的那些所谓系统，没有谁的系统是特别吊的，做了老师这么多年有
什么没见过“，答辩让我们1分钟讲完。 我又不能容忍花了很多心血做的引擎被说成”那些系统“，答辩的时候ZHUANG B了一下，那老师又
不懂，只能从论文里强行找bug，给的成绩也不是优。
</pre>

<br>
<br>
<br>

# Targets
- 


# features
***
## General
- entity-component

***
## Math
- an in-house math lib

## Renderer
- d3d11 
- hlsl
- Assimp based model converter
- data driven pipeline
- multi-threading rendering
- render components : skeleton animation,billboard, particle effect, quadtree terrain, decals
- very customized and friendly material system
- forward, deferred rendering switch
- PCF shadow
- Frustum culling
- instancing
- auto shader parameters management

 <pre>
  The renderer is totally data-driven, which allow you to modify the renderpath to config any 
combinated frames you want. e.g. reflection-refrection water, screen-based fog, bloom, volumetric light, 
SSAO, and even you can easily switch between forward and defferred rendering. The engine also has a 
customized material system. Basically the material file is a xml, which composite of shader, variables, 
textures. There, you can pass whatever you want to the shader through the xml, even a RenderTarget on the 
fly, which contain the drawed result based on your renderpath, and that is up to you. So-what skybox, 
reflection-refrecion water, trasparent things will all be easy stuff, haha. Togeter with the renderpath and 
material system, you can config whatever frames, and can test a graphic algorithm efficiently with few little 
xml files.  
  The engine has some render component hard coded, such as mesh/skinned-mesh, billboard group, 
quadtree terrain, particles, so enjoy it by few lines of codes.  
</pre>
   

 


***
## Editor 
- hot loading
- scene edit
- view model
- material edit
- component edit
 
 <pre>
 The editor is designed to edit the scene, view the models, etc. Since the engine is entity-component based, 
so you can modify component and material in the editor. Everything will be stream to a xml scene file, everything 
is persistent!!!
</pre>

***

<br>
<br>
<br>
<br>

# Samples

Completed at 2017.5.18
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
![](https://github.com/kampxtr/LiberatorEngine/blob/master/screenshots/clipboard.png)
<br>
<br>
<br>
<br>
<br>
<br>
![](https://github.com/kampxtr/LiberatorEngine/blob/master/screenshots/%E5%9B%BE%E7%89%873.png)
<br>
<br>
<br>
<br>
<br>
<br>
![](https://github.com/kampxtr/LiberatorEngine/blob/master/screenshots/%E5%9B%BE%E7%89%871.png)
<br>
<br>
<br>
<br>
<br>
<br>
![](https://github.com/kampxtr/LiberatorEngine/blob/master/screenshots/%E5%9B%BE%E7%89%872.png)








