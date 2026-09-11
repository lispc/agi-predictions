# agi-predictions

科技与金融预测仓库，当前聚焦 **AGI 推演与 AI 风险**：AGI/ASI 时间线、起飞争论、AI 资本周期（泡沫）、中美 AI 竞赛、AI×生物安全。方法上向 LessWrong 预测文化看齐：概率显式、可证伪、按期校准。

## 目录地图

| 目录 | 内容 | 起点 |
|---|---|---|
| **agi-timelines/** | AGI 时间线与起飞话语研究：LW 圈内（时间线、起飞辩论、方法论、我方预测、作者图谱）+ LW 之外全景（实验室掌门人、学界调查、经济学争论、预测平台、政策、中国视角、泡沫框架） | [README](agi-timelines/README.md) |
| **ai-finance-bubble/** | AI 资本周期分析：12 个月泡沫情景推演（A/B/C=50/20/30）+ 5 篇事实清单（capex/债务/循环交易、估值/集中度、宏观/利率、能力/收入/采用、泡沫类比/触发器） | [ai-bubble-scenarios-2026-08.md](ai-finance-bubble/ai-bubble-scenarios-2026-08.md) |
| **watch/** | 观察三刊：`capability/`（METR 基准、模型与收入、capex、预测市场，月度）+ `macro/`（美债、利率、流动性，月度）+ `bio/`（AI×生物安全，季度、2026-10 创刊）——互相校准泡沫情景与时间线概率 | [capability 首期 8/27](watch/capability/2026-08-27-ai-timeline-watch.md) ｜ [capability 第二期 9/9](watch/capability/2026-09-09-ai-timeline-watch.md) ｜ [macro 美债观察 8/26](watch/macro/2026-08-26-us-debt-crisis-watch.md) ｜ [Jackson Hole 重估 8/31](watch/macro/2026-08-31-jackson-hole-review.md) ｜ [macro 9 月刊 9/9](watch/macro/2026-09-09-september-macro-watch.md) |
| **scenarios/** | 跨域整合推演：金融周期 × AGI 时间线的多年期情景 | [穿过泡沫的 AGI 路径 2027-2032](scenarios/agi-through-the-bubble-2027-2032.md) |
| **china-ai-race/** | 中美 AI 竞赛：算力/芯片、模型/生态、电力/政策/市场——用中文一手源补英文世界的盲区 | [README](china-ai-race/README.md) |
| **ai-bio-risk/** | **AI 生物安全风险**：uplift 证据曲线（01）、实验室阈值框架触及史（02）、治理的美欧英国际中四轨（03）、威胁基率与自然疫情基线面（04）、我方预测与 p(doom) 生物通道分解（05）——与起飞叙事正交的灾难通道 | [README](ai-bio-risk/README.md) |
| **predictions/** | **预测登记簿**：全仓库概率的唯一权威登记处，OUR/EXT/CHK 编号 + Brier 计分 + 季度校准协议 | [ledger.md](predictions/ledger.md) |

## 工作流

```
预测（scenarios / 04-my-forecasts / ai-bio-risk 05）
   ↓ 登记
predictions/ledger.md（编号、概率、可证伪清算标准）
   ↓ 监测
watch/capability/（能力侧） + watch/macro/（宏观侧）—— 月度；watch/bio/（生物安全）—— 季度（2026-10 创刊）
   ↓ 校准
季度回顾（首季 2026-10）：结算 Brier → 巡检仪表盘（金融 CHK-001~019 + 生物 CHK-020~028）→ 更新情景概率与 04 锚 → 修订历史
```

## 核心判断速览（2026-09-09 时点）

- **金融**：晚期泡沫、真实盈利、循环融资是阿喀琉斯之踵。情景 A 破裂 **55%** / B 20% / C 25%（8/31 由 50/20/30 修订：8/28 Warsh Jackson Hole 首秀明确鹰派、9 月加息定价升至 ~60%，CHK-002 触发；NVDA 财报大超预期未触发破裂信号，但 8/28 单日 -4.6% 显示宏观压倒基本面）。破裂窗口 2026-10 ~ 2027-03 不变（见 [8/31 Jackson Hole 重估](watch/macro/2026-08-31-jackson-hole-review.md)）。9/9 快照：概率未动（无 CHK 新触发）；8 月非农上修推翻"就业负值"论据、油价反转 Brent ~$97、10Y 4.78% 创 52 周新高、30Y 抹平 Bessent 干预涨幅，下一节点 9/11 CPI → 9/16 FOMC（见 [9 月宏观观察](watch/macro/2026-09-09-september-macro-watch.md)）。
- **时间线**：自动化 AI 研究员中位 **2032-2033**（我方）；认真对待金融周期后条件化至 **2033-2034**（穿过泡沫情景）。社区聚合 ~2030-2031，超预 2047-2050。9/9 快照：GPT-6 Astra 发布（首个 Critical 网络级模型、攻克 ARC-AGI-3），Metaculus 弱 AGI 中位前移至 2027-10——我方锚不变，留待 10 月季度回顾（见 [capability 第二期](watch/capability/2026-09-09-ai-timeline-watch.md)）。
- **中国**：扩散侧差距已收窄到月级（AI Index 2.7%），起源侧（前沿训练算力）仍差一个数量级；官方赌渗透率而非 AGI 时刻——这不参与"何时 AGI"的竞猜，却在压低全球 AI 供给曲线。
- **生物安全（AI×bio，9/11 建库）**：uplift 任务级证据已实（VCT 超专家线、5 倍协议撰写）、端到端为零、历史基率"三连败"；p(doom) 12% 中生物通道 ≈2–3pp 且可在工具 AI 阶段兑现（与起飞正交，见 [ai-bio-risk/05](ai-bio-risk/05-forecasts.md)）。五年三情景：α 防线粘住 45% / β 灰色侵蚀 35% / γ 门槛击穿 20%；净倾斜取决于 DNA 合成筛查覆盖率 vs 自动化湿实验室扩散速度的赛跑。最重要近期清算锚：Anthropic 首次实测披露 ASL-4 级（我方 0.35 by 2027；Metaculus Q38589 中位 2027-07）。
- **p(doom)**：我方 ~12%（介于主流 5-9% 与 LW 社区 20-40%）；其中生物通道分解 ~2.5pp（OUR-056）。

## 约定

- 所有预测性数字登记入 `predictions/ledger.md`，其他文档不单独维护概率。
- 数据标注来源与日期；低可信度来源显式标注；口径冲突并列呈现。
- 我方预测署名 GLM-5.3（研究代理）；季度校准回顾每年 10 月首周执行。
