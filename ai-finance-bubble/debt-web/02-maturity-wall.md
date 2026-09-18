# 到期墙与再融资周期：AI 债务"什么时候爆"的时间结构

撰写日期：2026-09-18｜系列：debt-web 02/07

> 本篇回答"什么时候爆"：不预测引信（见 `crash-dynamics/03-acute-crash-playbook.md` §1：引信不可预测），而是绘制**再融资需求的日历**——哪个季度有多少债必须回到市场、按什么价格。利率基准（2026-09-16/17）：联邦基金 3.75–4.00%（9/16 加息 25bp 落地，点阵图指向 12 月再加）、10Y 5.00%、30Y 5.34%、HY OAS 2.65%（9/11）、IG OAS ~77bp（背景状态，见 `watch/macro/2026-09-17-fomc-hike-review.md`）。SOFR 推算约 3.85–3.90%。可信度三级：[高]=官方/一手文件，[中]=主流财经媒体/具名机构，[低-中]=中小博客/聚合站。口径冲突并列。

---

## 1. 逐主体到期墙（2026Q4–2030）

### 1.1 CoreWeave：不是一堵墙，是"浮动利率持续重定价 + 2029–32 子弹集群"

**存量结构（截至 2026-03-31 10-Q，总债务净额 $24.86B）**——[CoreWeave Q1'26 10-Q，转引自 AI Infrastructure Financing 报告， 2026-07-20 核验 [高/中]](https://ai-physical-infra-debt-analysis.vercel.app/)：

| 层级 | 规模 | 定价 | 到期/特征 |
|---|---|---|---|
| DDTL 1.0（2023-07） | 余额 $1.44B | **15% 有效利率** | 高成本私募信贷遗留，按月摊还 |
| DDTL 2.0（2024-05） | 余额 $4.43B | SOFR+6.0%~13.0%（按客户信用分层），11% 有效 | 按月摊还 |
| DDTL 2.1（2025-09） | 余额 $3.0B | SOFR+4.25%，9% 有效 | 按月摊还 |
| DDTL 3.0（2025-07，OpenAI 合同） | 余额 $1.7B | SOFR+4.00%，9% 有效 | 母公司担保 |
| OEM/软件许可融资 | 余额 $5.0B | 10% 有效 | 与硬件采购同步到期 |
| DDTL 4.0（2026-03-30） | $8.5B 承诺 | **SOFR+2.25% 浮动**（0% 下限）+固定利率公式档（媒体报 ~5.9%） | **2032-03-31 到期**；非追索（仅 bad-acts 例外）、DSCR 1.15x；媒体报道 A3/A(low)、Blackstone 锚定（8-K 未点名客户/评级/锚定人）；**承诺提款期 2027-06 终止** |
| DDTL 5.0（2026-05-15） | $3.1B | SOFR+4.50%（银团中收窄 50bp） | **2031-11-15 到期**；Ba2/BB+；两个非 IG 客户；首个公开银团 HPC 抵押贷 |
| DDTL 5.5（2026-08-10） | $2.6B | **SOFR+5.50%** | 到期日未披露（按系列惯例约 5.5 年 → ~2032 初）；JPMorgan/MUFG 安排 |

来源：[CoreWeave 8-K/新闻稿， 2026-03/05 [高]](https://www.stocktitan.net/sec-filings/CRWV/8-k-core-weave-inc-reports-material-event-0b56fb496fc5.html)；[CoreWeave DDTL 5.5 新闻稿， 2026-08-10 [中]](https://lasvegassun.com/news/2026/aug/10/coreweave-closes-26-billion-loan-facility-expandin/)；[ai2.work, 2026-04-24 [低-中]](https://ai2.work/blog/coreweave-s-8-5b-gpu-loan-exposes-the-ai-debt-treadmill)；[tech-insider, 2026-09-04 [低-中]](https://tech-insider.org/volta-ai-cloud-deal-coreweave-debt-2026/)

**无担保子弹层**（这才是教科书意义的"到期墙"）：
- 9.250% 优先债 **2030-06 到期**（$2B，2025-06 发行）；
- 可转债 $2.25B @1.75%，**2031-12-01 到期**（2025-12 发行）— [CoreWeave 8-K, 2025-12-08 [高]](https://www.sec.gov/Archives/edgar/data/1769628/000176962825000105/crwv-20251208.htm)；S&P 评级 B [S&P, 2025-12-10 [高]](https://www.spglobal.com/ratings/en/regulatory/article/-/view/type/HTML/id/3492923)；
- 可转债 $3.5B，**2032-10-01 到期**（2026-04-10 定价）— [CoreWeave 新闻稿, 2026-04-10 [高]](https://investors.coreweave.com/news/news-details/2026/CoreWeave-Prices-Upsized-3-5-Billion-Convertible-Senior-Notes-Offering/default.aspx)；
- 9.750% 优先债 **2031-10-01 到期**（定价时 $1.0B，2026-04-16）— [CoreWeave 新闻稿 [高]](https://investors.coreweave.com/news/news-details/2026/CoreWeave-Announces-Pricing-of-1000-million-of-9-750-Senior-Notes-due-2031/default.aspx)；**口径冲突**：SanCap 记 4 月该笔为 $2.75B/9.75% 5 年期 HY 发行（可能含后续增发）[SanCap, 2026-05-08 [中]](https://portfolio-strategy.apsec.com/2026/05/08/special-report-risk-and-reward-as-data-centers-tap-the-debt-markets/)。

**结构解读**：CoreWeave 的 DDTL 全部按月摊还——没有单笔悬崖，但有两个更隐蔽的风险：(a) **浮动利率部分（余额 $15B+）每季度随 SOFR 重定价**，9/16 加息直接抬升当期利息，无需等到任何"到期日"；(b) 摊还曲线 vs 抵押 GPU 价值曲线的交叉点（§3）。真正的子弹集群在 **2030-06 至 2032-10**：约 $8.75B 无担保债 + DDTL 5.0/4.0 到期尾款，全部落在 30 个月内。2026 capex 指引 $30–35B、预期 FCF ~-$18.8B（research-01 §2），意味着**展期不是选项而是生存前提**。FY2025 利息净额 $1,229M（另有 $159M 资本化），EBITDA 口径利息覆盖 1.96x、全口径 1.73x [MetricDuck 基于 10-K, 2026-03-17 [低-中]](https://www.metricduck.com/blog/crwv-10k-168-pct-revenue-growth-070x-debt-service-coverage)——覆盖倍数 <2x 意味着利率每 +100bp 都是利润表事件。

**数据缺口**：Q2/Q3'26 10-Q 后的全量到期阶梯（公开可得的是 Q1'26 余额）；DDTL 5.5 到期日与摊还表；各 DDTL 的逐年摊还本金表（未公开）。

### 1.2 其他 neocloud：墙更矮但更脆（可转债依赖股价）

- **Nebius**：五个月内举债 ~$8.8B [SERVOLA, 2026-08-21 [低-中]](https://servola.de/journal/nebius-borrows-another-4-5bn-to-keep-the-gpu-bet-going/)。构成：可转债 $4B（2026-03-19：$2.25B @1.250% **2031 到期** + $1.75B @2.625% **2033 到期**）[LinkedIn/Leo Gergs, 2026-03-30 [低-中]](https://www.linkedin.com/pulse/lifestyles-rich-famous-bank-of-america-doubles-down-neoclouds-coreweave-down-50-post-gtc-nebius-prices-4b-convertibles-xfwee)；**首笔有担保债 $775M @SOFR+2.50%，2030-10-31 到期**（2026-07-17）[Nebius/SEC, 2026-07-17 [高]](https://www.sec.gov/Archives/edgar/data/1513845/000110465926084452/tm2620683d1_ex99-1.htm)；可转债 $5.0B（2026-08-19 定价：$3.0B @0.50% **2030 到期** + $2.0B @4.50% **2034 到期**）[Coloprice, 2026-08-20 [低-中]](https://coloprice.com/guides/nebius-5-billion-convertible-notes/)。结构特征：**子弹式为主、票息极低、偿付依赖转股**——本质是股权期权融资；若股价跌破转股价值预期，2030/2031 两笔 $5.25B 将以现金到期撞上再融资市场。
- **Lambda**：2026-08 完成 $1B 私募债（为 Microsoft 合同购 Nvidia GPU，GPU 抵押）[BigGo Finance, 2026-08-30 [低-中]](https://finance.biggo.com/news/f3f546f1-49df-4e7e-985f-238bcc820952)。到期条款未公开——**数据缺口**。
- **Crusoe**：$750M Brookfield 信贷额度（2025-06）[Crusoe, 2025-06-11 [高]](https://www.crusoe.ai/resources/newsroom/crusoe-secures-usd750-million-credit-facility-from-brookfield-to-accelerate)；条款未公开——**数据缺口**。
- **Applied Digital**（上市、可追踪的摊还结构样本）：$2.35B @9.250% 优先担保摊还债（2025-11）[APLD IR, 2025-11-13 [高]](https://ir.applieddigital.com/news-events/press-releases/detail/136/applied-digital-announces-pricing-of-2-35-billion-of)；$2.15B（2026-03，Polaris Forge 2，数据中心租约关键节点后每半年摊还）[Globe and Mail/APLD, 2026-03-11 [中]](https://www.theglobeandmail.com/investing/markets/stocks/APLD-Q/pressreleases/702463/applied-digital-completes-2-15-billion-senior-notes-offering/)；$1.59B @7.000% 优先担保债（2026-06，用于偿还 Goldman 过桥贷）[StockTitan, 2026-06-09 [中]](https://www.stocktitan.net/news/APLD/applied-digital-announces-pricing-of-1-59-billion-of-senior-secured-qb729o5rn7zn.html)。注意成本轨迹：9.25% → 7.00% 改善，但前提是租约签署落地。
- 行业观察：可公开查到的 merchant GPU cloud 到期表"2026 年聚集、2027 更大、尾部延至 2028" [Medium, 2026-05-05 [低-中]](https://medium.com/@Elongated_musk/the-neocloud-refinancing-wall-is-the-cleanest-risk-in-ai-infrastructure-c6b2afb17c1e)——方向与本文独立核验一致，但具体金额以发行人文件为准。

### 1.3 Oracle：墙不高但"到期 + 新增"叠加，且单一客户风险在 RPO 里

FY2026 10-K（截至 2026-05-31）到期阶梯，全部借款本金合计 **$130.1B** [Oracle 10-K, 2026-06-22 [高]](https://www.sec.gov/Archives/edgar/data/1341439/000119312526277521/orcl-20260531.htm)：

| 财年（至 5/31） | 到期本金 |
|---|---|
| FY2027 | **$7.21B**（其中 $5.7B 已在 FY26 重分类为流动负债） |
| FY2028 | **$10.15B** |
| FY2029 | $5.50B |
| FY2030 | $7.25B |
| FY2031 | $9.75B |
| 此后 | $90.25B（最远至 2066） |

要点：(a) 到期分布本身平缓（Fitch："阶梯式到期至 2065"，BBB/稳定，2026-02-02 [高](https://www.fitchratings.com/research/corporate-finance/fitch-rates-oracle-senior-notes-offering-bbb-affirms-idr-outlook-stable-02-02-2026)）；(b) **真正的压力是叠加项**——FY26 已发 $43.0B 优先债（票息 4.45%–6.85%，含 $0.5B 浮息 2029-02 到期）+ $5.0B 强制转优先股 @6.50%，FY27 计划再融 ~$40B 债+股（research-01 §2，Octus 2025-11 [中]）；(c) 存量到期券多为低利率年代发行（例：4.80% 2028-08-03 到期券，当前收益率 5.04% [Public.com, 2026-03-09 [低-中]](https://public.com/bonds/corporate/oracle-corp/orcl-4.8-08-03-2028-68389xcy9)），重定价方向单向向上；(d) 10-K 另披露 $260B 表外数据中心租赁承诺（FY27Q1 起陆续生效，15–19 年期）——债表之外还有一层准债务久期。反向意见如实记录：AInvest 称"到期墙是迷思、现金流才是真问题"（FY26 经营现金流 $32B）[AInvest, 2026-07-11 [低-中]](https://www.ainvest.com/news/oracle-debt-wall-myth-cash-flow-problem-real-2607/)——两读法不矛盾：墙是平的，但墙前站着 $55.7B/年且还在涨的 capex。

### 1.4 Meta Hyperion SPV（Beignet）：摊还型，墙的答案在"租约 vs 摊还表"

- $27.3B **6.581% 优先担保摊还债，2049-05 到期**，T+225bp，A+（S&P 初步评级，2025-10-16 [高](https://www.spglobal.com/ratings/en/regulatory/article/-/view/sourceId/101651795)）[Chavez Calva, 2026-08-27 [中]](https://joseluischavezcalva.substack.com/p/residual-exposure-in-the-ai-data)；PIMCO 锚定 ~$18B，定价时收益率被买至 5.68% [FT, 2025-10-30 [中]](https://www.ft.com/content/d0344253-b0a2-4c6d-8b97-520243678afd)。
- **偿付链条**：Meta 租赁实体 Pelican Leap 与 Laidley 签 **4 年租约、2029 年起付租**，租金经 JV 流向 Beignet 偿还本息 [富途/Odaily, 2026-07-29 [低-中]](https://news.futunn.com/en/post/76756890/building-on-the-edge-of-a-cliff-the-debt-that)。即：**23.6 年摊还债由 4 年初始租约启动**——续约权是整笔债的命门（详见 §3 第三层）。
- **续作已遇阻**：第二单 Sopaipilla（Meta/BlackRock JV，El Paso 960MW）2026-07-27 定价 $12.547B @**7.534%、T+287.5bp**，2048-11 到期 [Yahoo/IFR, 2026-07-28 [中]](https://ca.finance.yahoo.com/news/investors-dig-12-5b-data-134615348.html)；IFR 标题直言"债券市场开始质疑 AI 繁荣，Beignet 续作遇冷" [IFR, 2026-07-31 [中]](https://www.ifre.com/bonds/2463746/bond-market-begins-to-question-ai-boom-as-beignet-sequel-falls-flat)。**九个月内同结构资产利差 +62.5bp、票息 +95bp——这是 AI 债重定价最干净的实证锚。**

### 1.5 私募信贷软件贷款：2027 开闸、2028 主峰

- Morgan Stanley（引 PitchBook）：直接贷款中软件借款人 **11% 2027 年到期、20% 2028 年到期**；AI 颠覆叠加到期墙，私募信贷违约率或达 8%（疫情以来峰值）[Firstpost/MS, 2026-03-17 [中]](https://www.firstpost.com/business/private-credit-default-rates-may-hit-8-as-ai-disruption-strains-software-loans-morgan-stanley-13990285.html)。
- Apollo：**2028 年软件债到期墙 ~$40B**，以 B- 级为主 [Apollo Academy, 2026-03-12 [中]](https://www.apolloacademy.com/software-maturity-wall/)。
- Fitch：再投资期内 BSL CLO 对 2028 年到期的软件贷款平均敞口 4.9%（区间 0.7%–12.7%）[Fitch, 2026-05-12 [高]](https://www.fitchratings.com/research/corporate-finance/software-maturity-wall-poses-challenge-for-us-bsl-clos-12-05-2026)。
- Moody's：BDC 2028 到期墙风险 [Bloomberg, 2026-04-22 [中]](https://www.bloomberg.com/news/articles/2026-04-22/private-credit-bdcs-2028-maturity-wall-poses-risk-moody-s-says)；Reuters 口径：$84B BDC 资产中今年仅 $15B 到期，**主体峰值在 2028–29** [Reuters via Capital Refinery, 2026-05-01 [中]](https://capitalrefinery.com/before-the-refinance-call)。
- 结构特征：直接贷款几乎全部**浮动利率（SOFR+500~650bp）、子弹式到期**——政策利率的传导无时滞，9/16 加息当季即体现在借款人利息账单上。MS 指出软件贷款已是"杠杆最高、覆盖率最低"的主要行业板块。

**跨主体小结**：2026Q4 几乎没有"必须偿还"的悬崖（BDC 口径今年仅 $15B）；墙从 **2027 年软件贷款开闸**开始爬坡，**2028 年多墙共振**（软件 $40B 主峰 + Oracle FY28 $10.1B + CoreWeave 摊还进入深水区），**2030–32 是 neocloud 无担保子弹集群**。

---

## 2. 再融资利率冲击的算术

**基准价格（2026-09 中）**：新发行定价 = 无风险利率 + 利差。10Y 5.00%、SOFR ~3.85–3.90%、HY OAS 2.65%、IG OAS ~77bp。对应档位：IG 10Y 新发行 ~5.8%；CoreWeave 级 HY（B1/B/BB-）straight debt ~9.75%（4 月实价）；GPU 抵押 DDTL S+2.25%~S+5.50%（视合同质量），全成本 ~6.1%–9.4%。

**实证锚（已在发生的重定价，非假设）**：
- CoreWeave DDTL 利差轨迹：**S+2.25%（3 月）→ S+4.50%（5 月）→ S+5.50%（8 月）**——五个月内同类抵押融资利差 +325bp。部分可解释为客户信用差异（DDTL 4.0 据报 A 级客户 vs 5.0/5.5 非 IG 客户），但方向与大盘一致；
- Beignet T+225 → Sopaipilla T+287.5（§1.4）；
- 9/16 加息 25bp + 点阵图指向 12 月再加（会后定价 ~50%）——浮动利率存量即时 +25bp，前瞻再加 25bp。

**敏感性表（每 $10B 受冲击本金的年度利息支出增量）**：

| 冲击 | 年利息增量（每 $10B） | 作用对象 |
|---|---|---|
| 基准利率 +100bp | **+$100M** | 全部浮动存量（DDTL ~$15B+、私募信贷软件贷、Oracle 浮息券）即时生效 |
| 基准利率 +200bp | **+$200M** | 同上 |
| 利差 +200bp | **+$200M** | 仅到期重定价/新发行部分 |
| +100bp 利率 + 200bp 利差叠加 | **+$300M** | 到期重定价部分的现实情景（对照：HY OAS 从 2.65% 回到 4% 即 +135bp） |

**代入主体的量级**：
- **CoreWeave**：浮动 DDTL 余额 ~$15B，+100bp = +$150M/年 ≈ FY25 利息净额（$1,229M）的 12%。若 2030–32 子弹集群（~$8.75B）按当前市场重定价——存量可转债票息 0.5–1.75% vs 新 straight debt ~9.75%——**利息增量的上限是 +$700M/年量级**（假设无法续发转债的极端情形）；中性情形（一半转股、一半按 9–10% 展期）约 +$350–400M/年。对照其 1.73x 的全口径利息覆盖，**+200bp 利率冲击即可把覆盖率压向 1x**。
- **Oracle**：FY27–28 到期 $17.4B，存量券票息多在 3–5%，按 ~5.8–6.2% 重定价 = **+$200–450M/年**；更大的项是 FY27 计划新增 ~$40B 债+股——若全债且按 6%+ 定价，年利息 ~$2.4B，较 FY26 发行平均票息（~5.5%）再贵 ~$200M/年。
- **私募信贷软件借款人**：直接贷款存量按 ~$1T 量级估，几乎全浮动，政策利率每 +100bp = **全行业 +$10B/年**利息负担，直接吃覆盖率最低的板块的 EBITDA。MS 的 8% 违约率预测即建立在此算术上。
- **财政部对照**：年借款 >$2T、年化利息已 ~$1.2T（CRFB，§4）——同样的算术在主权端同步运行，这是利差难以收窄的结构性原因。

**反方向证据（如实记录）**：HY OAS 2.65% 对加息纹丝不动（9/11 与两周前持平，见 `watch/macro/2026-09-17-fomc-hike-review.md` §一.4）；9/10 30Y 国债拍卖 b/c 2.61 创 2018 年来最强——市场仍在为一切融资，只是价格更高。**冲击目前体现在"价格"（利差与票息），尚未体现在"数量"（融资渠道关闭）。**

---

## 3. 久期错配：三层叠放，哪层先断

**第一层：GPU 抵押贷（债 5–6.5 年 vs 资产 3–5 年）。** DDTL 系列期限 5–6.5 年（2023-07 DDTL 1.0 → 2032-03 DDTL 4.0），按月摊还；抵押物 GPU 的经济寿命争议本身就是战场：CoreWeave 按 6 年直线折旧，Nebius 4 年、Lambda 5 年（research-01 §4）；Goldman 测算折旧年限从 5 年缩至 3 年，2026–31 累计折旧从 ~$3T 升至 ~$4T（单一假设 $1T 摆动）。抵押品市价正在验证短端：H100 时租 2026 年跌至 **$3.38/hr（"腰斩"标题）** [shattered.io, 2026-09-05 [低-中]](https://shattered.io/h100-h200-b200-cloud-gpu-pricing-2026/)，9/13 全市场 27 家加权均价 $3.84/hr [Mercatus, 2026-09-16 [低-中]](https://www.mercatus-ai.com/blog/gpu-rental-prices)；（**口径冲突，并列呈现**：research-04 §4 记 2026 年中 marketplace 价 $1.33–1.49、Silicon Data 指数 2025-12 为 $2.00——$3.38–3.84 为 9 月全市场加权/含 premium 档位口径且来源可信度低；两口径方向一致（下行）但水平值差一倍，引用时须注明口径。另见 05 篇"时租已崩、卡价未崩"裂口分析。）GPU 贷款预付率惯例 50–70% FMV，3 年后残值估算区间 10%–60%（分歧本身就是风险定价缺失的证据）[AI Infrastructure Financing, 2026-07-20 [中]](https://ai-physical-infra-debt-analysis.vercel.app/)。**这一层的断裂机制**：摊还表是线性的，抵押品价值是指数式衰减的（新架构每年一代），两者在贷款生命周期后段交叉——2023–24 年发放的早期 DDTL 恰在 2027–28 进入该区域。

**第二层：数据中心债（20–30 年 vs 租约 5–15 年）。** Beignet 摊还至 2049、Sopaipilla 至 2048；对照租户合同：Meta 对 Hyperion 的初始租约仅 **4 年**（2029 起算）；KBRA 租赁研究确认超大规模租约多为净租赁但**终止/缩容/转让条款是信用关键变量**，单一租户资产尤甚 [KBRA via AI Infrastructure Financing [中]](https://ai-physical-infra-debt-analysis.vercel.app/)。债是 23 年的，现金流合同是 4 年的，中间靠续约假设填充。

**第三层：技术迭代（2–3 年）。** GPU 架构已进入年度节奏（Blackwell→Rubin），训练负载向新一代迁移即压旧代租金（第一层数据的成因）；推理需求部分对冲，但 spot 市场成熟使旧卡价格发现更快。

**哪层先断的判断**：**第一层先断，但它断的方式是"信号"而非"违约潮"**——GPU 抵押贷摊还快、有合同现金流覆盖（DDTL 4.0 DSCR 1.15x），最先出现的是抵押率不足触发的**追加股权/结构重置**（2027–28），借款人是负 FCF 的 neocloud，追加能力有限 → 被迫出售资产或收缩 capex → 成为破裂链条的第一环（对应 `crash-dynamics/03` §2.1"杠杆最高者先死"）。第二层的断裂更慢但更贵：4 年租约的第一个续约决策点在 **~2033**（Hyperion），若届时 AI 需求证伪，23 年摊还债的残值风险全部落在保险/养老金持有人身上——这是"慢炖"层。三层的时间顺序：**浮动利率重定价（即时）→ GPU 抵押交叉点（2027–28）→ 无担保子弹集群（2030–32）→ 数据中心租约续约（2033+）**。

---

## 4. 与财政部抢久期：crowding out 的量化

衔接 `watch/macro/2026-08-26-us-debt-crisis-watch.md` §3.2"久期争夺"（该笔记的预警状态更新：**10Y >5% 已于 9/15 触发收盘 5.00%，30Y 5.34% 持续越线；Bessent 回购证伪；但拍卖需求仍强**——见 9/17 FOMC 重估）。

算术本身：
- **供给端**：财政部 FY2026 借款 >$2T（前 10 个月赤字 $1.8T，CRFB 2026-08-12 [高]）；AI 相关 2026 净发行 **$230B**（JPM，+76% YoY [中]）；AI 债存量 $1.2T、已是 IG 最大板块（M&G [中]）；财政部+AI 在同一 IG 买家池（保险、养老金、外资、债基）中竞标。
- **需求端**：外资上半年净增持美债仅 +$77 亿（同比 -98%）；买盘转向价格敏感的对冲基金/杠杆资金——**价格弹性买家占比上升 = 均衡利率对供给增量更敏感**。
- **量级判断**：$230B AI 净发行约为财政部借款的 11%，单独不足以 crowding out；真正的挤压是**久期段的重叠**——Beignet/Sopaipilla 这类 20–23 年摊还债直接落在 10–30Y 国债同一曲线段，与 $2T 长端供给争夺同一批年金/保险负债匹配资金。30Y 5.34% 的环境下，SPV 债定价只能随行就市（Sopaipilla T+287.5 即结果）。
- **均衡形态**（9/10 拍卖的启示）：需求没有消失，只是要求更高收益率——"价格发现正常但均衡利率上移"。对 AI 债务人，这意味着**融资渠道保持开放、但每一笔续作都在更高利率平台上成交**，压力以利息费用慢性累积而非突然断供的形式出现。这是与 2008 的关键差异，也是 `crash-dynamics/03` §3 速度谱系的含义：本轮这一层的破裂速度以**季度**计（摊还+重定价节奏），不是以日计。

---

## 5. 时点结论：再融资压力热力图与先行指标

### 5.1 时间热力图（2026Q4–2030）

| 窗口 | 热度 | 构成 |
|---|---|---|
| **2026Q4** | 🟡 黄 | 到期量极小，但**重定价与发行密度最高**：Oracle FY27 ~$40B 融资计划启动、Q3 财报季 capex 措辞检验（CHK-004，10 月下旬）、12/9 FOMC 再加概率 ~50%。风险形态是"利差先行"，不是"到期爆发" |
| **2027H1** | 🟠 橙 | 软件贷款 11% 到期开闸；Oracle FY27 $7.2B 到期兑付；DDTL 4.0 提款承诺期 6 月终止（CoreWeave 资金来源窗口关闭点）；早期 DDTL 摊还进入抵押品贬值加速区 |
| **2027H2–2028** | 🔴 **红——最危险窗口** | **多墙共振**：软件贷款 20%/$40B 主峰（B- 级为主）；Oracle FY28 $10.1B 到期 + FY27 融资计划的债务部分进入付息高峰；CoreWeave 早期 DDTL 摊还与 GPU 残值曲线交叉；若点阵图兑现，整个重定价发生在 4.00–4.50% 政策利率平台 + 财政部 $2T/年供给的利差环境中 |
| **2029–2030** | 🟠 橙（条件性升级） | Nebius $3.0B 转债 2030、CoreWeave $2B 9.25% 债 2030-06；Hyperion 2029 起付租（Beignet 偿付链正式上电）；Oracle FY30 $7.25B。若 2027–28 的重定价已抬高整个资本结构成本，此窗口从"橙"升级为"红" |
| **2031–2032** | ⚪ 未定 | CoreWeave 子弹集群主峰（转债 $2.25B 2031-12、9.75% 债 2031-10、DDTL 5.0 2031-11、DDTL 4.0 2032-03、转债 $3.5B 2032-10，合计 ~$15B+）；Nebius 2031/2033/2034。距今 5 年+，利率环境不可定价，仅登记日历 |

**核心结论**：到期墙的形态不是单一悬崖而是**三段式爬坡**——2026Q4–2027H1 的"价格重定价段"（已经在发生，利差证据确凿）、**2027H2–2028 的"数量到期段"（多墙共振，全周期最危险窗口）**、2030–32 的"neocloud 子弹段"（烈度取决于前两段的出清程度）。对应 `crash-dynamics/03` 的速度谱系：这一段链条的杠杆以季度频率重定价（浮动利率）+ 按月摊还，破裂形态更接近"电信式慢炖 + 信用利差先行"，而非 1987 式闪崩。

### 5.2 先行指标（按领先性排序，接入 watch 双刊监测）

1. **新发行利差轨迹**：CoreWeave DDTL 系列 S+2.25→S+4.50→S+5.50（2026-03/05/08）；下一笔 GPU 抵押贷或 SPV 债定价是否突破 S+600 / T+300。**这是最干净的高频信号。**
2. **撤销/缩量发行（pulled deals）**：Sopaipilla 7 月"遇冷"已是第一声（IFR 2026-07-31 [中]）；关注推迟发行、缩小规模、增加股权垫层的公告。一次公开的 pulled deal 比 100bp 利差走阔更有信息量。
3. **HY OAS**：当前 2.65%（9/11）——突破 ~3.0% = AI 高收益融资渠道开始收紧；CHK-009 阈值 4% = 破裂确认级。**加息落地后纹丝不动是当前最重要的反方向证据。**
4. **评级行动密度**：CoreWeave B1/B/BB-、DDTL 5.0 Ba2/BB+、Oracle BBB（Fitch 稳定）、Applied Digital 投机级——关注下调/负面观察的节奏，尤其是**从"评级随发行走"到"评级追着存量债下调"的拐点**。
5. **可转债闸门**：Nebius/CoreWeave 的低息子弹依赖股价高于转股价；股价持续下跌 → 转债窗口关闭 → 被迫转向 9.75% 级 straight debt → 利息负担阶跃。监测 CRWV/NBIS 股价相对转股价的距离。
6. **GPU 时租价格**：H100 时租月度轨迹（口径见 §3 注：marketplace $1.33–1.49 vs 全市场加权 $3.38–3.84 并存）= 抵押品价值的高频代理；B200/Rubin 爬坡期的旧卡价格弹性是 2027 摊还交叉点的先行读数。
7. **财政部拍卖 tail 与回购规模**：tail 连续出现 = crowding out 从价格传导升级为数量传导；Bessent 回购单次升至百亿级 = 官方承认失控（CHK-017）。
8. **Oracle 融资执行**：FY27 ~$40B 债+股计划的市场吸收情况（定价、订单倍数、是否被迫转向股权）——单一最大发行人行为本身就是信号。

### 5.3 数据缺口清单（如实登记）

1. CoreWeave Q2/Q3'26 后的全量债务到期阶梯（10-Q 逐年本金表未抓取）；DDTL 5.5 到期日与摊还表（新闻稿未披露）；各 DDTL 逐年摊还本金（结构性非公开）。
2. Nebius 2025-09 首轮转债的到期细节；Lambda $1B、Crusoe $750M 的期限/摊还/利率（私募，无公开条款）。
3. Beignet/Sopaipilla 摊还表（level-pay 还是后置）、Meta Pelican Leap 租约续约条款（4 年初始期之后的定价与选择权，仅 [低-中] 来源）。
4. 私募信贷软件到期墙的全行业金额（MS/Apollo/Fitch 均为比例或板块估算，无统一本金表）。
5. Oracle FY27 $40B 融资计划的债股比例与时间表（仅 FY26 计划公告与媒体口径）。
6. AI 债持有人结构（保险/养老金/杠杆基金占比）——"谁持有、以什么杠杆、按什么估值"无公开合并视图（AI Infrastructure Financing 报告同判）。
