# hexo-theme-even

> fork from <https://github.com/ahonn/hexo-theme-even/>

A super simple theme for Hexo.

For more options, check out the [document](https://github.com/ahonn/hexo-theme-even/wiki)

## 与 upstream 的差异记录

### 个性化视觉定制（`source/css/_custom/_custom.scss`）

- **2019-11-30** — polymer logo（`#polymer`）、miracle-point 呼吸动画（`#miracle-point`）、taiji 悬停旋转（`.taiji`）
- **2024-01-20** — 背景斜角装饰（`#main:before / #main:after`）

### 滚动进度条

- **2019-11-30** — `_header.scss` 新增 `.scrollPercentage` 顶部固定进度条样式；`even.js` 新增滚动百分比计算逻辑

### 页脚动效（`_footer/_copyright.scss`）

- **2019-11-30** — heart 图标跳动动画；新增 `.netlify-link` 主题色样式

### 样式微调

| 文件 | 改动 | 时间 |
|------|------|------|
| `_base.scss` | 注释掉顶部 3px 主题色 border | 2019-11-30 |
| `_back-to-top.scss` | 位置从固定 px 改为 `5%`，移动端不再强制隐藏 | 2019-11-30 |
| `_post/_code.scss` | padding 从 `7px` 改为 `2px 7px` | 2019-12-01 |
| `_post/_content.scss` | 注释掉表格 double border | 2019-12-01 |
| `_mobile.scss` | 注释掉 mobile 导航 `margin-top: 2px` | 2019-11-30 |

### 工程改动

- **2021-03-09** — 新增 `bootstrap.js` 自定义初始化文件（`Even.visits()` 调用）
- **2023-09-23** — 删除 `.github/workflows/pages.yml` CI 工作流
- **2023-10-10** — swig 模板全部转换为 ejs
- **2026-06-16** — npm 依赖升级（audit fix）

## Installation

```shell
npm install hexo-renderer-ejs hexo-renderer-dartsass --save
git clone https://github.com/zeed-w-beez/hexo-theme-even themes/even
cp themes/even/_config.yml.example themes/even/_config.yml
```

Modify `yoursite/_config.yml`:

```yaml
# Extensions
## Plugins: http://hexo.io/plugins/
## Themes: http://hexo.io/themes/
theme: even
```
