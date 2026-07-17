# scv-pine-script

SCV TradingView Pine Script — 选股系统三大成分：

| 成分 | 说明 | 文件 | 状态 |
|------|------|------|------|
| **S** — Stage | 以 150 均线判断 Stage 1~4 阶段 | `scripts/SCV_Stage.pine` | ✅ 完成 |
| **C** — Contraction | 收缩形态 | — | ⏳ 待写 |
| **V** — Volume | 交易量 | — | ⏳ 待写 |

## 使用方法

1. 打开 TradingView → Pine Editor
2. 复制 `scripts/SCV_Stage.pine` 的内容贴上
3. 点「Add to chart」

## Stage 规则摘要

- **Stage 1**：150均线趋平 · 横盘至少半年 · 交易量低迷 → 不交易
- **Stage 2**：150均线趋上 · 阳烛量放大 → 做多时期
- **Stage 3**：150均线趋平 · 阴烛量放大 · 跌穿150均线 → 不交易
- **Stage 4**：150均线趋下 → 做空时期

均线颜色：50均线 灰色 · 150均线 青色 · 200均线 红色
