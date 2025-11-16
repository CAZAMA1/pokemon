# 就决定是你了，皮卡丘！

这是一个用来练习前端技能的简单静态网页示例，展示了一个基于 Vue 2 的迷你 Pokémon（神奇宝贝）队伍选择界面。

## 项目概览

- 文件：`index.html`
- 主要功能：显示 6 只 Pokémon，可以随机生成新队伍，选择某一只会高亮并显示动画效果与血量条。
- 主要技术：纯静态页面，使用 Vue 2（通过 CDN）、原生 HTML/CSS、少量内联 JS。
- 资源：部分样式和字体来自 CDN（Normalize.css、Google Fonts），精灵图使用外部图片 CDN（pokemondb）。

## 主要特性

- 支持显示 Pokémon 名称、等级、性别、血量条、特殊效果（心形、糖果等）。
- 点击某只 Pokémon 会高亮并显示箭头与动画。
- `New Team` 按钮会随机生成一个新的 6 人队伍（从内置名单中随机选取）。

## 如何运行

打开项目根目录中的 `index.html`：
在资源管理器中双击 `index.html`，用浏览器打开。

## 开发说明

- 代码集中在 `index.html`，包含内联的样式和脚本，主要组件为 Vue 组件：`Arrow`、`Bg`、`Pokeball`、`Male`、`Female`、`Pokemon`、`List`。
- 数据源：页面顶部通过 `window.pokemon`、`window.alolan`、`window.candies` 和 `window.team` 定义示例数据。
- 精灵图 URL 规则：组件中将 Pokémon 名称小写后拼接到 `https://img.pokemondb.net/sprites/lets-go-pikachu-eevee/normal/{name}.png`（alolan 会加后缀 `-alolan`）。

## 已知限制

- 页面依赖外部 CDN（字体、normalize.css、Vue、精灵图），在离线或被限制的网络环境下部分资源可能不可用。

## 许可证 & 鸣谢

此代码为个人练习示例。你可以自由修改并用于学习或演示。若要公开分发或用于商业用途，请检查第三方资源（图像/字体）的使用许可。
感谢 Pokémon 社区提供的资源与灵感！
