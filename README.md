
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

