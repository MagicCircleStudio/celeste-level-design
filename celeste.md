## 活动介绍
- 本次活动的主题是复刻或设计《蔚蓝》(*《celeste》*)中的关卡
  >《蔚蓝》是由开发商Matt Makes Games Inc.开发的一款平台跳跃游戏，获得了TGA2018年度最佳独立游戏奖项。平台跳跃类是一种有着悠久历史和广大受众的游戏类型，最出名的游戏系列有《超级马里奥》系列等。

- 我们提供一个包含基本要素的演示项目: [演示项目下载地址](github.com/mixandjam/Celeste-Movement)

- 设计的目标，借助已有的演示项目:
  - 实现一个有着完整起始、终止的关卡
  - 有着完整的成功、失败判定
  - 未提供的美术资源、关卡设计所需的含有各种功能的平台等，需要个人解决
- 可供参考的学习资源：
  - Celeste部分源码: [Madeline移动源码](github.com/NoelFB/Celeste)
  - 与演示项目相对应的视频教程(可能需要科学上网): [Mix And Jam (Youtube)](youtu.be/STyY26a_dPY)

---
## 《蔚蓝》游戏介绍与设计思路：
### a. 主角的移动特性：
- 在空中或者地面上可以八方向冲刺一次，脚踩到地面上时恢复冲刺次数；
- 靠近墙壁时：
  - 可以抓取，悬停在墙壁上；
  - 可以抓取后上爬；可以以墙作为弹跳点跳跃一次。
  - 其中抓取和上爬都是要消耗体力的，消耗完之后就不能抓取了，强制沿墙壁滑下；但是体力消耗完后仍可以以墙作为弹跳点跳跃

### b. 关卡设计tips：
  利用主角的移动特性:
  - 利用冲刺技能，设计两个平台，其间的距离无法用普通跳跃跨过:<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/1.gif)
  - 最简单的利用抓取上爬:<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/2.gif)
  - 最简单的利用弹墙跳，设计两个相对的墙壁：<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/3.gif)
  - 空中可以捡到的恢复角色冲刺的道具：<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/4.gif)
  - 组合以上几种: <br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/5.gif)

  一般的平台跳跃类游戏：
  - 根据时间往返移动的平台：<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/6.gif)
  - 在空中改变角色动量的方块：<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/7.gif)
  - 角色触碰便会死亡的方块：<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/8.gif)
  - 角色触碰便会移动的方块：<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/9.gif)
  - 角色站立后过一段时间会消失的方块：<br>
  ![image](https://github.com/MagicCircleStudio/celeste-level-design/blob/master/gifs/10.gif)

事实上，仅仅组合以上元素已经可以设计出相当有趣味性的关卡了，在此贴上蔚蓝中某一关的通关视频 [蔚蓝1c](https://www.bilibili.com/video/BV1a7411g7Ci) 作为参考，当然，更好的方式是购买游戏在游戏中体会关卡设计的精妙，并运用于自己的实践之中。

---
### c. 个人意见：
我个人认为，设计关卡的核心思想，不仅是要组合多种元素进行设计，更是要让玩家需要思考如何分配自己的跳跃、冲刺和体力资源来通过这个关卡（类似于解谜），并且在玩家通关的过程中，可以通过限制玩家的“休息时间”（即玩家在通过整关之时，中间可以停留的时间，例如完全不留可以站立的平台，参考设计实例1），来提升玩家在通过关卡后的成就感。**当然，难度设计要合理。**


