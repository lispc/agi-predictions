# agi-predictions

科技与金融预测仓库，当前聚焦 **AGI 推演与 AI 风险**：AGI/ASI 时间线、起飞争论、AI 资本周期（泡沫）、中美 AI 竞赛、AI×生物安全。方法上向 LessWrong 预测文化看齐：概率显式、可证伪、按期校准。

## 目录地图

| 目录 | 内容 | 起点 |
|---|---|---|
| **agi-timelines/** | AGI 时间线与起飞话语研究：LW 圈内（时间线、起飞辩论、方法论、我方预测、作者图谱）+ LW 之外全景（实验室掌门人、学界调查、经济学争论、预测平台、政策、中国视角、泡沫框架）+ 信源索引（08：watch/季度校准的输入清单） | [README](agi-timelines/README.md) |
| **ai-finance-bubble/** | AI 资本周期分析：泡沫情景推演主报告（长期维护，概率镜像 ledger OUR-025–027）+ `raw-reports/` 下 5 篇事实底稿（2026-08-21 冻结快照）+ `crash-dynamics/` 破灭动力学系列（2000 科网 / 2008 次贷解剖、急性破裂一般规律含中国 2015、AI 泡沫编年史虚构推演）+ `debt-web/` 债务结构深挖（总量三层图、到期墙、或有担保法律强度、最终持有人图谱、抵押品回收率、私募信贷估值纪律、传染路径图与债务仪表盘） | [ai-bubble-scenarios.md](ai-finance-bubble/ai-bubble-scenarios.md) |
| **watch/** | 观察三刊：`capability/`（METR 基准、模型与收入、capex、预测市场，月度）+ `macro/`（美债、利率、流动性，月度）+ `bio/`（AI×生物安全，季度、2026-10 创刊）——互相校准泡沫情景与时间线概率 | [capability 首期 8/27](watch/capability/2026-08-27-ai-timeline-watch.md) ｜ [capability 第二期 9/9](watch/capability/2026-09-09-ai-timeline-watch.md) ｜ [macro 美债观察 8/26](watch/macro/2026-08-26-us-debt-crisis-watch.md) ｜ [Jackson Hole 重估 8/31](watch/macro/2026-08-31-jackson-hole-review.md) ｜ [macro 9 月刊 9/9](watch/macro/2026-09-09-september-macro-watch.md) ｜ [FOMC 加息重估 9/17](watch/macro/2026-09-17-fomc-hike-review.md) ｜ [暂停争论事件笔记 9/17](watch/capability/2026-09-17-pause-debate-note.md) ｜ [预测者战绩审计 9/28](watch/capability/2026-09-28-forecaster-track-record.md) ｜ [季度回顾·宏观 10/1](watch/macro/2026-10-01-quarterly-review-macro.md) ｜ [bio 创刊号 10/1](watch/bio/2026-10-01-bio-watch-01.md) ｜ [macro 信用双触发事件刊 10/20](watch/macro/2026-10-20-credit-triggers-review.md) ｜ [capability 期中更新 10/20](watch/capability/2026-10-20-ai-timeline-watch.md) ｜ [macro "AI is on trial" 事件刊 10/23](watch/macro/2026-10-23-ai-on-trial-review.md) ｜ [macro Anthropic S-1 事件刊 10/27](watch/macro/2026-10-27-anthropic-s1-ipo.md) |
| **scenarios/** | 跨域整合推演：金融周期 × AGI 时间线的多年期情景 | [穿过泡沫的 AGI 路径 2027-2032](scenarios/agi-through-the-bubble-2027-2032.md) |
| **china-ai-race/** | 中美 AI 竞赛：算力/芯片、EUV 光刻、模型/生态、电力/政策/市场——用中文一手源补英文世界的盲区 | [README](china-ai-race/README.md) |
| **ai-bio-risk/** | **AI 生物安全风险**：uplift 证据曲线（01）、实验室阈值框架触及史（02）、治理的美欧英国际中四轨（03）、威胁基率与自然疫情基线面（04）、我方预测与 p(doom) 生物通道分解（05）——与起飞叙事正交的灾难通道 | [README](ai-bio-risk/README.md) |
| **predictions/** | **预测登记簿**：全仓库概率的唯一权威登记处，OUR/EXT/CHK 编号 + Brier 计分 + 季度校准协议；2026-09-26 起为主簿（规则＋修订历史）＋agi/finance/bio 三分簿 | [ledger.md](predictions/ledger.md) |

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

## 核心判断速览（2026-09-17 时点，金融行 2026-10-27 / 时间线行 2026-10-20 更新）

- **金融**：晚期泡沫、真实盈利、循环融资是阿喀琉斯之踵。情景 A 破裂 **80%** / B 5% / C 15%（2026-10-20 事件性修订，规则强制：信用侧双触发同日确认——Oracle 5Y CDS **288bp**〔10-15，S&P Global 经 AP，CHK-030〕＋ CoreWeave 公开债 **79.15c** 最后成交〔Reuters 10-15〕/欧元 2032 债 **77.24c**〔CHK-031〕，+5pp/触发×2，原 70/10/20；依据见 ledger-finance OUR-025–027、主簿 §4.3 与 [10-20 信用触发重估](watch/macro/2026-10-20-credit-triggers-review.md)）。**10-23 维持不动**（无新触发；见 [10-23 "AI is on trial" 事件刊](watch/macro/2026-10-23-ai-on-trial-review.md)）：10-22 AI 抛售日（SOX -6.72% 自高点 -26%、Meta -7% FCF 十余年首负、CRWV 年内最低收盘 $55.60），但 SPX 距高点仅 -1.96%、宽度健康；**10Y 避险跌破 5%（2023 年银行危机以来最大单日降幅）——连续 >5% 定格恰好 20 个交易日，OUR-039 前置①擦线达成后被打破（前置②未达成，钩子未触发）；相位切换：利率冲击腿→增长恐慌腿**。传导确认仍缺 HY OAS >4%（10-21 收 3.27%）。下一判决点：MSFT/GOOGL/AMZN 财报（10-27~29，CHK-004）、FOMC（10-28）、CHK-034 两周零定价判决（~11-02，HY 一级已"实质冻结至中选后"）、中选（11-03）、Anthropic 定价（11-09 当周）、CoreWeave Q3（~11-11）。**10-27 维持不动**（无新触发；见 [10-27 Anthropic S-1 事件刊](watch/macro/2026-10-27-anthropic-s1-ipo.md)）：**S-1 于 10-26 挂出 EDGAR**——H1 收入 $16.3B（+1,300%）、Q2 单季经营利润 +$974M（六季度来首盈，OUR-035 钩子方向首个证据点）vs 具名算力承诺 ~$637B（MSFT"无论实际用量"、~80% take-or-pay）、9M 收入 5–7% 来自违规用量自披露；CHK-007 进入定价阶段但未触发（区间空白、chatter $1.8–2T＞$1.4T 阈值、Polymarket 11 月挂牌 62.2%）；盘面 10-23 SPX 较基期转负 → 10-26 +0.70% 反弹（S-1 乐观＋油价回落）但连续三日收 50 日线下方；HY 3.40%（10-22 跳宽）→3.38%（仍 <4%）；10Y 回 5.00%（相位切换未确认）。下一判决点：GOOGL/MSFT 盘后（10-27/28）、FOMC（10-28）、GDP+PCE（10-29）、CHK-034（~11-02）、中选（11-03）、Anthropic 定价（11-09 当周）。
- **时间线**：自动化 AI 研究员中位 **2032-2033**（我方）；认真对待金融周期后条件化至 **2033-2034**（穿过泡沫情景）。社区聚合 ~2030-2031，超预 2047-2050。10/1 季度回顾：OUR-009（2027 前）0.25→**0.10**（Astra 因对齐失败取消发布＋METR 空窗 9 月）、OUR-004（2030 前）0.25→**0.35**（Kalshi by-2028 一月 26.5%→44%、by-2030 →63.9%；OpenAI ARR ~$70B 两月 +75%）——单调性张力裁决消解，中位锚不变（见主簿 §4.3 10-01 行）。10/20 期中更新（见 [capability 期中更新](watch/capability/2026-10-20-ai-timeline-watch.md)）：Q3479 仍未裁决（Metaculus 官方"重建测试"裁定 reliably 标准，Opus 5.5 亦通关 Montezuma）；Epoch ECI 榜首易主 Opus 5.5（166.82＞Astra 166.41）；OpenAI ARR 口径裁决（9 月底 ~$50B 净 vs 年底指引 ≥$70B，早前 $70B 系含伙伴毛收入）使 OUR-004 理由之一强度减半——按不回改纪律维持 0.35，列 2027-01 校准项；市场近端续冷（Kalshi OAIAGI by-2027 3.1–8.9%、RSI 合约 11）、监管机器全面启动（FTC 传票×2／EU AI Act 首单／9 州在诉／白宫 SI Force）。中位锚不变。
- **治理（9/17 新增）**：暂停争论进入掌门人议程——Amodei《We Must Pace the Frontier》（9/12）获 Altman/Musk/Hassabis/Nadella 背书，Zuckerberg/黄仁勋反对，前沿阵营分裂；Ban ASI Act 获 Warren 支持但中选前立法窗口已关；Anthropic 研究员 Coxon 以"十年 p(doom)>10%"辞职（已登记 EXT-088/089，见 [暂停争论事件笔记](watch/capability/2026-09-17-pause-debate-note.md)）。
- **中国**：扩散侧差距已收窄到月级（AI Index 2.7%），起源侧（前沿训练算力）仍差一个数量级；官方赌渗透率而非 AGI 时刻——这不参与"何时 AGI"的竞猜，却在压低全球 AI 供给曲线。
- **生物安全（AI×bio，9/11 建库）**：uplift 任务级证据已实（VCT 超专家线、5 倍协议撰写）、端到端为零、历史基率"三连败"；p(doom) 12% 中生物通道 ≈2–3pp 且可在工具 AI 阶段兑现（与起飞正交，见 [ai-bio-risk/05](ai-bio-risk/05-forecasts.md)）。五年三情景：α 防线粘住 45% / β 灰色侵蚀 35% / γ 门槛击穿 20%；净倾斜取决于 DNA 合成筛查覆盖率 vs 自动化湿实验室扩散速度的赛跑。最重要近期清算锚：Anthropic 首次实测披露 ASL-4 级（我方 0.35 by 2027；Metaculus Q38589 中位 2027-07）。
- **p(doom)**：我方 ~12%（介于主流 5-9% 与 LW 社区 20-40%）。通道分解：**错齐 7.0 / 生物滥用 2.5 / AI 加速战争 1.5 / 渐进失权 0.7 / 其他 0.3（pp，9/11 建档）**——生物通道为唯一可在工具 AI 阶段兑现的主通道，全表见 [agi-timelines/06](agi-timelines/06-pdoom-decomposition.md)。

## 约定

- 所有预测性数字登记入 `predictions/ledger.md` 及其分簿，其他文档不单独维护概率。
- 数据标注来源与日期；低可信度来源显式标注；口径冲突并列呈现。
- 我方预测署名 GLM-5.3（研究代理）；季度校准回顾每年 10 月首周执行。
