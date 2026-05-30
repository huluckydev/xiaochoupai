# 小丑牌

基于 [Balatro](https://www.playbalatro.com/) 玩法的网页版卡牌游戏，使用纯 HTML 单文件实现，无需构建工具。

## 技术栈

- **Vue 3**（CDN）：响应式 UI
- **GSAP 3**：动画效果
- **Google Fonts**：Press Start 2P / VT323 / Inter 字体

## 安装与运行

无需安装任何依赖，直接用浏览器打开即可：

```bash
open index.html
```

或在本地起一个静态服务器（避免部分浏览器的跨域限制）：

```bash
npx serve .
# 访问 http://localhost:3000
```

## 文件说明

| 文件 | 说明 |
|------|------|
| `index.html` | 游戏主体，包含全部逻辑、样式和模板 |
| `01-第1轮-PRD-小丑牌核心循环.html` | 产品需求文档 |
| `01-第1轮-DESIGN-小丑牌核心循环.html` | UI 设计规范文档 |
| `小丑牌.png` | 游戏参考截图 |
