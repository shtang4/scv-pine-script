# scv-pine-script

SCV TradingView Pine Script — 选股系统三大成分：

| 成分 | 说明 | 文件 | 状态 |
|------|------|------|------|
| **SCV 合并版** | Stage + Contraction + Volume 一个指标全包（主图） | `scripts/SCV_All.pine` | ✅ 推荐使用 |
| **S** — Stage | 以 150 均线判断 Stage 1~4 阶段 | `scripts/SCV_Stage.pine` | ✅ 完成 |
| **C** — Contraction | VCP 式收缩形态 C1~C6、Base 突破、买点 | `scripts/SCV_Contraction.pine` | ✅ 完成 |
| **V** — Volume | 结构量能、突破放量、流动性、烛数加分（副图，含成交量柱） | `scripts/SCV_Volume.pine` | ✅ 完成 |

## 使用方法

1. 打开 TradingView → Pine Editor
2. 复制 `scripts/SCV_All.pine` 的内容贴上（或按需使用单独的 S / C / V 脚本）
3. 点「Add to chart」

> 合并版是主图指标，成交量直方图请开 TradingView 内建的成交量；
> 放量突破以K线上方圆点标记。想要带颜色的成交量柱可另外加载 `SCV_Volume.pine`。

## Stage 规则摘要

- **Stage 1**：150均线趋平 · 横盘至少半年 · 交易量低迷 → 不交易
- **Stage 2**：150均线趋上 · 阳烛量放大 → 做多时期
- **Stage 3**：150均线趋平 · 阴烛量放大 · 跌穿150均线 → 不交易
- **Stage 4**：150均线趋下 → 做空时期

均线颜色：50均线 灰色 · 150均线 青色 · 200均线 红色
