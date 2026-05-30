# 小丑牌 — Claude 工作手册

## 项目定位

网页版小丑牌（Balatro 同人），纯前端单文件游戏，用 Vue 3 CDN + GSAP 实现，无构建流程。

## 目录结构

```
游戏/
├── index.html                          # 游戏主体（唯一可运行的入口）
├── 01-第1轮-PRD-小丑牌核心循环.html    # 产品需求文档
├── 01-第1轮-DESIGN-小丑牌核心循环.html # UI 设计规范
└── 小丑牌.png                          # 参考截图
```

## 常用操作

```bash
# 直接打开游戏
open index.html

# 本地静态服务（推荐，避免跨域问题）
npx serve .
```

## 开发约定

- 所有代码、模板、样式均写在 `index.html` 一个文件里，不拆分
- Vue 组件通过 `app.component(...)` 或 `setup()` 内联定义
- 样式写在 `<style>` 块，使用 CSS 变量（定义在 `:root`）管理主题色
- 动画优先用 GSAP，避免 CSS keyframe 与 Vue 过渡混用造成冲突
- 中文注释优先，保持与 PRD/DESIGN 文档的术语一致
