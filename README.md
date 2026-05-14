# Personal UI Portfolio

极简科技风个人作品展示页面，黑色底色搭配淡蓝色点缀，内置动态粒子背景与鼠标交互效果。

## 功能特性

- **动态粒子背景** — 全屏霓虹多彩粒子系统，粒子间自动连线形成网状结构
- **鼠标涟漪交互** — 光标周围粒子消退并产生波浪起伏，附带旋转光环与扩散波纹
- **毛玻璃卡片** — 各内容板块采用 `backdrop-filter` 玻璃拟态效果，层次分明
- **技能展示** — 分类标签云 + 淡蓝发光进度条
- **项目作品** — 响应式卡片网格，悬停上浮高亮
- **平滑滚动** — 导航栏点击锚点平滑跳转，滚动渐入动画
- **自适应布局** — 桌面三列 / 平板两列 / 手机单列

## 技术栈

纯原生实现，无任何框架或依赖：

- HTML5 Canvas 粒子引擎
- CSS3 变量 + Flexbox + Grid + backdrop-filter
- Intersection Observer API（滚动动画）
- requestAnimationFrame（60fps 粒子渲染）

## 使用方法

直接在浏览器中打开 `index.html` 即可预览。

```
git clone https://github.com/Permanent-cpu/UI.git
cd UI
# 用浏览器打开 index.html
```

## 自定义内容

编辑 `index.html`，搜索以下关键词快速定位占位内容：

| 关键词 | 对应内容 |
|--------|----------|
| `Permanent0307` | 姓名 |
| `嵌入式开发者` | 个人标语 |
| `skill-tag` | 技能标签 |
| `data-width` | 技能熟练度百分比 |
| `project-name` | 项目名称 |
| `project-desc` | 项目描述 |
| `project-tag` | 项目技术标签 |
| `permanent0307@163.com` | 联系邮箱 |
| `github.com/Permanent-cpu` | GitHub 链接 |
| `linkedin.com/in/your-profile` | LinkedIn 链接 |
| `twitter.com/your-handle` | Twitter 链接 |

粒子效果参数位于 `<script>` 顶部常量区，可调整：

- `GRID_SPACING` — 粒子密度
- `INNER_RADIUS` / `MID_RADIUS` / `OUTER_RADIUS` — 鼠标交互范围
- `ORBIT_RADIUS` — 光标光环轨道半径
- `PALETTE` — 粒子颜色调色板

## 项目结构

```
UI/
└── index.html    # 全部 HTML / CSS / JS
```

## 浏览器支持

所有现代浏览器（Chrome / Firefox / Safari / Edge）。

## License

MIT
