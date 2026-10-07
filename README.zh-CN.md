# Happy Collector: 20-Level Three.js Browser Platformer

<p align="center">
  <img src="assets/readme/happy-collector-banner.png" alt="Happy Collector" width="100%">
</p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.ar.md">العربية</a> ·
  <a href="README.fr.md">Français</a> ·
  <a href="README.zh-CN.md">简体中文</a>
</p>

**Play:** https://kids-happy-collector.vercel.app/  
**Itch.io:** https://joenasr.itch.io/happy-collector

## 简体中文

**Happy Collector** 是一款使用 Three.js 制作、可直接在浏览器中游玩的 20 关 3D 平台游戏。它作为阿联酋儿童多游戏互动寓教于乐活动中的一个游戏模块开发。

玩家控制一个微笑的黄色方块，在漂浮的平台路线中前进。黄色方块代表积极情绪与品质；移动的红色敌人代表消极情绪与行为。收集黄色方块获得分数，避开或从上方踩掉红色敌人，通过平台机关并到达关卡终点的门，即可进入下一关。

## 玩法

- 收集黄色方块：**+10 分**
- 下落时从上方踩掉红色敌人：**+5 分**
- 碰到红色敌人或跌出路线会失去一条生命
- 每局开始时有 **3 条生命**
- 失去一条生命后会重新开始当前关卡，并保留剩余生命
- 完成关卡**不要求**收集全部黄色方块
- 到达关卡终点的门即可进入下一关
- 完成第 20 关后显示 **MASTER COLLECTOR!**

黄色方块使用 **BRAVERY, JOY, LOVE, HOPE, PEACE, KINDNESS, CALM, PRIDE, TRUST, HAPPINESS**。红色敌人使用 **ANGER, GREED, JEALOUSY, RUDENESS, ENVY, HATE, DESPAIR**。

## 操作

**电脑：** `A / D` 或左右方向键移动；`W`、空格键或上方向键跳跃；开始移动后可使用鼠标滚轮缩放。  
**手机：** 使用屏幕上的左右移动与跳跃按钮；开始移动后可双指缩放。

## 游戏系统

游戏包含水平和垂直移动平台、摆动平台、弧形桥与绳桥平台序列、按钮控制的闸门、按钮升起的台阶、玻璃平台，以及可从上方踩掉的巡逻红色敌人。玻璃平台在玩家站上去时会裂开，在玩家停留期间保持实体，离开后会坠落并淡出。游戏还包含不同的天空环境、音乐、声音和视觉反馈，以及在支持设备上的震动反馈。

## 关卡架构

全部 20 个关卡都由运行时的确定性蓝图生成器使用可复用的平台和障碍元素构建。第 11–20 关包含在代码中明确设计的高层级序列。

## 实现

完整游戏及运行逻辑位于 `index.html`，Three.js r128 使用本地文件加载，并包含本地音乐、音频、字体和关卡/QA 文档。游戏运行不依赖 CDN 加载 Three.js。

## 项目背景

Happy Collector 作为阿联酋儿童多游戏互动寓教于乐活动中的一个游戏模块开发。

活动制作：[Peach Society](https://peach-society.com/)。

## 许可

该仓库目前没有声明覆盖整个项目的许可证。仓库中的 Three.js 许可证仅适用于 Three.js，不应被理解为自动许可 Happy Collector 的游戏代码、图形、音频、字体或其他项目资源。
