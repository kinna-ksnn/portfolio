# Minecraft 终极攻略 · 交互式网页

在线地址：https://kinna-ksnn.github.io/portfolio/

## 技术亮点

- **材质弹簧动画系统** — 6 种 MC 方块纹理对应 6 套物理弹簧参数（草方块、石头、下界岩、末地石、黑曜石、木板），GSAP + ScrollTrigger 驱动，每个区块的弹性体感与纹理材质一致
- **MC 原版音效** — 从游戏资产提取 10 个 .ogg 音效文件，HTMLAudioElement 池化播放，file:// 协议兼容，带静音开关
- **像素粒子引擎** — Canvas 覆盖层绘制 4px 像素方块，点击爆开、hover 火花上浮，重力衰减，颜色跟随材质
- **像素风设计系统** — 38 个 CSS 变量、物品栏风格边框 (beveled borders)、16×16 纹理背景、Minecraftia 像素字体
- **响应式布局** — 侧边栏折叠、快捷栏缩放、打印样式
- **零依赖** — 除 GSAP CDN 外无外部框架，纯手写 CSS + JS

## 功能模块

| 模块 | 内容 |
|------|------|
| 通关路线图 | 木→石→炎→眼→龙→翼 进度条 + 阶段耗时表 |
| 生存入门 | 第一天时间线、工具链合成、食物排名、庇护所方案 |
| 采矿时代 | 鱼骨挖矿法、9 种矿石分布高度表、附魔系统、盔甲进阶 |
| 下界指南 | 传送门搭建、生存法则、药水酿造配方表 |
| 末地攻略 | 要塞定位、末影龙 BOSS 战四阶段、鞘翅与潜影盒 |
| 战斗系统 | 11 种怪物对策表、4 大 BOSS 攻略 + 召唤方法 |
| 视频嵌入 | 4 个 B站 iframe，带封面图 + 悬停播放提示 |
| 搜索系统 | 实时关键词高亮 + 章节匹配计数，Ctrl+K 快捷键 |

## 文件结构

```
portfolio/
├── index.html          # 主页面 (≈75KB, 单文件)
├── mc-textures/        # 28 个 64×64 PNG 纹理
│   ├── stone.png
│   ├── grass_block_side.png
│   ├── diamond_ore.png
│   └── ...
├── mc-sounds/          # 10 个 MC 原版 .ogg 音效
│   ├── random/click.ogg
│   ├── note/pling.ogg
│   └── ...
└── README.md
```

## 部署

GitHub Pages，`master` 分支自动构建。
