---
layout: post
title: 1.10.2农业工艺（AgriCraft）教程——兼容性极高的IC2杂交继承者
tags: [wiki]
description: >
  JJN，开心不，惊喜不，意外不。我接坑了
---

> 农业工艺这个mod制作的初衷就是要继承并发展IC2那个十分有趣却兼容性极差的农业。在其诞生一年多后的今天来看，它已经很好地实现了这个目标。关于这个教程，最初我只想简单地写一下，为几天后另一个mod的教程做个铺垫。不过在仔细研究了几天后，我发现AgriCraft本身的可玩性、兼容性和自定义程度都十分地高，值得详细介绍一下。此教程的遗漏或是错误之处，欢迎指出。同时也欢迎各位整合包制作者利用AgriCraft高度的自定义性与兼容性做出有趣的农业向魔改整合。
>
> Author：原1.7.10中文教程作者`JJN`

使用版本：`Agricraft-2.0.0-0.11.0-a21`

## 一、简介

Agricraft（以下均简称AC）实际上早在去年11月就更新到了1.10.2，但是随后几乎再无更新且bug众多。经历了漫长的alpha时期后，`CodesCubesAndCrashes`终于接坑修复了里面的众多bug，在多个知名大型整合包测试后并将其发布了出来。至少稳定性上有了很大提升。

IC应该算是开创了农业杂交的先河，但是长久以来却不为人所熟知。兼容性差，而且又并不是独立模块。这或许是其独创而又不流行的原因之一。AC吸取了其优点，将其独立做成模块，2.0版本更进一步，直接舍弃原来硬编码的思想，全面采用Json格式配置文件来书写兼容，可谓是一代更比一代强。即使在其之前还未更新，bug众多的情况下，许多知名整合包仍然添加了这个模组，可见此模组地位之高。

通过AC的作物架，玩家可以任意杂交作物实现一些重要资源的获得，恰如其分的讲农业带入了Minecraft科技线发展中。当然，杂交本身是一个极为随机的过程，所以很多人也戏称这个模组叫做`非提工艺`。

## 二、联动mod介绍（基础篇）

> AC联动的mod数量众多，主要分为三类。第一类是辅助类的联动，第二类联动是支持许多mod的作物种在AC的作物架上并给部分作物添加杂交配方，第三类联动是支持一些mod对AC作物架上的作物自动收获（AC作物架和IC2的一样，收获时只会收获作物的产物，作物的种子仍然会种在作物架上）
>
> Author：原1.7.10中文教程作者`JJN`

### 1.辅助向模组

#### (1) JEI

首先要说的是JEI，在JEI中可以很容易地查到AC作物的杂交路线、种植条件和相应的产物。

![jei](https://public.lightpic.info/image/58F7_59F47C4D0.jpg)



#### (2) Hwyla 和 The One Probe

然后要说的是Hwyla和The One Probe，AC对Hwyla和The One Probe添加了支持，在Hwyla和The One Probe中可以直接看到AC作物的各项数据（即生长速度、产量和抗性，种子需要先分析过才能看到），也能看到作物生长状态和杂草的相关提示信息,如下图所示：

![hwyla](https://public.lightpic.info/image/A163_59F47BD40.jpg)

### 2.作物兼容

2.0以后提供的Json加载兼容方式摒弃了旧版本的硬编码，使得其理论上支持任何模组的作物种植。不过默认生成的几个配置文件仍然主动添加了几个模组的兼容。

#### (1)实用拓展(Actually Addition)

实用拓展的油菜，咖啡，亚麻，水稻可以种植在作物架上。

#### (2)神秘农业(Mysticalagriculture)及其附属模组

包括Mysticalagriculture，Mysticalagriculture Addition，Mysticalagriculture Expansion在内的所有作物。

#### (3)潘马斯的丰收工艺(Harvestcraft)

基本上支持所有种子种植在作物架上。

#### (4)植物魔法(Botania)

需种在灰化土上，收获时得到相应的神秘花瓣。也添加了杂交出它们的配方.

####(5)沉浸工程(ImmersiveEngineering)

IE的工业大麻可以种植。

#### (6)自然(Natura)

支持自然模组的大麦和棉花。



没了，其他变化不大。