# 债务总量与结构图：AI 资本周期的三层负债底图

撰写日期：2026-09-18｜系列：debt-web 01/07

> 本篇是全系列的底图：把 AI 资本周期的债务按**显性债（表内）／表外与准隐形债／或有负债**三层铺开，逐层逐公司汇总存量与流量。概率判断不在这里（唯一登记处是 `predictions/ledger.md`）；本篇只做事实结构。数字均带时点，来源内联标注，可信度三级（[高]=官方/一手，[中]=主流财经媒体/具名机构研究，[低-中]=中小博客/聚合站）；口径冲突并列呈现。事实底稿为 `../raw-reports/2026-08-21-capex-debt-circular-deals.md`（冻结于 2026-08-21），本篇已用 2026-08 下旬以来的新数据更新（Q2'26 财报季、9 月市场）。

---

## 〇、三层定义与读图须知

- **第一层 显性债**：落在资产负债表上的债券、贷款、可转债、融资租赁负债。法律上是债，评级、期限、利率可查。
- **第二层 表外/准隐形债**：SPV/JV 债务（发起人少数持股、不并表）、已签约但尚未生效的租赁与采购承诺（GAAP 下起租前不进表）、私募信贷直接放贷。法律上是债，但不在科技公司的表上。
- **第三层 或有负债**：容量兜底、股权投资承诺、残值担保、take-or-pay、RPO 的付款方视角。**名义上是承诺不是债**——只在触发条件成立时变成现金流出；但对手方把它们当作信用支持计入了自己的融资能力。
- 三层之间**存在结构性重复计算**（同一笔 OpenAI 支出承诺同时出现在第三层的承诺清单与供应商的 RPO/融资抵押里），加总必须去重，见 §五。

---

## 一、第一层：显性债

### 1.1 总量与流量

- **存量**：AI 相关债务存量 2025-10 达 **~$1.2T**，已成 IG 市场最大板块 [中, [M&G, 2026-03-04](https://www.mandg.com/investments/professional-investor/en-ch/insights/mandg-insights/latest-insights/2026/03/strat-fi-na-ai-hitting-bond-markets)]。注意这是宽口径（含公用事业、电力、电信等 AI 受益链），不只是科技公司债——构成见 §1.3。
- **2025 年流量**：五大超大规模厂商发债合计 **~$121B**，为 2020–24 年均值（~$28B/年）的 4 倍以上 [中, [Investing.com, 2026-05-26](https://www.investing.com/analysis/ai-bond-issuance-tests-the-markets-appetite-for-longdated-tech-debt-200680972)；[ScanX/Barclays, 2026-01-16](https://scanx.trade/stock-market-news/global/ai-investment-boom-to-drive-us-corporate-bond-issuance-to-2-46-trillion-in-2026/30085664)]。
- **2026 年流量（新数据，截至 9 月中）**：
  - AI 相关全球发行 2026 年前 5 个月已 ~$236B（上年同期 4 倍），H1 末约 $250–300B [中, [Reuters/Morgan Stanley, 2026-06-10](https://www.reuters.com/business/global-ai-debt-issuance-top-500-billion-2026-morgan-stanley-says-2026-06-10/)；[低-中, Universal Asset Owners, 2026-07-01](https://www.universalassetowners.com/probability-desk/the-probability-desk-2026-07-01/)]。
  - **全年预测口径并列**：Morgan Stanley ~$570B（AI 相关全球总发行，2026-06-10）[中]；JPM 科技/TMT 发行预测 8 月从 $450B 上调至 **$540B**（2026-08-08）[低-中, [KuCoin 转引](https://www.kucoin.com/news/flash/jpmorgan-upgrades-tech-debt-issuance-outlook-to-over-500-billion-in-2026)]；JPM AM 估 2026 超大规模厂商发行 **$279B**、2027 再 $220–300B [中, [JPM AM, 2026-08-05](https://am.jpmorgan.com/us/en/asset-management/adv/insights/market-insights/market-updates/on-the-minds-of-investors/can-credit-markets-absorb-the-ai-buildout/)]；Goldman 追踪口径"近 $500B AI 相关发行，超大规模厂商仅占 40%"（2026-08-05）[中, [Goldman Sachs](https://www.goldmansachs.com/insights/goldman-sachs-exchanges/how-ai-debt-is-reshaping-the-credit-market)]。早前的 JPM 净发行 $230B 指引（2026-07-28，见底稿 §2）已被上述毛发行口径取代——**净 vs 毛、科技 vs AI 宽口径是这组数字差异的主因**。
  - 超大规模厂商占美元 IG 发行比例：2022–24 年 2% → 2026 年预计 **9%** [中, [JPM AM, 2026-08-20](https://am.jpmorgan.com/gb/en/asset-management/institutional/insights/market-insights/market-updates/on-the-minds-of-investors/hyperscaler-debt-issuance-ai-buildout/)]。
  - 需求侧裂缝：投资者需求在供给放量下开始走弱 [中, [Fortune, 2026-07-17](https://fortune.com/2026/07/17/ai-boom-debt-blitz-investor-demand-hyperscaler-bond-issuance/)]；Fortune 口径"五大未来每年发行 $300B，2026 年 $175B"——与 JPM 的 $279B 不一致，公司集合与净/毛口径不同，并列存疑。

### 1.2 逐公司明细

**Oracle（本轮表内加杠杆最激进者）**
- 存量：总负债 $174.5B（截至 2025-11-30），其中优先无担保债 $108.1B [高, [Oracle 424B2, 2026-02-02](https://www.stocktitan.net/sec-filings/ORCL/424b2-oracle-corp-prospectus-supplement-1ca97c4668f6.html)]；评级 Baa2/BBB——五大中最低 [中, [Mawer, 2026-03-18](https://www.mawer.com/the-art-of-boring/blog/hey-google-how-much-can-i-borrow-before-i-break-the-bond-market)]。
- 融资序列：2025-09 发债 $18B；2025-11 起银行筹备 ~$38B 贷款（$23B+$15B 定期贷款，JPM 牵头）+ $18B 债券 [中, [DCD, 2025-09-26](https://www.datacenterdynamics.com/en/news/oracle-takes-on-18bn-in-debt-ahead-of-ai-data-center-build-out/)；[Octus, 2025-11-11](https://octus.com/resources/articles/banks-prep-series-of-multibillion-dollar-debt-offerings-for-oracle/)]。
- **CY2026 融资计划（2026-02-01 官宣）**：全年筹资 $45–50B，一半股权（强制可转优先股 + 新授权 $20B ATM）、一半债（单次 IG 优先无担保发行）；已在 2026-02-02 完成 **$25B 债（8 个档次含浮息）+ $5B 强制可转优先股** [高, [Oracle IR](https://investor.oracle.com/investor-news/news-details/2026/Oracle-announces-Equity-and-Debt-Financing-Plan-for-Calendar-Year-2026/default.aspx)；[Goldman Sachs IB, 2026-02-05](https://www.linkedin.com/posts/goldman-sachs-investment-banking_on-february-2-oracle-successfully-priced-activity-7425230413297594369-iXOH)]。用途明说：满足 AMD、Meta、NVIDIA、OpenAI、TikTok、xAI 等 OCI 大客户的合同需求——**表内债直接对接第三层循环承诺**。FY26 capex 实际 $55.7B，FY27 指引 ~$70B [高, [Oracle IR, 2026-06-10](https://investor.oracle.com/investor-news/news-details/2026/Oracle-Announces-Record-Q4-and-FY-2026-Results-Driven-by-Cloud-Infrastructure--Cloud-Applications/default.aspx)]。

**Meta**
- 2025-10 发债 $25B（公司史上最大，订单超 $125B，Moody's Aa3）[中, [Stocktwits, 2025-10-30](https://stocktwits.com/news-articles/markets/equity/meta-offering-breaks-record-with-125-billion-orders-for-25-billion-bond-sale/cLG8bKxR3xY)]；2026 H1 再发债 $24.9B [高, Meta Q2'26 8-K 现金流表，转引自 [Drawpie, 2026-07-30](https://drawpie.com/blog/meta-stock-drop-free-cash-flow-collapse/)]。
- 长期债务 $58.7B（FY25 末）→ **$83.7B**（2026-06-30）；净现金头寸从 -$41.4B 收窄至 -$6.6B，"距净负债约一个季度" [低-中, [MenFem 基于 10-Q, 2026-07-22](https://menfem.com/companies/meta)]。Q2'26 FCF 仅 $784M、回购归零——**自我融资时代结束，Meta 已转入债务驱动** [高, Meta Q2'26 财报，2026-07-29]。

**Amazon / Alphabet / Microsoft**
- Amazon：2025-11 重返债市 $12B [中, [Proactive, 2025-11-17](https://www.proactiveinvestors.com/companies/news/1082651/amazon-returns-to-us-bond-market-with-12b-offering-1082651.html)]；2026 年至 6 月初已发行 ~$57B，7 月再增发 $25B（30 年期），全年领跑 [低-中, [Deepstory Research, 2026-08-06](https://deepstoryresearch.com/data/ai-debt-financing/issuance-by-issuer/)；[Sage Advisory, 2026-07-16](https://www.sageadvisory.com/article/hyperscaler-debt-deluge-the-new-driver-of-ig-spread-pressure)]。
- Alphabet：2026 年至 6 月初发行 ~$52B（与 Amazon 合计占五大 2026 年 $159B 的一半以上）[低-中, Deepstory 同上]；另有最高 $84.75B 股权融资计划（$40B ATM + $10B 巴菲特私募配售，2026-06）[低-中, GPUSmith 底稿]。
- Microsoft：表内发债相对克制，杠杆主通道在第二层（租赁承诺，见 §2.3）。

**Nvidia（新进入者）**
- **2026-06-15 发债 $25B**，2021 年以来首次，7 个档次最晚 2056 到期，订单 $85B vs 初始目标 $20B [中, [Reuters, 2026-06-15](https://www.reuters.com/business/finance/nvidia-raise-20-billion-source-says-first-corporate-bond-issuance-five-years-2026-06-15/)；[Bloomberg](https://www.bloomberg.com/news/articles/2026-06-15/nvidia-kicks-off-first-high-grade-bond-offering-since-2021)]。CFO Kress 同期披露：Nvidia 承诺总额"基本在 **~$124B**"（供应义务+投资承诺），长期债正是为这类需求设计 [低-中, [TIKR 转引 BofA 科技大会发言, 2026-06](https://www.tikr.com/de/blog/nvidia-just-raised-25-billion-in-its-biggest-bond-deal-ever-heres-what-it-signals-for-2026)]。**意义：循环中枢自身开始债务化**。

**CoreWeave（neocloud 样本）**
- 长期债务 $7.9B（FY24 末）→ $21.4B（FY25 末）；叠加 2026 年前 8 个月公布的新融资额度 ~$24.5B（$8.5B DDTL 4.0 + $4.0B 可转债 + $2.75B 优先票据等），总债务口径 ~$25B+ [低-中, [Mungomash 基于 SEC 文件, 2026-08-13](https://mungomash.com/orgs/coreweave/financials/)]；2026 年迄今股债合计融资 >$30B，其中无担保+可转债 >$10B [低-中, [ECM Source 引 8-K, 2026-09-12](https://ecmsource.com/nebius-group-4-5-billion-convertible-notes-ai-data-centers-august-2026/)]。
- 结构与成本：多层 DDTL（GPU+客户合同抵押）+ 优先债 + 可转债；早期私募信贷定价 10–15%，2026-03 的 DDTL 4.0（$8.5B）为首个获 IG 评级的 GPU 抵押贷（Moody's A3/DBRS A low，SOFR+225bp、~5.9% 固定，2032 到期，Blackstone 锚定）[中, [Sascha Steffen, 2026-08-14](https://www.sascha-steffen.de/updates/nvidia-500bn-ai-financing-credit-risk)；[低-中, Peony, 2026-08-19](https://www.peony.ink/blog/neocloud-capital-raise)]。Q2'26 利息费用 $640M（上年同期 $267M），年化 ~$2.6B [低-中, [CCIR, 2026-08-12](https://ccir.io/research/two-order-books)]。抵押品是贬值中的 GPU——这是第一层里评级与真实风险差距最大的部分。
- 另有经营性租赁负债 $10.1B（2026-03-31，非 GPU 固定义务）[低-中, [Milvern 引 10-Q, 2026-05-16](https://milvern.com/analysis/detail?ticker=CRWV)]。

**xAI**
- 2026 年初发行 ~$5B 债券+贷款补充现金；WSJ 估算 Colossus 2 仅芯片采购就需 $18B [中, [EnergyNow/Bloomberg, 2026-02](https://energynow.com/2026/02/the-3-trillion-ai-data-center-build-out-becomes-all-consuming-for-debt-markets/)；[WSJ, 2025-11-11](https://www.wsj.com/tech/ai/three-ai-megadeals-are-breaking-new-ground-on-wall-street-896e0023)]。私人公司，披露不全，实际杠杆高于可见值。

### 1.3 "$1.2T 成 IG 最大板块"的构成分解

- 宽口径构成（M&G/JPM/Goldman 口径拼图）：**超大规模厂商债约占 40%**（Goldman 追踪 ~$500B 发行中 hyperscaler 占 40%），其余为：公用事业/电力（数据中心供电链）、电信/光纤、房地产/数据中心 REIT、芯片与硬件链、neocloud [中, Goldman 2026-08-05 上引]。
- 评级分布：头部（MSFT/GOOGL/AMZN/META/NVDA）AA–AAA 区间；Oracle Baa2/BBB 为尾部；SPV 债（Hyperion A+、DDTL 4.0 A3）构成新的中间层。
- 期限结构：本轮发行显著长久期化——Hyperion 2049 到期、Nvidia 2056、Amazon 30 年期增发；发行人锁定利率，**把技术迭代风险转移给了久期买家（保险/年金）**。

---

## 二、第二层：表外/准隐形债

### 2.1 SPV 旗舰：Meta Hyperion

- 结构：SPV "Beignet Investor LLC"，Blue Owl 基金 80% / Meta 20%；Morgan Stanley 安排 ~$27.3B 债 + ~$2.5–3B 股权；**债券 A+（S&P），发行收益率 6.58%，2049 到期、全额摊还**；PIMCO 锚定 ~$18B，BlackRock >$3B；股权出资 Meta $5.8B vs Blue Owl $23.0B [高, [Meta IR, 2025-10-21](https://investor.atmeta.com/investor-news/press-release-details/2025/Meta-Announces-Joint-Venture-with-Funds-Managed-by-Blue-Owl-Capital-to-Develop-Hyperion-Data-Center/default.aspx)；中, Sascha Steffen 上引；低-中, [Global Data Center Hub, 2026-07-20](https://www.globaldatacenterhub.com/p/the-hyperion-financing-is-the-signal)]。债务不上 Meta 表。
- 项目口径漂移：$27B（JV 融资）/ ~$30B（总开发成本）/ **>$50B**（2026-07-13 确认扩至 5GW、3,200 英亩）[低-中, [Global Data Center Hub](https://www.globaldatacenterhub.com/p/meta-scales-hyperion-to-5gw-and-over)]。
- **关键回表通道**：Meta 向 JV 提供**前 16 年运营的残值担保**——租约不续或提前终止时 Meta 现金补足差额。债务在表外，下行风险在表内（见 §三）[低-中, [FlowVerify, 2026-06-29](https://www.flowverify.co/blog/hyperscaler-ai-data-center-leases-off-balance-sheet)]。

### 2.2 其他 SPV 与"影子债务"总量

- **Apollo/Blackstone "Compute SPV"（2026-06）**：Atlas SP Partners 设立单一目的载体发行 **$35B** 债，购芯片后租给 Anthropic 五年，以租约现金流定价为类 IG——史上最大私募信贷交易之一，"Anthropic 的租约被做成了债" [低-中, [Vector/The Economist 转述, 2026-06-10](https://vector.news/ais-risk-goes-off-the-books-but-still-lurks/)]。**这是第二层的新范式：把第三层的客户承诺直接证券化为第二层的债。**
- 科技巨头表外"影子债务"累计 ~$120B（含 Meta Hyperion、xAI、Oracle 相关 SPV 等）[低-中, [Futunn, 2025-12-26](https://news.futunn.com/en/post/66651650/120-billion-usd-in-phantom-debt-unveiling-the-other-ledger)；[techerati, 2026-01-02](https://www.techerati.com/features-hub/ais-hidden-price-tag-record-debt-and-off-balance-sheet-financing/)]——**逐家分解无权威公开版**，可辨识锚点：Hyperion ~$27B、Compute SPV $35B、CoreWeave DDTL 系列的 SPV 部分、xAI 相关载体，其余为中小项目融资。
- Morgan Stanley 估算 2025–2028 年数据中心**表外融资总量 ~$800B**（含私募信贷、SPV、证券化）[低-中, [Joe Toppe/LinkedIn 引 MS, 2026-05-27](https://www.linkedin.com/pulse/800-billion-bet-how-ai-data-centers-being-financed-where-joe-toppe-rfaoe)]。

### 2.3 未生效租赁与合同承诺（Q2'26 财报季大幅上跳）

- **Meta**：未生效经营/融资租赁承诺 $182.9B（2026-03-31）→ **$279.0B**（2026-06-30，单季 +52%）；另有不可撤销合同承诺 $349.3B（多为云与基础设施采购，Q1'26 电话会曾披露单季新增 $107B）；7 月再签 ~$68B 租赁（2027–28 起租）[高, [Meta Q2'26 10-Q](https://www.sec.gov/Archives/edgar/data/1326801/000162828026050705/meta-20260630.htm)；中, [Business Insider, 2026-07-30](https://www.businessinsider.com/meta-future-ai-data-center-leases-quarter-trillion-dollars-2026-7)]。
- **Microsoft**：未生效租赁承诺总额 $329.1B（Q2'26）；Meta+Microsoft 单季合计新增 >$120B [低-中, [AI Weekly/Bloomberg, 2026-07-30](https://aiweekly.co/alerts/metas-q2-filing-piles-more-billions-onto-ai-lease-stack)]。
- **Alphabet**：未生效租赁 $85.2B（Q2'26 10-Q）[低-中, [Otto Analytics 引 10-Q](https://ottoanalytics.ai/ai-capacity)]。
- **全行业口径**：未生效数据中心租赁承诺合计 **>$850B**（2026 年中）[低-中, [mlq.ai, 2026-06-25](https://mlq.ai/news/meta-and-microsoft-add-120b-in-lease-commitments-in-one-quarter-industry-total-tops-850b/)]；另一口径"超大规模厂商隐藏租赁债 $662B"（FlowVerify 2026-06-29，仅 lease、时点更早）——差异来自公司集合与是否含采购承诺。
- 性质：GAAP 下起租前不进表、不计利息，但**是带期限的固定付款义务**，经济实质等同债务；起租后将以租赁负债形式逐季回表。

### 2.4 私募信贷直接放贷

- GPU 抵押贷定价从 2024–25 年的 10–15% 压缩至 2026 年 IG 级 SOFR+225bp（CoreWeave DDTL 4.0）——利差压缩本身就是"风险被评级外衣重定价"的信号。
- 数据中心/AI 基建已成为私募信贷最大单一主题之一；Morgan Stanley $800B（2025–28 表外总口径）中私募信贷为主体部分。BDC/私募信贷载体是 §三 或有负债的最终承接层之一（对照 `../crash-dynamics/02-subprime-2007-08-anatomy.md` §六"谁是本轮 Reserve Primary"）。

---

## 三、第三层：或有负债（承诺、担保与"不能算资产的预期"）

### 3.1 供应商侧的兜底与股权投资承诺

- **NVDA–CoreWeave $6.3B 容量兜底**：Nvidia 须购买至 **2032-04** 的未售云容量——写在 neocloud 链条上的看跌期权，行权人是 CoreWeave 的债权人 [中, [Investopedia, 2025-09-15](https://www.investopedia.com/coreweave-stock-pops-on-6-3b-nvidia-deal-11810215)]。
- **NVDA→OpenAI**：$100B LOI（2025-09-22）于 2026-02 正式放弃，改为在 OpenAI $110B 融资轮中敲定 **$30B** 股权投资（2 月底注入）；黄仁勋 2026-03-04 称 $100B "probably not in the cards"、$30B 或为 IPO 前最后一笔 [中, [FT, 2026-02-19](https://www.ft.com/content/dea24046-0a73-40b2-8246-5ac7b7a54323)；[Reuters, 2026-02-20](https://www.reuters.com/business/nvidia-close-finalizing-30-billion-investment-openai-funding-round-ft-reports-2026-02-20/)；[Stocktwits, 2026-03-05](https://stocktwits.com/news-articles/markets/equity/nvidia-huang-says-30b-openai-investment-may-be-last-pre-ipo-deal/cZd9vW8RIdI)]。另有 2026-08 报道称 Nvidia 为 OpenAI 俄亥俄项目提供最高 $105B 担保 + $1.5B 投资——**单源、未获主流确认，列为待核** [低-中, [Baptista Research, 2026-08-18](https://baptistaresearch.com/nvidia-openai-deal-ai-demand/)]。
- Nvidia 2026 年前 4 个月 AI 股权投资承诺 >$40B（$30B OpenAI + Corning ≤$3.2B + IREN $2.1B 权证 + Nebius $2B 附 5GW 部署承诺等）[中, [TNW, 2026-05-10](https://thenextweb.com/news/nvidia-40bn-ai-equity-investments-2026)]；CFO 口径承诺总额 ~$124B（§1.2）。
- **Meta 残值担保**：Hyperion JV 前 16 年残值兜底（§2.1）——SPV 债的 A+ 评级实质上是 Meta 信用通过担保条款的外溢。

### 3.2 take-or-pay、完工担保与流动性支持函

- neocloud 收入的 98% 来自多年期 take-or-pay 合同（CoreWeave 10-Q 口径）——**对客户（OpenAI/Microsoft/Meta）是无论用不用都得付的承诺**；Meta 一家对 CoreWeave 的累计承诺已 >$35B（含 2026-04-09 的 $21B/2027–32 合同）[中, [Morningstar, 2026-04-13](https://www.morningstar.com/stocks/coreweave-21-billion-meta-commitment-is-cornerstone-continuous-high-growth)]。
- 数据中心项目融资普遍含完工担保（completion guarantee）与母公司流动性支持函；诉讼风险已在积聚（工期延误、成本超支的追责链）[中, [Quinn Emanuel, 2026-03-13](https://www.quinnemanuel.com/the-firm/publications/client-alert-emerging-litigation-risks-in-financing-ai-data-centers-boom/)]。

### 3.3 RPO 的反向视角：供应商的 backlog = 客户的承诺支出

- Oracle RPO $638B（Q4-FY26），其中 ~$300B 来自 OpenAI（$300B/5 年合同，2027 起 ~$60B/年）[中, [IntuitionLabs, 2025-11-30](https://intuitionlabs.ai/articles/oracle-openai-300b-deal-analysis)；Oracle IR 上引]。
- Microsoft 云 RPO $625–627B，~45% 来自 OpenAI（$250B Azure 承诺至 2032）[中, [GeekWire, 2025-10-28](https://www.geekwire.com/2025/microsoft-secures-27-stake-in-openai-in-new-deal-with-commitment-for-250b-in-azure-usage/)；[BetaFinch, 2026-05-01](https://betafinch.com/blog/big-tech-anthropic-openai-revenue-q1-2026)]。
- CoreWeave 合同收入 backlog **$104B**（2026-08）[低-中, ECM Source 上引]。
- **反向读法**：RPO 对供应商是"已锁定收入"（且被拿去抵押融资——CoreWeave 的 DDTL 即以合同为锚），对付款方则是尚未进表的承诺支出。**OpenAI 站在所有 RPO 的对面**：可核验承诺 $1.15T（Tom Tunguz 口径，七家供应商明细见底稿 §5）至 $1.4T（含 Stargate 扩容名义值，WSJ 2026-08 报道其收入不及预期、承诺承压）。这部分"预期"在供应商资产负债表上支撑了第一层与第二层的真实债务，但对 OpenAI 自己**既不算资产也不算负债**——它是全结构中最薄的那张纸。

---

## 四、三层总量估算表

| 层 | 口径 | 区间（2026-09 时点） | 可信度 | 备注 |
|---|---|---|---|---|
| **第一层 显性债** | AI 相关债务存量（宽口径，含电力/电信链） | **~$1.2T** | [中]（M&G 单源，构成可交叉验证） | IG 最大板块；科技公司占 ~40% |
| | 其中：五大+Oracle+Nvidia+neocloud 可辨识表内债 | **~$550–700B** | [中]（逐家加总，推断） | Oracle $174.5B 总负债 + Meta $83.7B 长债 + 其余各家存量 |
| | 2026 年发行流量（AI 相关全球） | **$500–570B**（全年预测） | [中]（MS/JPM/GS 收敛） | H1 已落地 ~$250–300B |
| **第二层 表外/准隐形** | 已落地 SPV/影子债务 | **~$120–150B** | [低-中]（聚合口径，无逐家权威版） | Hyperion $27B + Compute SPV $35B 为锚 |
| | 未生效租赁+采购承诺（全行业） | **~$850B–1T** | [中]（Meta/MSFT/GOOGL 为 10-Q 一手，外推部分低） | Meta $279B+$349B、MSFT $329B、GOOGL $85B |
| | 表外融资管道（2025–28 累计预测） | **~$800B** | [低-中]（MS 估算转引） | 含未落地项目，非存量 |
| **第三层 或有负债** | 可核验承诺名义值（OpenAI 中心环路 + NVDA 兜底/投资 + 担保类） | **~$1.1–1.4T 名义** | [中]（合同可核验部分）/ [低-中]（扩容与担保部分） | **名义值 ≠ 风险敞口**；违约情景下实际损失是名义值的折扣 |
| | 其中 NVDA 敞口（兜底 $6.3B + 已投/承诺股权 $40B+，总承诺 ~$124B） | **$46–124B** | [中] | 区间宽因"承诺总额"构成未完全披露 |

**读表警告**：三行**不可直接相加**。第一层含第二层抵押支撑的部分债务（DDTL 以第三层合同为锚）；第二层的租赁承诺起租后将迁移进第一层；第三层是前两层部分债务存在的理由而非独立敞口。若坚持要一个"总涉及名义值"，~$3T 量级（对应"The $3 Trillion AI Data Center Build-Out"的媒体口径 [中, EnergyNow/Bloomberg 2026-02]），但其中真实的风险加权敞口远小于此——见 §五。

---

## 五、口径陷阱（本篇最容易读错的地方）

1. **承诺不是债**。Meta $279B 未生效租赁、OpenAI $1.15T 采购承诺、Nvidia $124B 供应义务，在 GAAP 下都不是负债。它们只在三种情况下变成真实现金压力：起租/交付、对手方违约触发担保、或再融资链条断裂迫使承诺方提前兑现。把所有承诺当债务加总会**高估存量、但低估触发时的跳变速度**——这些数字的特征是台阶式兑现，不是渐变。
2. **重复计算的三层叠加**。同一美元可出现三次：Nvidia 投 OpenAI $30B（第三层）→ OpenAI 用其对 Oracle/MSFT/CoreWeave 的采购承诺进入对方 RPO（第三层另一侧）→ 供应商以 RPO 为锚发债或设 SPV（第一/二层）。媒体口径的"$1.4T 循环"已经把这种叠加算进去了，再加总一次就是双重计算。
3. **名义 vs 风险**。Hyperion $27.3B 债对 PIMCO 是 A+ 摊还债券，对 Meta 的**风险**只是残值担保的尾部（前 16 年、特定触发条件）；CoreWeave $104B backlog 的名义值依赖 OpenAI/Microsoft 履约能力，集中度使"评级"与"真实信用"脱节（A3 的 DDTL 底层是同一批循环合同）。
4. **RPO 不是资产**。对供应商，RPO 是收入预期的记账科目，不能抵押、不能变现（除非像 CoreWeave 那样以合同融资）；对客户，它是承诺支出。Oracle 市值把 $638B RPO 当"已锁定收入"定价，而其中 ~47% 的信用来自一家收入覆盖率 1:30 的公司（主报告 §2.4）——这是"交易对手信用被叙事替代"的计价。
5. **净发行 vs 毛发行、科技 vs AI 宽口径**。2026 年发行预测从 $175B（Fortune 五大口径）到 $570B（MS 全球 AI 相关）相差 3 倍，全部可以各自成立。引用时必须先问：谁的公司集合、毛还是净、含不含电力链。
6. **未提取额度 vs 债务余额**。CoreWeave "~$25B 总债务"含 DDTL 已提取部分；其公布的新融资"额度"（~$24.5B）大部分尚未提取——额度在客户合同撤销时不会自动变成债，但已提取部分的抵押品（GPU）在贬值。

---

## 六、结构对照：2000 年电信 vs 2007 年 SIV（参见 `../crash-dynamics/01`、`02`）

**与 2000 年电信的同构**（vendor financing 层）：
- 机制相同：设备商/供应商向客户输血购买自家产品——Lucent/Nortel→WorldCom 之于 Nvidia→OpenAI/neocloud。Oxford Economics 等已作此类比（底稿 §3）。
- 分布不同：2000 年烧钱主体（电信运营商）的债在表内且为 HY；本轮烧钱主力 OpenAI 在一级市场，上市公司侧以 IG+SPV 承接，**评级更高、链条更长、穿透更难**。2000 年你在债券募集书里能看到 WorldCom；2026 年你在 PIMCO 持有的 A+ 2049 年摊还债券里看到的是"路易斯安那电力资产"，OpenAI 三个字不出现。

**与 2007 年 SIV 的同构**（表外层，对照 crash-dynamics/02 §六）：
- SIV 的教训是**"表外"只是会计状态，不是风险状态**：SIV 有母行流动性支持函，危机时风险全部回表（Citibank 2007-12 被迫并表 $49B SIV）。Hyperion 的残值担保、Compute SPV 的租约依赖、DDTL 的合同抵押，都是同族结构——**发起人用担保条款换取不并表，评级机构按担保方信用给评级，但资产端的真实风险（GPU 迭代、单一客户）留在结构里**。
- 关键差异（本轮更"结实"的部分）：Hyperion 是**全额摊还、久期匹配**（2049 债对长期租约），没有 SIV 的短融长投错配；买家是保险/年金（持有至到期），不是货基——挤兑机制弱于 2007。
- 关键差异（本轮更脆弱的部分）：SIV 的底层是分散的房贷池，本轮 SPV 的底层是**单租户/单客户合同**——分散化幻觉反过来成立。且隐性担保方高度集中：Nvidia 一家同时是供应商、股权投资人和容量兜底人（crash-dynamics/02 §六的"谁是本轮 AIG"判据：谁的承诺被对手方计入资本充足性——答案是 Nvidia 与 OpenAI 互为对方的 AIG）。
- 急性期映射：若破裂，第二层的回表路径不是挤兑而是**触发式**——残值担保行权、take-or-pay 违约、completion guarantee 追责（Quinn Emanuel 已在记录诉讼前兆）。监测优先级：SPV 债利差（Hyperion 2029 年起摊还进度）、DDTL 抵押品重估、BDC 赎回窗口——引擎信号早于主体名单 2–4 周（crash-dynamics/02 §六.5）。

---

## 主要来源（节选）

- [高] Oracle IR（CY2026 融资计划 2026-02-01；FY26 财报 2026-06-10）；Meta Q2'26 10-Q/8-K（2026-07-29/30）；Meta IR（Hyperion JV 2025-10-21）；Oracle 424B2（2026-02-02）
- [中] Reuters（MS $570B 预测 2026-06-10；NVDA $25B 债 2026-06-15；NVDA-OpenAI $30B 2026-02-20）；FT（$100B LOI 放弃 2026-02-19）；Bloomberg/EnergyNow（$3T 口径 2026-02）；JPM AM（2026-08-05/08-20）；Goldman Sachs Exchanges（2026-08-05）；M&G（$1.2T 存量 2026-03-04）；Fortune（需求裂缝 2026-07-17）；Business Insider（Meta Q2 租赁 2026-07-30）；Morningstar（Meta-CoreWeave $21B 2026-04-13）；Quinn Emanuel（诉讼风险 2026-03-13）；Sascha Steffen（NVDA 债务机器信用分析 2026-08-14）
- [低-中] Deepstory Research（2026 发行人明细 2026-08-06）；Mungomash（CoreWeave 债务结构 2026-08-13）；CCIR（neocloud 资金成本 2026-08-12）；ECM Source（CoreWeave $30B YTD 2026-09-12）；Global Data Center Hub（Hyperion 扩产/股权明细 2026-07-20）；FlowVerify（$662B 租赁+残值担保 2026-06-29）；mlq.ai（行业 $850B 2026-06-25）；Futunn/techerati（$120B 影子债务）；Universal Asset Owners（H1 发行 2026-07-01）；Vector（Compute SPV 2026-06-10）；TIKR（Kress $124B 承诺 2026-06）

## 修订记录

- **2026-09-18**：初稿（debt-web 系列第 1 篇）。
