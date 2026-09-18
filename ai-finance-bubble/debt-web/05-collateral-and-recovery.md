# 抵押品经济学与违约回收率前瞻：真违约时，债主能拿回几毛钱

撰写日期：2026-09-18｜系列：debt-web 05/07

> 定位：debt-web 系列第 5 篇。前篇讨论债务结构与传导链，本篇回答清算端问题——违约落地时，各层债权的抵押品在公开市场上值多少钱。可信度三级：[高]官方/一手，[中]主流财经媒体/具名机构，[低-中]中小来源。回收率数字为**分析假设区间**（附依据与类比），非登记预测；如需转为可证伪条目须走 `predictions/ledger.md` 流程。核心输入：`../raw-reports/2026-08-21-capex-debt-circular-deals.md`（research-01）、`../raw-reports/2026-08-21-ai-progress-revenue-adoption.md`（research-04）、`../crash-dynamics/01-dotcom-2000-anatomy.md`（电信回收率类比）。核实于 2026-09-18。

---

## 一、GPU 抵押贷款的估值机制

### 1.1 结构模板：CoreWeave DDTL 是全行业的母本

CoreWeave 的延迟提取定期贷款（DDTL）结构已成为 GPU 抵押贷的行业模板——每一层贷款以**特定 GPU 库存 + 其所服务的客户合同**作抵押，而非母公司信用：[中] [MTS Drops, 2026-05-10](https://drops.mts.now/ai-capex/wiki/operators/neoclouds/)

| 层 | 规模 | 时间 | 定价 | 备注 |
|---|---|---|---|---|
| DDTL 1.0 | $2.3B | 2023-08 | ~15% 浮动 | Magnetar/Blackstone 牵头，契约最重 |
| DDTL 2.0 | ~$7.5B | 2024-05 | ~11% 浮动 | Blackstone/Magnetar |
| DDTL 4.0 | $7.5B（可扩至 $8.5B） | 2026-03-31 关闭 | SOFR+225bp 浮动 / ~5.9% 固定 | MUFG 行政代理、U.S. Bank 抵押代理，2032 到期，季度摊销 |

[中] [Global Data Center Hub, 2026-07-23](https://www.globaldatacenterhub.com/p/is-coreweaves-85-billion-deal-the)；[LinkedIn/Himmel, 2026-05-18](https://www.linkedin.com/pulse/financialization-ai-infrastructure-capital-abundance-top-himmel-ycvke)；[Margin Notes, 2026-05-18](https://crepesupreme.substack.com/p/the-chips-age-faster-than-the-debt)。截至 Q1'26 CoreWeave 总债务 ~$25B（research-01 §2）。行业新进入者的典型条款：LTV 60–70%、期限 3–5 年、硬件即抵押。[低-中] [American Compute, 2026-03-09](https://www.amcompute.com/blog/starting-a-neocloud)

### 1.2 估值谁定：采购价入账，市价重估机制缺位

这是本篇最重要的机制发现：**GPU 抵押贷的抵押价值在存续期内基本不做市价重估**。

- 放款时按采购发票价/装机成本入账，LTV 60–70% 打在采购价上；
- 存续期保护靠两件事：(a) 季度本金摊销使贷款余额下降速度快于（假设的）折旧曲线；(b) 客户合同现金流覆盖倍数，而非抵押物市价；
- 核验手段是物理性的：序列号追踪、季度放款人现场检查、要求 GPU 安装在放款人认可的设施内、UCC-1 备案确权。[低-中] [AltStreet, 2026-01-17](https://altstreet.investments/reference/structures/gpu-collateralization)；[Thinh's Substack, 2026-03-31](https://tle9.substack.com/p/the-financialization-of-artificial)
- 后果：**抵押账面价值与二手市价之间没有制度化的传导管道**。只要借款人还在付息，没有任何一方（放款人、审计师、评级机构）被强制按市价重估抵押物。ABS 层的残值假设更是冻结在发行日：GPU ABS 模型假设 3 年残值 50%、5 年 20%。[低-中] [The AI Realist, 2026-02-20](https://www.airealist.ai/p/two-markets-one-asset-the-gpu-debt)

对照：住房抵押贷在 2006 年前同样是"重估缺位"，直到大宗法拍成交价把市价砸在所有人面前。GPU 世界目前正处在"法拍尚未开始"的阶段。

### 1.3 租金已崩、卡价未崩：抵押品账面的关键脆弱点

两个价格的背离是 2026 年中最值得盯的数据结构：

- **时租（流量价格）已崩**：H100 marketplace 时租从 2023 年峰值 ~$8 跌至 $1.33–1.49（research-04 §4，[中]）；综合口径 ~$2，部分 marketplace 已破 $1；H200 自 AWS 发布价 $10.60 跌至 $3.39 中位数（-68%/17 个月）；B200 自 $14 跌至 <$4（-73%/9 个月）。[低-中] [The AI Realist, 2026-02-20](https://www.airealist.ai/p/two-markets-one-asset-the-gpu-debt)。SemiAnalysis 估计 H100 需租到 $0.98/时才能与 Blackwell 的每 token 成本打平——即再跌 55%。[中] [CNBC 转引, 2025-03-26](https://www.airealist.ai/p/two-markets-one-asset-the-gpu-debt)
- **二手卡价（存量价格）尚未崩**：2026 年中二手 H100 SXM5 经纪商/翻新渠道报价 $18–25K，约为 $30K 新卡价的 60–85%（[低-中] [Mercatus, 2026-07-08](https://www.mercatus-ai.com/blog/h100-resale-value)；[Caladan Semi, 2026-05-14](https://caladansemi.com/blog/nvidia-gpu-pricing-trends-2026)）；eBay 长尾挂单低至 $6–9K，口径冲突并列标注 [低-中] [Instagram 聚合, 2026-07](https://www.instagram.com/p/DVGHCcTkZ52/)。
- **解读**：卡价坚挺不是因为价值真实，而是因为**至今没有大规模强制卖出**。现有二手流量是零星的、卖方不着急的；租金曲线（前瞻收入）与卡价（账面锚）之间的裂口，会在第一次大宗清算拍卖时以跳空方式收敛——方向向下。

### 1.4 二手市场：有渠道、无深度、无大宗成交先例

价格发现基础设施 2025–26 年快速成形但深度极薄：

- **渠道**：经纪商（BuySellRam、GPU Smith）、翻新商（Mercatus，含质保）、拍卖行（Exit Technologies）、指数服务（Silicon Data H100 指数已上 Bloomberg；Ornn OCPI 覆盖 H100/H200/B200/RTX 5090）。[低-中] [Servnet, 2026-07-31](https://www.servnetuk.com/insights/used-hopper-h100-h200-buy-second-hand-2026)
- **衍生品层**：Ornn 2026-01 完成首笔 OTC 算力互换，推出"残值互换"（实为 GPU 看跌期权，与 USD.AI 合作为第 3–4 年硬件提供保底价）；Architect（前 FTX US 总裁 Brett Harrison）即将上线 GPU 时租永续期货。**注意 AIG 式对手方风险：Ornn 融资仅 $5.7M，却在为年贬 70–80% 的资产担保残值。** [低-中] [The AI Realist, 2026-02-20](https://www.airealist.ai/p/two-markets-one-asset-the-gpu-debt)
- **关键事实**：至今没有一次 neocloud 破产清算的大宗 GPU 拍卖成交。当前所有"市价"都是**零售边际报价**，不是出清价。出清价只有在第一具尸体上才能量出来（见 §五）。

### 1.5 Tricolor 式重复质押在 GPU 世界的可能性

2025-09 Tricolor（次级车贷）Chapter 7 崩塌是资产抵押融资（ABF）的信任事件：同一批车贷被重复质押给多个放款人/证券化载体，一家承销商 2025-08 的分析发现 7 笔证券化中 $365.5M 本金被双重质押，破产受托人的法证会计认定借款基数虚增至少 $675M；SEC 于 2026-08-18 起诉三名前高管，DOJ 2025-12 已刑事起诉 CEO/COO。[高] [DOJ SDNY, 2026-05-04](https://www.justice.gov/usao-sdny/prosecuting-fraud)；[中] [American Banker, 2026-08-20](https://www.americanbanker.com/news/sec-sues-three-ex-tricolor-executives-over-bond-fraud)

GPU 抵押的防重复质押条件**好于车贷但非免疫**：

- **有利面**：GPU 物理集中于少数数据中心、有序列号、可被现场盘点、UCC-1 备案公开可查；放款人普遍要求季度检查与托管设施白名单（§1.2）。车贷欺诈赖以生存的"资产分散在十万车主手里、核验靠贷款磁带"的条件在 GPU 世界不成立。
- **风险面**：重复质押的 GPU 版本不是"同一张卡押两次"，而是**同一现金流的多重切割**——同一集群的 GPU 押给 DDTL A、其上租约应收款打包进 ABS、机柜所在建筑再做售后回租、母层再发公司债。每一层单独看都"有抵押"，叠加后同一经济资产被切了三四刀。Tricolor 教训的真正要点是：**核验的是文件，欺诈发生在文件之间的缝隙里**。CoreWeave 多层 DDTL + 可转债 + 售后回租的叠床架屋结构（总债 $25B 对 2026 预期 FCF -$18.8B，research-01 §2）正是缝隙最多的结构。
- **修补尝试**：USD.AI 用链上登记做 GPU 真实性/位置实时核验，是市场对 Tricolor 冲击的直接回应。[低-中] [USD.AI, 2025-12-05](https://usd.ai/insights/how-to-finance-gpu-cluster-7-days-usd-ai)

---

## 二、数据中心清算价值分解

违约的数据中心不是单一资产，是三层折旧速度完全不同的资产的捆绑。分别估：

### 2.1 三层拆解与回收率假设

| 层 | 内容 | 占总成本量级 | 回收率假设（违约清算情形） | 依据 |
|---|---|---|---|---|
| **硬层：带电土地 + 变电站 + 并网权** | 已通电地块、专用变电站、变压器、并网协议排队位置 | 15–25% | **60–80%** | 电力接入是当前最稀缺要素：大型变压器交期 128 周、升压机组 144 周（Wood Mackenzie，research-04 §4）；并网排队是最大瓶颈。"带电"本身是可交易的稀缺品，且不受 GPU 代际贬值影响——这是 2000 年类比中"光纤管道/铁塔"的位置 |
| **半硬层：建筑壳 + 制冷 + 配电** | 机房建筑、液冷/风冷系统、中低压配电 | 30–40% | **30–50%** | AI 专用设计（高功率密度、液冷管路）对通用 colocation 或改作他用是减分项，改造费用侵蚀残值；但若电力容量保留，壳+电的组合对下一家算力运营商仍有重建价值 |
| **软层：GPU + 网络设备** | GPU 服务器、InfiniBand/光模块、存储 | 40–55% | **20–40%（基准情形）；出清期 10–20%** | 年贬 70–80% 的租金曲线（§1.3）；2000 年类比：暗光纤卖原始成本 1–2 折、WorldCom 债权人回收 35–40 美分（crash-dynamics 01 §五）；GPU 比光纤贬得快——光纤 2.7% 点亮率十年后仍是骨干，H100 三年后是电老虎 |

成本结构参照：2026 年数据中心建设成本基准 $8–12M/MW（标准）至 $15–20M+/MW（AI 级）。[低-中] [irecruit, 2026-05-18](https://www.irecruit.co/insights/data-center-construction-cost-per-mw-2026-benchmarks-owners)

**合并口径**：一个违约的满载 AI 数据中心，整体清算回收率基准假设 **35–50%**（加权），其中电力层贡献主要价值。这意味着以资产本身论，LTV 60–70% 的贷款在违约时**天然资不抵债**——放款人的真实保护从来不是抵押物，而是摊销进度 + 租户合同。

### 2.2 空置率情景：今天的 1–2% 不是出清期的数字

- 当前：北弗吉尼亚空置率 0.3%（2026 Q1）、全国 ~2%（Newmark）、预租率 81.5%（research-04 §4，[中]）。在这个市场状态下违约，资产有真实竞标者，回收率取上沿。
- 出清情形假设：若情景 A 兑现（capex 收缩 + neocloud 连锁违约），空置率假设推到 **15–25%**——参照 2002 年光纤点亮率 2.7% 的极端（crash-dynamics 01 §二），AI 数据中心即使需求塌方也不会那么惨（推理需求真实存在），但**新增供给惯性 + 集中违约同时砸盘**足以把边际买家变成秃鹫。此情形下：硬层回收率降至 40–60%（电力稀缺溢价仍在但买家杀价）、半硬层 15–30%、软层 10–20%，整体 **20–35%**。
- **历史锚**：Cyxtera 2023-06 Chapter 11（61 个数据中心、曾以 $3.4B SPAC 上市），Brookfield 以 $775M 收购几乎全部资产（2024-01-12 完成）——**约相当于 SPAC 估值的 2.3 折**，且这发生在空置率历史低位、没有行业性危机的 2023 年。注意口径：该价含运营业务转移与租约重组，非纯地产清算价，标注不确定。[高] [SEC 8-K, 2023-11](https://www.sec.gov/Archives/edgar/1794905/000179490523000087/cyxtbrookfieldapapressrele.htm)；[低-中] [Rotten WiFi, 2026-09-07](https://rottenwifi.com/brookfield-completed-its-775-million-acquisition-of-bankrupt-cyxtera-what-the-deal-included/)

---

## 三、评级假设审视

### 3.1 Hyperion A+ 的隐含回收假设：锚定的是 Meta，不是资产

Meta Hyperion SPV（Beignet Investor）$27B 债获 S&P A+，2049 到期、全额摊销、定价 SOFR+225bp、收益率 6.58%——**评级是投资级，定价是准垃圾级**。市场用脚投票指出了评级的真实逻辑：[中] [WSJ, 2025-10-21](https://www.wsj.com/finance/investing/blackrock-etfs-among-biggest-investors-in-metas-giant-data-center-debt-deal-087fe671)；[PE Insights, 2025-10](https://pe-insights.com/blue-owl-and-meta-close-record-30bn-financing-for-ai-data-centre-expansion-in-louisiana/)

A+ 的隐含假设拆解：

1. **第一还款来源是 Meta 租约**（15 年+、triple-net），不是资产。Meta 另提供**有上限的 16 年残值担保**。[低-中] [Margin Notes, 2026-05-18](https://crepesupreme.substack.com/p/the-chips-age-faster-than-the-debt)；[Cogniscendo, 2026-08-11](https://www.cogniscendo.com/p/compute-is-revenue-revenue-is-collateral)
2. 换言之，A+ ≈ "Meta 的信用 - 若干档结构化折扣"。资产清算价值在评级方法论里只是次级后备。
3. **脆弱点**：担保是 capped 的。若 2035 年后 Meta 不续租，残值担保上限之外的缺口由债券持有人吃。按 §2.1，5GW、>$50B 总成本的项目里，GPU/网络层届时已折旧近零，硬+半硬层的清算价值对 $27B 债的覆盖率可能在 30–50%——**A+ 的真实含义是"Meta 不出事"，而不是"这堆资产值这个价"**。

### 3.2 数据中心 ABS/CMBS 的评级方法论分裂

- 市场规模：数据中心 ABS/CMBS 累计发行 $34.4B（69 笔、19 家发行人），2025 年内 $23.8B、同比翻倍；平均单笔从 2022 年 $320M 升至 2025 年 $1.1B；数据中心已占 SASB CMBS 市场的 13%。[低-中] [CRA Research/CREFC 转引, 2025-11](https://www.airealist.ai/p/two-markets-one-asset-the-gpu-debt)
- **机构间方法论分裂**：S&P 对整个数据中心 ABS 板块**封顶 A+**；Moody's 2026-02-11 却给出史上首个数据中心证券化 Aaa（Compass Datacenters $830M，6 个 100% 出租给 IG 租户的设施、$3.6B 评估地产、优先级 S+120bp）。同一资产类别，两家差出多个子级——上一次评级机构对新型抵押品分歧这么大，标的是住房按揭。[低-中] [The AI Realist, 2026-02-20](https://www.airealist.ai/p/two-markets-one-asset-the-gpu-debt)
- **GPU 残值假设已被证伪**：GPU ABS 的 50%@3 年残值假设，被 B200 用 9 个月跌 73% 打穿（§1.3）。Fitch 已就是否将 GPU 折旧正式纳入 AI 基础设施证券化评级发起公开咨询——方法论修订本身即是预警信号。[低-中] 同上
- 需求端狂热：Blackstone/QTS $3.46B CMBS 的**次级档**获 23 倍超购。[低-中] 同上

### 3.3 评级滞后史：2000–2002 电信债对照

WorldCom 时间线是评级滞后的标准教材：[高] [LA Times, 2002-05-10](https://www.latimes.com/archives/la-xpm-2002-may-10-fi-worldcom10-story.html)；[Bloomberg, 2002-06-25](https://www.bloomberg.com/news/articles/2002-06-25/s-and-p-cuts-worldcom-credit-rating)

- 2002 年初：Moody's 评级 A2（投资级中上）；
- 2002-05-09：一次性下调 3 档至 Ba2（垃圾级）；
- 2002-06-25（会计丑闻曝光次日）：S&P 从 B+ 砍至 CCC-；
- 2002-07-21：破产。
- 对照组：独立机构 Egan-Jones 早在 2000-11 就将其降至最低投资级、2002-03 降至垃圾级——**领先 issuer-pay 机构 14 个月以上**。[高] [Egan-Jones 向 SEC 陈述](https://www.sec.gov/news/extra/credrate/eganjones2.htm)

**映射**：Hyperion A+、Compass Aaa 与 CoreWeave CDS 640–700bp（隐含 5 年违约概率 40–55%）并存，就是 2002 年初"A2 评级 vs 债券市场已按 junk 交易"的复刻。[中] [The AI Realist, 2026-02-20](https://www.airealist.ai/p/two-markets-one-asset-the-gpu-debt)（CDS 数据为 2025-11/12 读数，此后可能已移动）。评级不是回收率的领先指标，是确认指标——本篇的回收率假设全部建立在"评级落地之前市场价先落地"的前提上。

---

## 四、回收率前瞻表

按主体类型分档。回收率指违约债权最终回收（面值美分），基准=需求温和收缩的违约情形；敏感性列=GPU 二手价在当前基础上再跌 50%（约相当于 H100 跌至 $8–12K、B200 跌破发行价一半——即情景 A 兑现 + Rubin 放量）。

| 档位 | 代表敞口 | 基准回收率 | GPU 再跌 50% 情形 | 依据与类比 |
|---|---|---|---|---|
| **① Hyperscaler 表内债** | Meta $25B 债、Oracle $18B+、Amazon $12B、MSFT/GOOG 发债 | **85–100 美分** | 80–95 | 还款来源是企业现金流而非 AI 资产清算；类比 2001 年 Cisco——计提 $22 亿库存减值后债券依然全额兑付。风险不是违约而是利差重定价 |
| **② SPV 项目债（强租户担保型）** | Meta Hyperion $27B（A+）、Compass 类 Aaa ABS、PIMCO/Oracle 密歇根 $14B | 租户履约：**~100**；租户违约/不续租：**40–70** | 租户违约情形降至 30–55 | 结构=租约信用 + capped 残值担保 + 电力硬资产兜底（§2.1 硬层 60–80%）。类比：有铁塔/牌照的电信资产回收显著高于纯流量故事（crash-dynamics 01 §五） |
| **③ Neocloud GPU 抵押贷** | CoreWeave DDTL 系列、Lambda GPU ABS、Nebius/Crusoe 抵押融资 | **30–50 美分** | **15–30** | 抵押物年贬 70–80% + 借款人负 FCF（CoreWeave 2026E FCF -$18.8B）；类比 WorldCom 债权人回收 35–40 美分、暗光纤 1–2 折。放款人博弈激励：宁可重组也不愿清算——清算会把二手价格砸穿、连带减值自己的存量抵押簿（§1.3）。这会人为抬高"账面回收率"、推迟真实价格发现 |
| **④ 私募信贷软件/企业贷款** | BDC/直接放贷组合中的 AI 应用层、SaaS 借款 | **45–65 美分** | 40–60（违约率升、单户回收变化小） | 传统 first-lien 中间市场回收中枢 40–60 美分；抵押是 ARR/企业价值而非硬件，GPU 价格传导弱，但需求侧（企业 AI 预算收缩）推高违约率 |
| **⑤ 无担保 vendor financing 敞口** | Nvidia→OpenAI 类投资/担保、AMD 认股权证结构、设备商应收 | **0–20 美分** | 0–10 | 无抵押、无优先权、且与借款人股价/再融资能力同涨同跌；类比 Lucent 2001–02 累计计提 $35 亿+客户坏账、Cisco 核销 $9 亿客户贷款（crash-dynamics 01 §二环③）。Nvidia 的 $6.3B CoreWeave 容量兜底是此类敞口的活样本 |

**表的总读数**：回收率与"离实物电力资产的距离"成正比、与"离 GPU 迭代曲线的距离"成反比。债权排序越靠近租约与变电站，越像 WorldCom 的 35–40 美分；越靠近 GPU 与无担保承诺，越像 CLEC 的 20 美分以下。

---

## 五、"公允价值证据"事件：什么会强制市场重估抵押品

主报告 `../ai-bubble-scenarios.md` Phase 2 的链条（neocloud 重组 → GPU 抵押贷减值 → 私募信贷连锁计提）目前卡在第一步之前：如 §1.3 所示，**租金崩了 80% 而卡价没崩**，审计师、放款人、评级机构都还能引用经纪商报价维持账面。打破这个均衡需要公开、不可回避的市价证据。按冲击力排序：

1. **大宗破产清算拍卖（决定性事件）。** 第一个中型以上 neocloud 清算、数千张 GPU 一次性砸进二级市场时，会产生第一个"出清价"数据点。所有按 $18–25K 报价记账的抵押簿将在一周内被要求对齐拍卖成交价。参照物：2001–02 年破产运营商设备流入二手市场直接压低全行业设备抵押价值（crash-dynamics 01 §二环③-3）。**监测对象**：CoreWeave 债券/CDS 定价、二线 neocloud 的再融资窗口（2026–27 到期墙）。
2. **审计师不签字 / 强制减值。** 触发点不是时租下跌（审计师可以辩称合同现金流仍在），而是二手成交价证据 + 残值互换市场（Ornn 类）报价同时出现，使"50%@3 年"假设在审计意义上不可辩护。Burry 的折旧指控（2026–28 累计少提 ~$176B，research-01 §4）目前停留在 X 帖层面；一旦四大会计师事务所之一在某家 hyperscaler 或 neocloud 的折旧/减值政策上出具保留意见，事件性质从"看空观点"变为"披露可信度危机"——对应 2002 年环④（安然/WorldCom）的传导模板。
3. **评级方法论修订落地。** Fitch 的 GPU 折旧咨询（§3.2）若落地为正式方法论，将追溯触发存量 GPU ABS 的评级复审；S&P 若将行业封顶从 A+ 下调、或 Moody's 撤回 Compass Aaa，任一动都是"评级机构自己承认旧假设错误"的公共知识事件——参照 Barron's《Burning Up》的机制：不需要新数据，只需要把私人怀疑变成公共知识（crash-dynamics 01 §一）。
4. **贷款契约的机械触发。** DDTL 的摊销与覆盖倍数契约在租金曲线下行中会陆续触线，触发追保或提前摊销。这类事件单笔不公开，但**再融资条款的恶化是可观察的**：若 2026Q4–2027 年 GPU 抵押贷再融资的 LTV 从 60–70% 系统性降至 40–50%、或利差大幅走阔，等于放款人用新条款承认旧抵押估值失效。
5. **残值衍生品市场给出报价。** Ornn 残值互换、Architect 永续期货一旦有足够成交量，GPU 将第一次有公开的远期价格曲线——这是双向的：它可以让放款人对冲从而稳定市场（§1.4），也可以让空头第一次有了不用持有实物的做空工具，加速价格发现。

**信号意义排序**：1 与 2 是 Phase 2 的点火器，3 与 4 是慢变量确认，5 是基础设施性的（发生后一切重估都会变快）。当前状态（2026-09-18）：3 已在途（Fitch 咨询），4 局部可见（CoreWeave DDTL 4.0 定价 SOFR+225 仍属温和），1、2、5 均未发生——**抵押品重估的全部证据链还差最关键的一环：一笔大宗强制成交**。

---

## 附：核实笔记与口径说明

- "租金崩、卡价未崩"是本文最反直觉的核实发现：2026 年中二手 H100 经纪渠道仍报 $18–25K（60–85% of list），与时租 -80% 并存；eBay $6–9K 口径（[低-中]）与经纪渠道并列呈现，差异反映零售长尾与机构渠道的价差。本文回收率假设基于"强制清算时向租金曲线隐含价值收敛"的判断。
- CoreWeave CDS 640–700bp 为 2025-11/12 读数，是截至本文撰写可独立溯源的最新公开数据，此后可能已移动；引用时保留时点。
- Cyxtera $775M 对 $3.4B SPAC 估值的"2.3 折"为粗口径：SPAC 估值含股权泡沫成分，$775M 含运营业务与租约重组，非纯资产清算价；仅作方向性参照。
- 变压器交期 128 周/升压机组 144 周转引自 research-04 §4（Wood Mackenzie）；2026-09 复核见 [The Network Installers, 2026-09-03](https://thenetworkinstallers.com/blog/data-center-construction-statistics/)（[低-中]，口径一致）。
- 本文回收率区间为分析假设，未登记入 `predictions/ledger.md`；若季度回顾认为应将"neocloud GPU 抵押贷违约回收率"转为可证伪条目，需附清算标准（如：以首单 neocloud Chapter 11 的有担保债权回收率为清算值）另行提名。
- "Nebtrix"一词未核到对应实体，按 Nebius（4 年折旧口径，research-01 §4）类 neocloud 处理。
