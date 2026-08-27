# agi-predictions

科技与金融预测仓库，当前聚焦 **AGI 推演**：AGI/ASI 时间线、起飞争论、AI 资本周期（泡沫）、中美 AI 竞赛。方法上向 LessWrong 预测文化看齐：概率显式、可证伪、按期校准。

## 目录地图

| 目录 | 内容 | 起点 |
|---|---|---|
| **lesswrong-ai-futurism/** | AGI 时间线与起飞话语研究：LW 圈内（时间线、起飞辩论、方法论、我方预测、作者图谱）+ LW 之外全景（实验室掌门人、学界调查、经济学争论、预测平台、政策、中国视角、泡沫框架） | [README](lesswrong-ai-futurism/README.md) |
| **ai-finance-bubble/** | AI 资本周期分析：12 个月泡沫情景推演（A/B/C=50/20/30）+ 5 篇事实清单（capex/债务/循环交易、估值/集中度、宏观/利率、能力/收入/采用、泡沫类比/触发器） | [ai-bubble-scenarios-2026-08.md](ai-finance-bubble/ai-bubble-scenarios-2026-08.md) |
| **ai-finance-bubble/periodic-watch/** | 宏观/信用观察（月度）：美债、利率、流动性——校准泡沫情景概率 | [2026-08-26 美债危机观察](ai-finance-bubble/periodic-watch/2026-08-26-us-debt-crisis-watch.md) |
| **timeline-watch/** | 能力/时间线观察（月度）：METR 基准、模型与收入、capex、预测市场——periodic-watch 的孪生刊 | [2026-08-27 首期](timeline-watch/2026-08-27-ai-timeline-watch.md) |
| **scenarios/** | 跨域整合推演：金融周期 × AGI 时间线的多年期情景 | [穿过泡沫的 AGI 路径 2027-2032](scenarios/agi-through-the-bubble-2027-2032.md) |
| **china-ai-race/** | 中美 AI 竞赛：算力/芯片、模型/生态、电力/政策/市场——用中文一手源补英文世界的盲区 | [README](china-ai-race/README.md) |
| **predictions/** | **预测登记簿**：全仓库概率的唯 一权威登记处，OUR/EXT/CHK 编号 + Brier 计分 + 季度校准协议 | [ledger.md](predictions/ledger.md) |

## 工作流

```
预测（scenarios / 04-my-forecasts）
   ↓ 登记
predictions/ledger.md（编号、概率、可证伪清算标准）
   ↓ 监测
timeline-watch/（能力侧） + periodic-watch/（宏观侧）—— 月度
   ↓ 校准
季度回顾（首季 2026-10）：结算 Brier → 巡检仪表盘 → 更新情景概率与 04 锚 → 修订历史
```

## 核心判断速览（2026-08-27 时点）

- **金融**：晚期泡沫、真实盈利、循环融资是阿喀琉斯之踵。情景 A 破裂 50%（窗口 2026-10 ~ 2027-03）；但 8/26 NVDA 财报大超预期，破裂信号首检未触发，证据结构暂偏 B/C（见 timeline-watch 首期）。
- **时间线**：自动化 AI 研究员中位 **2032-2033**（我方）；认真对待金融周期后条件化至 **2033-2034**（穿过泡沫情景）。社区聚合 ~2030-2031，超预 2047-2050。
- **中国**：扩散侧差距已收窄到月级（AI Index 2.7%），起源侧（前沿训练算力）仍差一个数量级；官方赌渗透率而非 AGI 时刻——这不参与"何时 AGI"的竞猜，却在压低全球 AI 供给曲线。
- **p(doom)**：我方 ~12%（介于主流 5-9% 与 LW 社区 20-40%）。

## 约定

- 所有预测性数字登记入 `predictions/ledger.md`，其他文档不单独维护概率。
- 数据标注来源与日期；低可信度来源显式标注；口径冲突并列呈现。
- 我方预测署名 GLM-5.3（研究代理）；季度校准回顾每年 10 月首周执行。
