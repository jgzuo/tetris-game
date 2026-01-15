# 🎮 Tetris - 俄罗斯方块

一个功能完整、界面精美的俄罗斯方块网页游戏，采用淡雅风格设计。

![Tetris Game](https://img.shields.io/badge/Game-Tetris-blue?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)

## ✨ 特性

- 🎯 **完整的游戏功能**：7种标准方块、旋转、碰撞检测、行消除
- 📊 **计分系统**：根据消除行数和等级计算得分
- 📈 **等级系统**：每消除10行升一级，速度递增
- 👀 **下一个方块预览**：提前查看即将出现的方块
- ⏸️ **暂停/继续**：随时暂停游戏
- 🎨 **精美界面**：淡雅配色方案，响应式设计
- ⌨️ **键盘控制**：支持多种快捷键操作
- 📱 **单文件**：无需依赖，直接在浏览器中运行

## 🎮 游戏操作

| 按键 | 功能 |
|------|------|
| ← | 左移方块 |
| → | 右移方块 |
| ↑ | 旋转方块 |
| ↓ | 加速下落 |
| Space | 直接落地 |
| P | 暂停/继续游戏 |
| R | 重新开始 |

## 📊 计分规则

- **消除行数**：
  - 1行：100 × 等级
  - 2行：300 × 等级
  - 3行：500 × 等级
  - 4行：800 × 等级
- **软降**（加速下落）：每格 1 分
- **硬降**（直接落地）：每格 2 分

## 🎯 等级系统

- 每消除 **10 行** 升一级
- 每升一级，下落速度加快 100ms
- 最高速度限制为 100ms

## 🎨 游戏界面

### 设计特点

- **淡雅配色**：采用柔和的马卡龙色系
- **白色背景**：简洁清爽的视觉体验
- **渐变设计**：微妙的渐变效果增强美感
- **圆角卡片**：现代化的 UI 设计风格
- **响应式布局**：适配不同屏幕尺寸

### 方块颜色

| 方块 | 颜色 | 代码 |
|------|------|------|
| I | 青蓝色 | #a8dadc |
| O | 米白色 | #f1faee |
| T | 淡紫色 | #cdb4db |
| S | 天蓝色 | #bde0fe |
| Z | 粉红色 | #ffc8dd |
| J | 浅蓝色 | #a2d2ff |
| L | 杏色 | #ffcdb2 |

## 🚀 快速开始

### 在线游玩

访问游戏页面：**[https://jgzuo.github.io/tetris-game/](https://jgzuo.github.io/tetris-game/)**

### 本地运行

1. 克隆或下载此仓库
2. 用浏览器打开 `tetris.html` 文件
3. 开始游戏！

```bash
# 克隆仓库
git clone https://github.com/jgzuo/tetris-game.git

# 进入目录
cd tetris-game

# 在浏览器中打开
open tetris.html  # macOS
# 或双击 tetris.html 文件
```

## 🛠️ 技术栈

- **HTML5 Canvas**：游戏渲染
- **Vanilla JavaScript**：游戏逻辑
- **CSS3**：界面样式和动画
- **无依赖**：纯原生实现，无需框架或库

## 📁 项目结构

```
tetris-game/
├── tetris.html    # 主游戏文件（包含所有代码）
└── README.md      # 项目说明文档
```

## 🔧 游戏机制

### 方块定义

游戏包含 7 种标准俄罗斯方块（tetrominoes）：

- **I 型**：4格直线
- **O 型**：2×2 正方形
- **T 型**：T 形状
- **S 型**：S 形状
- **Z 型**：Z 形状
- **J 型**：J 形状
- **L 型**：L 形状

### 核心功能

- **Wall Kick**：旋转时自动调整位置
- **碰撞检测**：精确的边界和方块检测
- **行消除**：自动检测并消除完整的行
- **游戏结束**：方块堆叠到顶部时结束

## 📝 开发说明

### 修改游戏参数

在 `tetris.html` 中可以调整以下参数：

```javascript
const COLS = 10;          // 游戏板列数
const ROWS = 20;          // 游戏板行数
const BLOCK_SIZE = 30;    // 方块大小（像素）
const gameSpeed = 1000;   // 初始下落速度（毫秒）
```

### 自定义配色

修改 `COLORS` 对象来自定义方块颜色：

```javascript
const COLORS = {
    I: '#a8dadc',
    O: '#f1faee',
    // ... 其他颜色
};
```

## 🎯 游戏技巧

1. **计划 ahead**：查看下一个方块预览，提前规划
2. **保持底部平整**：便于放置后续方块
3. **优先消除多行**：4行消除得分最高
4. **利用墙壁**：在边缘旋转可以节省空间
5. **保持冷静**：速度会逐渐加快，保持节奏

## 📈 未来改进

- [ ] 添加排行榜功能
- [ ] 支持触摸操作（移动端）
- [ ] 添加音效和背景音乐
- [ ] 实现保存/加载游戏
- [ ] 添加主题切换功能
- [ ]多人对战模式

## 📄 License

本项目采用 [MIT License](LICENSE) 开源协议。

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📮 联系方式

- GitHub：[@jgzuo](https://github.com/jgzuo)
- 游戏链接：[https://jgzuo.github.io/tetris-game/](https://jgzuo.github.io/tetris-game/)

## 🙏 致谢

- 经典的 Tetris 游戏设计
- 所有为开源社区做出贡献的开发者

---

**享受游戏！🎮**

如果喜欢这个项目，请给一个 ⭐ Star！
