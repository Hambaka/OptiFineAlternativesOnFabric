# Fabric 端一些推荐的 OptiFine 替代品
原文：[Recommended OptiFine alternatives on Fabric by LambdAurora][source]
本文为随缘渣翻，将原文翻译后搬运到自己的 github repo 已获得原作者 LambdAurora 许可。

[source]: https://gist.github.com/LambdAurora/1f6a4a99af374ce500f250c6b42e8754

# 缘由

OptiFine 本来是个非常不错的 Mod，在早期的时候，它的很多功能都改善了玩家的游戏体验。不过这么多年以来，不仅本来的优势已经衰退，还给 Mod 开发者们带来了不少问题。因为 Minecraft 的代码量一直在逐年增长，而 OptiFine 不仅闭源，还很激进地替换大片代码，所以也很难搞懂这 OptiFine 怎么就把别人开发的 Mod 给整出问题了。值得注意的是 OptiFine 并不原生支持 Fabric，OptiFabric 也很难继续维护。

时间推进到 Minecraft 的现代(1.14.x - ~)，在 Fabric 社区的努力下，Mod 开发者们也开始开发可以替代 OptiFine 大多数功能的 Mod，玩家也可以获得更好的游戏性能体验，Mod 兼容性，以及 Mod 支持。

[OptiFabric: 关于1.16崩溃的说明 (OptiFabric: A note about the 1.16 crashes)][optifabric_issue]

[optifabric_issue]: https://github.com/modmuss50/OptiFabric/issues/242

# 替代品

- [Connected Block Textures (CBT)][cbt] - 连接材质(CTM)，可以实现如无缝玻璃之类的效果。 (目前不适配 Sodium)
  - 若要修复玻璃板底部或顶部的视觉效果的问题，请访问该[链接][cbt_glass_panes]
- [Colormatic][colormatic] - 自定义颜色
- [CullLeaves] - 对树叶方块进行面剔除，类似于OptiFine中树叶设置里的“智能”选项。
- [LambDynamicLights][ldl] - 动态光源
- [LambdaBetterGrass] - 更好的草地和更好的雪地。
- [Raised Clouds][raised_clouds] & [Soaring Clouds][soaring_clouds] - 可配置云层高度
- [Varied Mob Textures][vmt] - 随机实体材质 (使用其特有的格式，目前不打算兼容 OptiFine 的格式)
- [FabricSkyboxes][fsb] - 自定义天空 (目前不兼容 OptiFine 的格式)
- [Fabrishot] - 用更高的分辨率截图
- [Custom Splash Screen] - 自定义资源加载页面的颜色、Logo以及进度条。
- [Dark Loading Screen][dls] - 资源加载界面的默认背景色改为暗色，但是和 OptiFine 一样支持自定义的颜色。
- [Splash] - 资源加载界面的默认背景色改为暗色，但是和 OptiFine 一样支持自定义的颜色。
- [Transparent] - 可以在资源包添加相应的配置文件更改画和各种方块的渲染方式，比如画可以应用透明材质，方块也可以选择是否应用玻璃连接面的渲染方式等等。

[cbt]: https://www.curseforge.com/minecraft/mc-mods/connected-block-textures "Connected Block Textures 的 CurseForge页面"
[cbt_glass_panes]: https://github.com/Nuclearfarts/connected-block-textures/issues/1 "Connected Block Textures 的玻璃板显示修复资源包"
[colormatic]: https://www.curseforge.com/minecraft/mc-mods/colormatic "Colormatic 的 CurseForge 页面"
[CullLeaves]: https://github.com/TeamMidnightDust/CullLeaves "CullLeaves 的 GitHub 页面"
[ldl]: https://modrinth.com/mod/lambdynamiclights "LambDynamicLights 的 Modrinth 页面"
[LambdaBetterGrass]: https://modrinth.com/mod/lambdabettergrass "LambdaBetterGrass 的 Modrinth 页面"
[raised_clouds]: https://www.curseforge.com/minecraft/mc-mods/raised-clouds "Raised Clouds 的 CurseForge 页面"
[soaring_clouds]: https://www.curseforge.com/minecraft/mc-mods/soaring-clouds "Soaring Clouds 的 CurseForge 页面"
[vmt]: https://www.curseforge.com/minecraft/mc-mods/varied-mob-textures "Varied Mob Textures 的 CurseForge 页面"
[fsb]: https://www.curseforge.com/minecraft/mc-mods/fabricskyboxes "FabricSkyboxes 的 CurseForge 页面"
[Fabrishot]: https://www.curseforge.com/minecraft/mc-mods/fabrishot "Fabrishot 的 CurseForge 页面"
[Custom Splash Screen]: https://www.curseforge.com/minecraft/mc-mods/custom-splash-screen "Custom Splash Screen"
[dls]: https://www.curseforge.com/minecraft/mc-mods/dark-loading-screen "Dark Loading Screen 的 CurseForge 页面"
[Splash]: https://www.curseforge.com/minecraft/mc-mods/splash "Splash 的 CurseForge 页面"
[Transparent]: https://www.curseforge.com/minecraft/mc-mods/transparent "Transparent 的 CurseForge 页面"

## 性能优化类

### 客户端

- [Sodium] - 性能优化 [(甚至比 OptiFine 更优秀)](https://youtu.be/0fAB6pJK6U4) 不过没有"高品质"选项 (如果想要"高品质"选项可以试试 Canvas Renderer)
- [Canvas Renderer][canvas] - 着色器与性能优化
- [Cull Particles][cull_particles] - 如果已经安装了 Sodium，就不需要安装本 Mod 了。
- [Dynamic FPS] - 游戏窗口处于非活动状态时，减少每秒渲染的帧数，降低 CPU/GPU 的使用率。

[Sodium]: https://modrinth.com/mod/sodium "Sodium 的 Modrinth 页面"
[canvas]: https://www.curseforge.com/minecraft/mc-mods/canvas-renderer "Canvas 的 CurseForge 页面"
[cull_particles]: https://www.curseforge.com/minecraft/mc-mods/cull-particles-fabric "Cull Particles 的 CurseForge 页面"
[Dynamic FPS]: https://www.curseforge.com/minecraft/mc-mods/dynamic-fps "Dynamic FPS 的 CurseForge 页面"

### 通用

- [Lithium] - 服务端优化 (单人模式也有用)
- [Phosphor] - 光照引擎优化 (与[Starlight]不兼容)
- [Starlight] - 重写光照引擎 (与 [Phosphor] 不兼容)，目前处于Beta阶段。

[Lithium]: https://modrinth.com/mod/lithium "Lithium 的 Modrinth 页面"
[Phosphor]: https://modrinth.com/mod/phosphor "Phosphor 的 Modrinth 页面"
[Starlight]: https://github.com/Spottedleaf/Starlight "Starlight 的 Modrinth 页面"

## 关闭动态 FOV(视场角)

**从1.16.2开始，原版的“辅助功能设置”添加了相关选项。如果你玩的是1.16.2或者更高的版本，就不用关注下列的 Mod 了**

这些是客户端 Mod，避免 Minecraft 在所有情况下更改 FOV。 (比如喝了迅捷药水之后的速度状态)

- [motioNO] - 关闭动态 FOV.
- [FovLock] - 添加了动态 FOV 锁定按钮.

[motioNO]: https://www.curseforge.com/minecraft/mc-mods/motiono "MotioNo的CurseForge页面"
[FovLock]: https://github.com/ChloeDawn/FovLock "FovLock的GitHub页面"

## 迷雾

- [Sodium] 可以开关主世界地形的迷雾。(当前正式版无此功能，仅开发版本具有该功能)
- [ClearView](https://www.curseforge.com/minecraft/mc-mods/clearview)
- [NoFog](https://www.curseforge.com/minecraft/mc-mods/nofog)
- [CustomFog](https://www.curseforge.com/minecraft/mc-mods/custom-fog)

## 光影(着色器)

- [Canvas Renderer][canvas]
- [Iris] - Minecraft的全新光影模组，旨在与现有的各类光影模组/Optifine光影兼容。

**注意:** Sodium与本节的所有模组都不兼容。

[Iris]: https://github.com/IrisShaders/Iris

## 视野放大

- [Ok Zoomer](https://www.curseforge.com/minecraft/mc-mods/ok-zoomer)
- [Logical Zoom](https://www.curseforge.com/minecraft/mc-mods/logical-zoom)

## 其他

- [Overworld Two] 新增一种世界生成，优化主世界和下界的世界生成速度。速度比原版快很多，但是生成的世界和原版并非完全一致。

[Overworld Two]: https://www.curseforge.com/minecraft/mc-mods/overworld-two "Overworld Two 的 CurseForge 页面"


# 暂无此类功能的替代品

- 上层/叠加/附加材质 (overlay textures)
- 自定义实体模型 (custom entity models)(也许会在原版1.17中实现该功能)
- 钓线与拴绳: 自定义线宽和材质。
- 光照:自定义不同维度下的火把，太阳，闪电以及下雨时的光照效果。

# 兼容性

Sodium 与 Canvas Renderer互不兼容。
Sodium 目前并没有实现 Fabric renderer API，所以与部分类似 Connected Block Textures (CBT) 的 Mod 不兼容。

# 帮助

如果安装这些 Mod 的时候遇到问题需要帮助，可以访问[ Fabric 的 Discord 服务器](https://discord.gg/v6v4pMv)，并在 player-support 频道询问。

如果有关于 Sodium, Lithium, Phosphor(简单讲就是 JellySquid 开发的 Mod )的问题，[请访问她的 Discord 服务器](https://jellysquid.me/discord)。

如果有跟 LambDynamicLights 相关的问题，又或者不想在评论区提建议，请访问[本文档原作者 LambdAurora 的 Discord 服务器](https://discord.gg/abEbzzv)

# 其他列表

 - [Fabric 端一些有用的服务端 Mod (Useful Fabric server-side mods)](https://gist.github.com/comp500/12417ee3685f6204362e933c9bcde603)
 - [Optifabric 的未来以及推荐的替代品 (The future of Optifabric and Recommended alternatives)](https://gist.github.com/modmuss50/deff1658c4550ca8b16cb5d40ceaa468)
 - [Calloatti 的列表](https://gist.github.com/calloatti/6220c04e136d329298fd35066dfcc9b0)
