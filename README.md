# Fabric端一些推荐的OptiFine替代品
原文：[Recommended OptiFine alternatives on Fabric by LambdAurora](https://gist.github.com/LambdAurora/1f6a4a99af374ce500f250c6b42e8754)
本文为随缘渣翻，将原文翻译后搬运到自己的github repo已获得原作者LambdAurora许可。

# 缘由

OptiFine本来是个非常不错的Mod，在早期的时候，它的很多功能都改善了玩家的游戏体验。不过这么多年以来，不仅本来的优势已经衰退，还给Mod开发者们带来了不少问题。因为Minecraft的代码量一直在逐年增长，而OptiFine不仅闭源，还很激进地替换大片代码，所以也很难搞懂这OptiFine怎么就把别人开发的Mod给整出问题了。值得注意的是OptiFine并不原生支持Fabric，OptiFabric也很难继续维护。

时间推进到Minecraft的现代(1.14.x - ~)，在Fabric社区的努力下，Mod开发者们也开始开发可以替代OptiFine大多数功能的Mod，玩家也可以获得更好的游戏性能体验，Mod兼容性，以及Mod支持。

[OptiFabric: 关于1.16崩溃的说明 (OptiFabric: A note about the 1.16 crashes)](https://github.com/modmuss50/OptiFabric/issues/242)

# 替代品

- [Connected Block Textures (CBT)](https://www.curseforge.com/minecraft/mc-mods/connected-block-textures) - 连接材质(CTM)，可以实现如无缝玻璃之类的效果。 (目前不适配Sodium)
  - 若要修复玻璃板底部或顶部的视觉效果的问题，请访问: https://github.com/Nuclearfarts/connected-block-textures/issues/1
- [Colormatic](https://www.curseforge.com/minecraft/mc-mods/colormatic) - 自定义颜色
- [LambDynamicLights](https://www.curseforge.com/minecraft/mc-mods/lambdynamiclights) - 动态光源
- [Soaring Clouds](https://www.curseforge.com/minecraft/mc-mods/soaring-clouds) - 可配置云层高度
- [ItemNbtModels](https://github.com/Linguardium/ItemNbtModels) - 自定义物品模型 (不支持OptiFine的格式)
- [Varied Mob Textures](https://www.curseforge.com/minecraft/mc-mods/varied-mob-textures) - 随机实体材质 (使用其特有的格式，目前不打算兼容OptiFine格式)

## 性能优化类

### 客户端

- [Sodium](https://www.curseforge.com/minecraft/mc-mods/sodium) - 性能优化 [(甚至比OptiFine优秀)](https://youtu.be/0fAB6pJK6U4) 不过没有"高品质"选项 (如果想要"高品质"选项可以试试Canvas Renderer)
- [Canvas Renderer](https://www.curseforge.com/minecraft/mc-mods/canvas-renderer) - 着色器与性能优化
- [Cull Particles](https://www.curseforge.com/minecraft/mc-mods/cull-particles-fabric) - 如果已经安装了Sodium，就不需要安装本Mod了。

### 通用

- [Lithium](https://www.curseforge.com/minecraft/mc-mods/lithium) - 服务端优化 (单人模式也有用)
- [Phosphor](https://www.curseforge.com/minecraft/mc-mods/phosphor) - 光照引擎优化

## 关闭动态FOV(视场角)

**从1.16.2-pre1开始，原版的“辅助功能设置”添加了相关选项。如果你玩的是1.16.2-pre1或者更高的版本，就不用关注下列的Mod了**

这些是客户端Mod，避免Minecraft在所有情况下更改FOV。 (比如喝了迅捷药水之后的速度状态)

- [motioNO](https://www.curseforge.com/minecraft/mc-mods/motiono) - 关闭动态FOV.
- [FovLock](https://github.com/ChloeDawn/FovLock) - 添加了动态FOV锁定按钮.

## 开启/关闭迷雾

- [Sodium](https://www.curseforge.com/minecraft/mc-mods/sodium) 可以开关主世界地形的迷雾。
- [ClearView](https://www.curseforge.com/minecraft/mc-mods/clearview)
- [NoFog](https://www.curseforge.com/minecraft/mc-mods/nofog)

## 视野放大

- [Ok Zoomer](https://www.curseforge.com/minecraft/mc-mods/ok-zoomer)
- [Logical Zoom](https://www.curseforge.com/minecraft/mc-mods/logical-zoom)
- [WI Zoom](https://www.curseforge.com/minecraft/mc-mods/wi-zoom)

# 暂无此类功能的替代品

- 自定义实体模型(custom entity models)
- 天空特性(sky features)

# 兼容性

Sodium与Canvas Renderer互不兼容。
Sodium目前并没有实现Fabric renderer API，所以与部分类似Connected Block Textures (CBT)的Mod不兼容。

# 帮助

如果安装这些Mod的时候遇到问题需要帮助，可以访问[Fabric的Discord服务器](https://discord.gg/v6v4pMv)，并在player-support频道询问。

如果有关于Sodium, Lithium, Phosphor（简单讲就是JellySquid开发的Mod）的问题，[请访问她的Discord服务器](https://jellysquid.me/discord)。

如果有跟LambDynamicLights相关的问题，又或者不想在评论区提建议，请访问[本文档原作者LambdAurora的Discord服务器](https://discord.gg/abEbzzv)

# 其他列表

 - [Fabric端一些有用的服务端Mod (Useful Fabric server-side mods)](https://gist.github.com/comp500/12417ee3685f6204362e933c9bcde603)
 - [Optifabric的未来以及推荐的替代品 (The future of Optifabric and Recommended alternatives)](https://gist.github.com/modmuss50/deff1658c4550ca8b16cb5d40ceaa468)
 - [Calloatti的列表](https://gist.github.com/calloatti/6220c04e136d329298fd35066dfcc9b0)
