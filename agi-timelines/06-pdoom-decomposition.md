# 06 · p(doom) 灾难通道分解

研究日期：2026-09-11。触发：仓库盘点发现 p(doom) 只有总量与零星通道估计，无按灾难类型的完整分解。来源：Toby Ord《The Precipice》原表（经 Precipice Revisited 核对）、Carlsmith 报告原文（arXiv:2206.13385）、AI Impacts 汇总表、Metaculus 页面直查（2026-09-11）、Vox/Axios/BBC 报道；由研究代理检索核实，概率保留原始口径。

## 一、现状盘点：仓库有什么、缺什么

| 已有 | 条目 |
|---|---|
| 总量 | OUR-018：p(doom) 12%（本世纪 AI 导致灭绝或永久失权，区间 10–15%） |
| 阶段分布 | OUR-019：风险质量 70% 集中在起飞阶段（元判断） |
| 单通道 | OUR-056：生物通道 ≈2.5pp（2026-09-11，ai-bio-risk）；OUR-057：生物路径若兑现则早于自动化研究员 |
| 外部点估计 | EXT-062~070（Yudkowsky >95% … AI Impacts 5%/9%） |

**缺**：把 12% 按灾难类型拆开的通道分解。本文件补上——结论先行：**12% ＝ 错齐/权力寻求 7.0pp ＋ 生物滥用 2.5pp ＋ AI 加速大国战争 1.5pp ＋ 渐进失权 0.7pp ＋ 其他 0.3pp**（登记 OUR-061~064，为 OUR-018 分解项、不双计）。

## 二、外部锚

### 2.1 Ord《The Precipice》表 6.1（至 2120，作者取整到最近数量级）

| 通道 | Ord 数字 |
|---|---|
| 非对齐 AI | **~1/10** |
| 不可预见的人类风险 | ~1/30 |
| 工程大流行 | ~1/30 |
| 其他人类风险（纳米、反乌托邦等） | ~1/50 |
| 核战争 / 气候变化 / 其他环境破坏 | 各 ~1/1000 |
| **自然大流行 / 超级火山** | 各 **~1/10,000** |
| 小行星/彗星 ~1/10⁶；恒星爆炸 ~1/10⁹ | 自然风险小计 ~1/10,000 |
| 人类风险小计与总量 | **~1/6** |

注：Ord 2024-07《The Precipice Revisited》确认主数字未大动（方向：气候调低、核战调高）。**口径修正**：ai-bio-risk/04 与 ledger EXT-071 原引"自然大流行 1/1000"有误，本表经原书核对为 1/10,000（自然小计 1/10,000 才自洽），已在两处订正（见修订历史）。

### 2.2 分解式尝试——全部是"前提链"，无人按灾难类型拆分

- **Carlsmith（2022，窗口 by 2070）**：六前提合取——P(2070 前可造权力寻求 AI) 65% × 激励相容 80% × 对齐困难 40% × 高影响失误 65% × 永久夺权 40% × 夺权即存亡灾难 95% ≈ **~5%**；作者终值上调至 **>10%**。超预测者复刻同前提：80%/90%/58%/25%/**5%**/40% ≈ **~1%**。
- **Baum（2021）**：Guesstimate 重参数化 Carlsmith 前提，四情形区间 [2.1%,14%]/[0.4%,34%]/[3.4%,15%]/[2.3%,8.3%]。
- **Samotsvety（2024）**：错齐 AI 接管 by 2100 **25%**。
- **Gradual Disempowerment**（Kulveit/Leech/Kilmer/Duvenaud/Kokotajlo，arXiv:2501.16946，2025-01）：**纯论证不给概率**；Duvenaud 个人口径 doom "70% to 80%"（80,000 Hours，2025 录/2026-01 刊）。
- **Hendrycks & Kaya《An Overview of Catastrophic AI Risks》(2023)**：武器化/滥用/竞赛/组织/失控五分类——**无概率**。CSET/CATO/Benton et al：未发现量化分解。

**结论：按灾难类型的量化分解在外部文献中不存在，本文件是自建框架、无直接对标。**

### 2.3 掌门人/研究者新引（补 EXT 缺口）

- **Dario Amodei**：10–25%（Logan Bartlett Show EP82，2023-10）；**2025-09-17 Axios AI+ Summit："There's a 25% chance that things go really, really badly"**（同时 75% "really, really well"；自称讨厌 p(doom) 这个词）。
- **Altman**：仅 ">0%"（2025-10 MD MEETS 访谈）；Noah Smith 转述 Döpfner 访谈 ~2%（二手，低-中可信度）。**Hassabis**：拒绝给数（">0"）。
- 研究者（Wikipedia P(doom) 词条收录口径）：**Hinton** 10–20%（综合）或 >50%（独立印象，METR 2024-06）；**Leike** 10–90%（2023）；**Bengio** 20%；**Karnofsky** 50%（Spectator 2024-03）；**Critch** 85%；**Duvenaud** 70–80%；Anthropic 现员工 **Hubinger** >10%（十年内 AI "could kill all humans"，BBC 2026-09）。
- **传闻级（未能核实）**："Anthropic 员工调查均值 ~25%"查无此调查——最接近的是 Vox 2024-01 报道的 AI Impacts 2023 调查（均值 14.4%/中位 5%）；前员工 Jacob Coxon 2026-09 在 CNN 称"约一半同事"认真看待末日（非正式）。**不登记入 EXT，只记录。**

### 2.4 Metaculus 直查（2026-09-11）

#578 任意原因灭绝 by 2100：**1%**（1.7k 人）；#27035 AI 致灭绝 by 2100（AI Risk 条件树系列）：**1%**；#26244 "AGI 后 5 年人类灭绝"：**1%**；#1495 若全球灾难发生、由 AI 失效模式引起：**30%**（对照 #1494 核战争 29%——**社区认为 AI 失效与核战是灾难的两个并列首要候选**）；"AI 直接引发核战争"独立问题未发现。

## 三、我方分解：12% 按灾难通道

| 通道 | 概率（pp） | 占比 | 推理依据 |
|---|---|---|---|
| **A 错齐/权力寻求**（起飞阶段的超级智能失齐，含快速夺权） | **7.0** | 58% | 主质量。锚：Carlsmith >10% 与 Samotsvety 25%（我方在其下——对齐研究在真实推进）、XPT 专家 3%（我方在其上——前提链每环独立证据支持）；与 04 §B 起飞形态经 §四桥表自洽 |
| **B 生物滥用**（工具阶段，AI×bio） | **2.5** | 21% | OUR-056（ai-bio-risk/05 §D），此处引用不重开 |
| **C AI 加速的大国战争**（含核升级；AI 作为决策加速器/误判源/首次打击变量） | **1.5** | 12.5% | 锚：Metaculus #1495/#1494（AI 失效与核战并列 30/29%）、Michael 2022 NLP 调查 36% 认同"AI 决策可致核级灾难"；我方折价：战争路径需多层失误叠加，且危机中人类保留离场能力的历史记录尚可（古巴导弹危机类） |
| **D 渐进失权**（Christiano《What Failure Looks Like》/Gradual Disempowerment 谱系：Goodhart 优化权移交、威权强化、价值锁定——无单一"事件"） | **0.7** | 6% | 最难清算的通道（OUR-018 的"永久失权"半边）；GD 论证有力但给不出概率，Duvenaud 70–80% 是极端锚；我方低位：人类制度对"缓慢"的适应力被 GD 低估，与 04"共识高估单一戏剧性"的立场一致 |
| **E 其他**（非生 WMD、AI 使能的不可预见复合路径——Ord "unforeseeable anthropogenic" 的 AI 版） | **0.3** | 2.5% | 残差项，承认框架不完备 |

**合计 12.0pp ＝ OUR-018。**

## 四、桥表：起飞形态 → 条件 p(doom)（连接 04 §B 与 §D）

把 §三按 04 §B 的四形态重排（条件于各形态的全部灾难通道合计）：

| 起飞形态（OUR-010~013 先验） | 条件 p(doom) | 贡献（pp） |
|---|---|---|
| 硬起飞（15%） | ~30% | 4.5 |
| 快起飞（30%） | ~20% | 6.0 |
| 慢起飞（40%） | ~5% | 2.0 |
| 无起飞/平台（15%） | ~0.5% | 0.75 |
| 加权 | — | **≈12.3 ≈ 12** ✓ |

这张表是 04 §B（起飞概率）与 OUR-018（p(doom)）之间此前缺失的连接件；条件值的合理区间应在 2027-08 年度回顾时重估（登记 OUR-065）。

## 五、一致性检查

- **vs OUR-019（70% 起飞集中）**：起飞阶段质量 ＝ A(7.0) ＋ C 的起飞期份额(~0.9) ＋ E(~0.15) ≈ 8.05/12 ≈ **67% ≈ 70%** ✓（B、D 主要在工具阶段）。
- **vs OUR-056/057**：B 通道即 OUR-056；OUR-057（生物早于自动化研究员）与 D/E 的工具阶段属性一致。
- **vs 外部阵营**：我方 12% 位于 Dario（25%）与 XPT 专家（3%）之间、低于 LW 主流（20–40%）——与 04 §D 原立场一致，本分解未改变总量。
- **非 AI 对照**：我方隐含"AI 占本世纪存亡风险质量的绝大部分"（12% vs Ord 非 AI 人类风险合计 ~5%、自然风险 ~0.01%）——与 Ord 的 1/10 非对齐 AI 主导结构同向。

## 六、登记与清算说明

- OUR-061~064 为 OUR-018 的**分解项**：校准统计只计 OUR-018，不双计（仿 OUR-056 惯例）；分解值不受 0.05 分辨率约束（pp 级拆分无意义），清算窗口同为 2100-12-31、远期仅记录。
- OUR-065（桥表条件值）为元判断，不计 Brier；在 OUR-010~013 形态确认时作复盘锚。
- 本文件不改 04 §D 任何数字；修订一律走 ledger（§四纪律）。

## 来源

- https://www.tobyord.com/writing/the-precipice-revisited （总表核对，2024-07）
- https://arxiv.org/abs/2206.13385 （Carlsmith 2022，窗口 2070）；https://joecarlsmith.com/2023/03/22/…shorter-version/ ；https://joecarlsmith.substack.com/p/superforecasting-the-premises-in （超预复刻）
- https://arxiv.org/abs/2501.16946 （Gradual Disempowerment）；https://80000hours.org/podcast/episodes/david-duvenaud-ais-could-soon-run-ai-research/ （Duvenaud 70–80%）
- https://en.wikipedia.org/wiki/P(doom) （掌门人/研究者引语汇总）；https://www.axios.com/2025/09/17/anthropic-dario-amodei-p-doom-25-percent ；https://www.bbc.com/news/articles/ckgwy1k42w4o （Hubinger）
- https://wiki.aiimpacts.org/uncategorized/ai_risk_surveys （汇总表）；https://forum.effectivealtruism.org/posts/EG9xDM8YRz4JN4wMN （Samotsvety 25%）
- Metaculus：metaculus.com/questions/{578,26244,27035,1495,1494,8531}/（2026-09-11 直查）
