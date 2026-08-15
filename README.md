# Logarithmic Spiral Quadrilateral Cell Calculator

An interactive browser-based calculator and visualizer for strict four-point logarithmic spiral quadrilateral cells.

## Features

- Live calculation from the initial radius `r₀`, growth factor `k`, cell count `N`, cell angle `Δθ`, and width ratio `λ`.
- Strict four-point Euclidean geometry for every quadrilateral cell.
- Selected-cell edge lengths, angle range, and point coordinates.
- Interactive 2D preview:
  - Drag a blank area to rotate.
  - Scroll to zoom.
  - Hold `Space` and drag to pan.
- DXF export for Fusion 360 sketch insertion.
  - ASCII DXF R14 / `AC1014` format.
  - 2D `LWPOLYLINE` entities.
  - Standard DXF tables and model/paper-space block records.
  - Layers: `0`, `INNER`, `OUTER`, and `CONNECTORS`.
  - Exported files use the suffix `fusion-r14-complete`.

## Geometry model

The radial profile is:

```text
r(θ) = r₀ exp(kθ)
R(θ) = (1 + λ) r(θ)
```

The width scale is self-similar:

```text
Wᵢ = λ rᵢ
```

Each cell is defined by four Euclidean points: inner start, inner end, outer end, and outer start.

## Files

- `logarithmic-spiral-calculator-en.html` — English version.
- `logarithmic-spiral-calculator-zh-CN.html` — Simplified Chinese version.
- `README.md` — English documentation.
- `README.zh-CN.md` — Simplified Chinese documentation.

## Run locally

Open either HTML file directly in a modern browser, or serve the folder with any static HTTP server.

## Fusion 360 workflow

1. Open the calculator and set the parameters.
2. Click **Export DXF (Fusion 360 Sketch)**.
3. Download the file whose name contains `fusion-r14-complete`.
4. In Fusion 360, choose **Design → Insert → Insert DXF**.
5. Select a sketch plane and choose the newly exported DXF file.

## GitHub Pages

To publish one language version as the default page, rename it to `index.html`, upload it to the repository root, and configure GitHub Pages to deploy from the `main` branch and the root folder.

The site is static and does not require a build step or external dependencies.

## License

Add the license that matches your project before public distribution.

---

# 对数螺旋四边形单元计算器

这是一个用于严格四点对数螺旋四边形单元的交互式浏览器计算器与可视化工具。

## 功能

- 根据初始半径 `r₀`、增长因子 `k`、单元数量 `N`、单元角度 `Δθ` 和宽度比例 `λ` 实时计算。
- 使用严格四点欧氏几何构造每个四边形单元。
- 显示选中单元的边长、角度范围和点坐标。
- 结构预览支持：
  - 拖拽空白处旋转。
  - 滚轮缩放。
  - 按住 `Space` 并拖拽进行平移。
- 导出可用于 Fusion 360 草图插入的 DXF 文件。
  - ASCII DXF R14 / `AC1014` 格式。
  - 二维 `LWPOLYLINE` 实体。
  - 包含标准 DXF 表以及模型空间/图纸空间块记录。
  - 图层：`0`、`INNER`、`OUTER` 和 `CONNECTORS`。
  - 导出文件名包含 `fusion-r14-complete`。

## 几何模型

径向函数为：

```text
r(θ) = r₀ exp(kθ)
R(θ) = (1 + λ) r(θ)
```

宽度采用自相似比例：

```text
Wᵢ = λ rᵢ
```

每个单元由四个欧氏点定义：内侧起点、内侧终点、外侧终点和外侧起点。

## 文件

- `logarithmic-spiral-calculator-en.html` — 英文版本。
- `logarithmic-spiral-calculator-zh-CN.html` — 简体中文版本。
- `README.md` — 英文说明。
- `README.zh-CN.md` — 简体中文说明。

## 本地运行

可以直接使用现代浏览器打开任意一个 HTML 文件，也可以使用任意静态 HTTP 服务器运行该文件夹。

## Fusion 360 使用流程

1. 打开计算器并设置参数。
2. 点击 **导出 DXF（Fusion 360 草图）**。
3. 下载文件名中包含 `fusion-r14-complete` 的文件。
4. 在 Fusion 360 中选择 **Design → Insert → Insert DXF**。
5. 选择草图平面，再选择刚刚导出的 DXF 文件。

## GitHub Pages

如果要将某个语言版本作为默认页面发布，请将它重命名为 `index.html`，上传到仓库根目录，然后将 GitHub Pages 设置为从 `main` 分支的根目录发布。

该网站是纯静态页面，不需要构建步骤，也不依赖外部软件包。

## 许可证

在公开发布前，请补充与你的项目相匹配的许可证。
