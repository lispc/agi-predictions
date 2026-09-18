# 最终持有人图谱：AI 债的损失落在谁身上，通过几条通道

撰写日期：2026-09-18｜系列：debt-web 04/07

> 本篇是全系列主菜：回答 crash-dynamics/02 的核心问题——**谁是本轮的 Reserve Primary（看似安全、实则连雷、会挤兑的池子）？** 方法：逐条拆解四条损失传导通道（保险/年金、散户化、养老金/捐赠基金、银行间接敞口），每条回答五个问题：资金从谁来到谁去、经过几层包装、每层谁收费谁担险、损失传导需要几步、有没有赎回 gate 这类延迟引信。收尾给出损失传导链图与 Reserve Primary 候选排序，外加一节"监管反身性"。数字均带时点；可信度三级（[高]=官方/一手，[中]=主流财经媒体/具名机构，[低-中]=中小博客/聚合站），口径冲突并列呈现。
>
> 总判断先行：**AI 债的最终持有人不是对冲基金和投行自营盘，而是年金购买人、散户退休金账户、寿险一般账户和公共养老金**——全部是经过 2–4 层包装、每层都收了费、却把损失留在最后一层的"慢钱"。2008 年的 Reserve Primary 教训是：挤兑不需要资产大面积违约，只需要 1.2% 的持仓违约 + 持有人坚信过"不会亏"。截至 2026-09，这个组合已经在散户 BDC 通道小规模引爆过一次（Blue Owl OBDC II 永久关门），其余三条通道的引信仍在燃烧。

---

## 一、保险/年金通道：私募信贷进一般账户，负债端是年金购买人

### 1.1 资金流向与包装层数

资金链：**年金购买人（散户，买 MYGA/FIA）→ 寿险公司一般账户 → 私募信贷/资产支持融资（ABF）→ 借款人（含 AI 基建 SPV）**。包装层数与每层角色：

1. **负债端**：散户买年金。美国零售年金销售 2025 年创纪录 $461B，主力产品是多年期保证年金（MYGA）与固定指数年金（FIA）[中, [Insurance Business America / Morningstar DBRS, 2026-06-16](https://www.insurancebusinessmag.com/us/news/life-insurance/us-annuity-boom-fuels-private-credit-surge-that-worries-regulators-579107.aspx)]。
2. **资产管理端**：Apollo–Athene、KKR–Global Atlantic、Brookfield 模式的本质是**另类资管公司收购/自建寿险公司，用年金负债给自己的私募信贷产品当永久买家**。HBS 工作论文测算：Athene 与 Global Atlantic 各自为母公司的资产负债表增加了超过 $5,000 亿保险负债 [高（学术）, [HBS Working Paper 26-008, 2025](https://www.hbs.edu/ris/Publication%20Files/26-008_e387fd74-6f4d-483d-b039-ce7afa81805f.pdf)]。闭环结构：储蓄人把保费交给 Athene → Athene 买 Apollo 发起的信贷 → Apollo 收取发起费 + 管理费 + 持有利差，**同一美元在机器里转一圈被收费多次，风险留在保单持有人的一般账户里**。
3. **离岸再保险层**：Athene 约 83% 总准备金再保给百慕大关联实体，其中 $142B 进 ACRA 载体、63% 的经济利益归属未具名第三方 sidecar 投资人；集团百慕大偿付能力比率两年内 285% → 242% → 202% [低-中, [zk2u 对 BMA 披露文件的梳理, 2026-07-13](https://zk2u.com/blog/apo2/)]——方向单向，仍高于监管线。
4. **再包装层（2026 新增）**：Apollo 2026-05 推出 AMAPS（Apollo Multi-Asset Prime Securities），把贷款与基金份额打包成分级证券，约 9 倍杠杆、85% 资本结构获投资级评级——**把私募信贷再证券化卖给需要 IG 评级的保险组合，这是 CLO 框架从 $2T 杠杆贷款市场向 $40T 私募 IG 市场的复制** [低-中, [LinkedIn 整理, 2026-07-10](https://www.linkedin.com/posts/shikhar-chokhani-4260ba11a_apollos-new-yield-machine-apollo-just-issued-activity-7481247090484920320-bOuQ)]。

### 1.2 规模与 AI 敞口

- 窄口径：私募信贷约占寿险一般账户资产 **6%**（2025），2020 年为 3% [中, [Truth on the Market, 2026-07-13](https://truthonthemarket.com/2026/07/13/private-credit-public-panic-why-life-insurers-are-stronger-than-the-headlines-suggest/)]。宽口径（含私募配售、ABF）：Moody's 估计美国寿险约 $6T 投资资产中多达三分之一是私募信贷类资产（2024 末）[低-中, [Altss 引 Moody's, 2026-07-13](https://altss.com/rankings/largest-insurance-companies)]。口径差来自"private credit"定义，两数并列。
- 寿险持有的**非公开评级债券**存量超 $408B [低-中, zk2u 引 NAIC 数据，上引]；私募非流动性债券持仓 2025 年达 $807B [中, Morningstar DBRS 上引]。
- **Hyperion 的 A+ 债确实进了保险组合**：PIMCO 锚定 ~$18B 后，把 2049 年到期的"Beignet 债"分销给其客户——**明确包括保险公司、养老金、捐赠基金与理财顾问** [中, [Seattle Times/Bloomberg, 2025-12-15](https://www.seattletimes.com/business/how-techs-biggest-companies-are-offloading-the-risks-of-the-ai-boom/)]；另有报道称"剩余债券大部分分配给了保险公司管理的基金" [低-中, [moomoo/财联社, 2025-10-30](https://www.moomoo.com/news/post/60508112/new-capital-strategies-in-the-ai-era-meta-secures-27)]。链条成立：Meta 的表外债务 → SPV 债 → PIMCO 代客组合 → **年金购买人成为 Hyperion 的最终贷款人之一，而无人告诉他们**。

### 1.3 评级购物丑闻与 NAIC 收紧（监管层全记录）

- **事实基础**：NAIC 资本市场局 2024-06 报告显示，小评级公司（Egan-Jones、KBRA、Morningstar DBRS 等）占据了保险私募评级增量的 ~86%；对 2023 年 109 只有私募信函评级（PLR）的证券复核，**106 只（97%）的评级高于 NAIC 自家 SVO 的评估，平均高出 2.74 个 notch** [中, [Capstone, 2026-05-14](https://capstonedc.com/insights/insurers-increasing-exposure-to-private-credit-attracts-regulators-scrutiny/)；原始报告为 NAIC Capital Markets Bureau, 2024-06]。评级直接决定资本计提档位，2.74 个 notch 的系统性强奸等于**全行业的风险资本被系统性少计**。
- **丑闻点**：该报告发布后被 NAIC 从公开渠道撤下，近一年未重新发布 [低-中, [moomoo, 2026-04-08](https://www.moomoo.com/news/post/68007444/the-next-target-of-the-us-private-credit-crisis-insurance)；[Buxton Helmsley, 2026-07-21](https://www.buxtonhelmsley.com/news-and-insights/the-unpublished-grade-how-private-letter-ratings-came-to-certify-insurers-trillion-dollar-private-credit-expansionand-what-institutional-investors-must-demand-before-they-trust-the-next-investment-grade-label)]。
- **监管回应（时间表）**：SVO 获授权对高出自身评估 3 个 notch 以上的 Filing Exempt 证券发起挑战，**2026-01-01 生效——但操作系统与保密协议未就绪，实际执行推迟**；聘请 PwC 建立对八家评级机构的尽职调查框架（CRP Due Diligence Framework）；VOSTF 解散、改组为 Invested Assets Task Force（2025-12）；离岸再保险资产充足性测试 AG 55 首批报告 2026-04-01 到期；CLO 自建模型再延期一年至 2026 年底 [中, [Clifford Chance NAIC 秋季年会纪要, 2026-01-12](https://www.cliffordchance.com/insights/resources/blogs/insurance-insights/2026/01/naic-fall-2025-national-meeting-summary.html)]。**评价：工具箱在纸面上齐了，扳机还没装上。**

### 1.4 延迟引信与传导步数

- **延迟引信①（保单端）**：年金的 surrender charge 通常 7–10 年，退保罚 5–9%——这是保险通道的"天然 gate"，使它不会像货币基金那样 48 小时挤兑。**但 2022 年后的高利率使新单利率远高于存量，到期窗口集中时会形成慢漏**。
- **延迟引信②（FHLB 借款）**：Athene 2025 年从联邦住房贷款银行系统借款 $233 亿，为全系统第二大借款人（仅次于 Truist）[中, [Royal Gazette, 2026-03-27](https://www.royalgazette.com/reinsurance/business/article/20260327/athene-second-biggest-borrower-from-federal-home-loan-bank-system/)]。FHLB 预付款是寿险的应急流动性来源——**这也意味着保险通道的流动性危机最后会传导到政府隐性担保的 FHLB 系统**（2023 年 SVB 模式的镜像）。
- **传导步数**：AI 借款人违约 → 私募信贷资产减值 →（一步）保险一般账户盈余侵蚀 →（两步）RBC 比率下降 + 评级机构下调财务实力评级 →（三步）新单销售冻结 + 到期年金不再滚存 →（四步）被迫卖出流动性最好的资产。**全程以季度为单位，不以天为单位——这是与 2008 货币基金路径的本质区别，也是它更隐蔽的原因。**

---

## 二、散户化通道：evergreen BDC、interval fund、ETF 与 401(k)

### 2.1 资金流向与包装层数

资金链：**散户（经纪账户/理财顾问/401(k)）→ 非交易 BDC / interval fund / 私募信贷 ETF → 直接贷款组合 → 中小企业借款人（其中软件/AI 相关敞口 6,000–7,500 亿，见 raw-reports 调研 5）**。包装层数：

1. **载体层**：非交易 BDC（Blackstone BCRED ~$47B、Apollo ADS $15.1B、Ares ASIF $10.7B、Blue Owl OCIC/OTIC/OBDC II 等）承诺"季度赎回，上限 NAV 的 5%"。管理人收管理费 + 激励费；散户担全部信用风险与流动性风险。
2. **分销层**：理财顾问（RIA/经纪行）收取配售佣金——这是 2021–25 年销售的真正引擎，也是 First Brands 后赎回潮的行为学基础：**买的时候是"类债券稳健收益"，卖的时候才发现是排队制**。
3. **ETF 层（2025–26 新增）**：State Street + Apollo 的 PRIV（2025-02-27 上市，首只公募+私募信贷混合 ETF）[高, [State Street, 2025-02-27](https://investors.statestreet.com/investor-news-events/press-releases/news-details/2025/State-Street-Global-Advisors-Democratizes-Access-to-Investment-Grade-Private-Credit-Markets-with-New-ETF/default.aspx)]；后续 PRSD（2025-09）与 ABS ETF（2026-03），全系列 AUM 至 2026-02-28 约 $9.8 亿 [高, [State Street, 2026-03-11](https://investors.statestreet.com/investor-news-events/press-releases/news-details/2026/State-Street-Investment-Management-Launches-Investment-Grade-Public-and-Private-ABS-ETF/default.aspx)]；BondBloxx PCMM（2024-12，CLO 份额）。ETF 承诺**每日流动性**，底层仍是 7 年期非流动贷款——流动性错配比 BDC 更极端，只是规模尚小。
4. **401(k) 层（政策进行时）**：行政令 EO 14330（2025-08-07）要求 DOL/SEC 为 DC 计划配置另类资产开路 [高, [白宫 fact sheet 转引, 2025-08-07](https://www.wagnerlawgroup.com/wp-content/uploads/sites/1101401/2025/12/WhitePaperAlternativeInvestmentsin401kPlans.pdf)]；DOL 拟议规则 2026-01-13 提交 OMB，2026-03-30 正式发布 [中, [Morrison Foerster, 2026-04-03](https://www.mofo.com/resources/insights/260403-dol-proposed-rule-401-k-alternative-assets)]。DC 计划总盘子约 $12.5T——**闸门尚未全开，但管道正在铺设；散户资金入场时点恰在信用周期成熟期，这是历史泡沫的经典错配**。
5. 配套松绑：SEC 2025-08 更新 Accredited Investor 解释，取消了私募资产超 15% 的注册基金只能卖给合格投资者+$25,000 下限的限制 [低-中, [Katten 分析转引, 2026-09](https://angelinvestorsnetwork.com/alternative-investments/private-credit-market-2026)]。

### 2.2 First Brands 后的赎回潮：延迟引信已经烧过一轮

Q1 2026 是该通道的第一次实战压力测试，数据完整：

| 基金 | 赎回请求 | 结果 | 来源 |
|---|---|---|---|
| Blackstone BCRED | Q3'25 1.8% → Q4 4.5% → Q1'26 **7.9% NAV（$37–38 亿）** | Blackstone 注资 $4 亿公司资金全额兑付，**未启动 gate** | [低-中, [jinlow, 2026-03-17](https://jinlow.substack.com/p/private-credit-is-eating-itself-no)；[AIN, 2026-09-16](https://angelinvestorsnetwork.com/alternative-investments/private-credit-market-2026)] |
| Blue Owl OBDC II（$16 亿） | 连续两季超 5% 上限 | **2026-02-19 永久关闭赎回**，改为酌情资本返还；此前已卖 $14 亿资产；分析师预期有序清算约返还 30% NAV | [低-中, AIN 上引引 Stanger/FA-Mag] |
| Blue Owl OTIC | Q1'26 请求达**发行在外的 40.7%** | 只能兑付 5%；BofA 预计 Q2'26 峰值 OCIC 28.5%、OTIC **52.9%** | [中, [BofA via Yahoo Finance, 2026-04-29](https://finance.yahoo.com/markets/stocks/articles/private-credit-bdc-redemption-requests-204012982.html)；低-中, [f1gmat, 2026-04-21](https://premium.f1gmat.com/private-equity/trends/2026/Q1)] |
| Apollo ADS（$15.1B 旗舰） | Q1'26 请求 **11.2%**（$16 亿） | 按 5% 上限兑付 ~$7.3 亿（请求的 ~45%）；Q2'26 请求升至 ~17% | [低-中, [Crypto Briefing, 2026-06-23](https://cryptobriefing.com/apollo-private-credit-fund-redemption-requests/)；[With Intelligence, 2026-07-28](https://www.withintelligence.com/insights/apollo-and-ares-cap-redemptions-for-non-traded-bdcs/)] |
| Ares ASIF（$10.7B） | 请求 11.6% | 按 5% 上限 gate | [低-中, [A.L. Capital, 2026-07-16](https://alcapitaladvisory.com/research/intelligence/private-credit.html)] |
| Morgan Stanley 旗下基金 | Q2'26 赎回请求 ~17% | gate | [低-中, [ECM Source, 2026-06-24](https://ecmsource.com/apollo-morgan-stanley-private-credit-gates-q2-2026/)] |

要点三条：

- **Gate 按设计工作了，这正是问题**。Q1 2026 约三分之一的永续型私募信贷市场告诉投资人"季度流动性是愿望不是合同" [低-中, [Private Credit Pulse, 2026-05-06](https://privatecreditpulse.substack.com/p/semi-liquid-pick-one)]。5% 季度上限意味着想退出的人实际要排队一年以上——**赎回队列滚动累积，退出窗口随每次排队延长**，这与 2008 年 Reserve Primary 的"先跑者全额、后跑者吃折价"是同一纳什均衡，只是速度慢放。
- **管理人自掏腰包是缓冲也是信号**：Blackstone 的 $4 亿注资避免了 BCRED 触发 gate，但它证明**即使行业最强资产负债表也会在散户情绪转向时承压**。对照 First Brands 链：Jefferies Point Bonita 敞口 $7.15 亿（占组合 25%），2025Q4 计提 $30M、2026Q1 减记至零，2026-02 遭基金投资人起诉欺诈（投资人称被告知有"cash dominion"控制应收账款，实际没有）；UBS O'Connor 相关基金敞口约 $5 亿 [中, [Reuters, 2026-01-07](https://www.reuters.com/business/finance/jefferies-profit-rises-dealmaking-rebound-strong-underwriting-2026-01-07/)；[WSJ, 2025-10-08](https://www.wsj.com/finance/first-brands-bankruptcy-damage-spreads-to-jefferies-ubs-54ad84ef)；[ACI, 2026-02-26](https://alternativecreditinvestor.com/2026/02/26/jefferies-sued-by-investors-over-first-brands-collapse/)]。
- **秃鹫已到**：Saba Capital 与 Cox Capital 开始在二级市场折价收购非交易 BDC 份额/推动清算——2008 年后每一个 gated 池子的标准结局 [低-中, f1gmat 上引]。

### 2.3 传导步数

AI/软件贷款减值 → BDC NAV 下调（季度、管理人自报）→ 散户从媒体得知"蟑螂"→ 赎回请求超 5% → gate 启动 → **仍在场内的人 NAV 继续缩水但出不来** → 二级折价/诉讼/清盘。步数比保险通道少、速度快，且**每一步都上新闻**——这是四条通道里媒体放大器最强的一条。

---

## 三、养老金/捐赠基金通道：旧伤未愈的慢钱

### 3.1 资金流向与现状

资金链：**公职人员养老金缴费人/捐赠基金受益人 → 养老金/捐赠基金 LP 份额 → PE/PC 基金（承诺制，10–12 年锁定期）→ 底层贷款与股权**。配置水平：全球养老金 PE 配置约 10–14%，捐赠基金均值 15–20%，家办约 22% [低-中, [PipelineRoad, 2026-01-31](https://pipelineroad.com/blog/institutional-allocation-trends-2026)]。

这条通道的特殊性在于**它带着 2021 年份的旧伤进入 AI 周期**：

- **退出堰塞湖**：全球 PE 持有未退出公司超 32,000 家、未实现价值约 $3.2T（2019 年为 19,000 家）[低-中, [CJPI, 2026-03-27](https://www.cjpi.com/insights/the-rise-of-the-secondary-market-clearing-the-private-equity-exit-backlog/)]；分红率（distributions/NAV）仅 8–10%，历史常态为 20% [中, [Allianz Research, 2026-02-20](https://www.allianz.com/en/economic_research/insights/publications/specials_fmo/260220-private-equity.html)]。
- **分母效应未消化**：2022 年以来的 denominator effect 仍在限制 LP 新承诺能力；2026 年美股反弹（标普年内 +13.6% 至 8 月中）本应缓解，但 LP 行为已变成"先看 DPI 再谈配置" [低-中, [Praxis Rock, 2026-02-20](https://praxisrock.com/insights/what-lps-want-2026-dpi-transparency)；[Angel Investors Network, 2026-08-18](https://angelinvestorsnetwork.com/market-analysis/denominator-effect-family-offices-cutting-venture-capital-2026)]。
- **NAV 贷款蔓延**：GP 用基金底层组合做抵押借钱，用途从"保护组合"扩展到**给 LP 造分红**。市场规模约 $1,000 亿（2024），ILPA 预计 2030 年达 $6,000 亿 [高, [ILPA Guidance, 2024-07-24](https://ilpa.org/wp-content/uploads/2024/07/ILPA-Guidance-on-NAV-Facilities-2024.pdf)]；另一口径（17Capital/Oaktree）为 $44B（2023）→ $145B（2030E）[中, Allianz Research 上引]。两口径相差数倍，并列呈现；方向无争议。**NAV 贷款是养老金通道里的基金层面杠杆：它让 LP 报表上的 DPI 好看，代价是把 LP 的剩余索取权劣后给银行。**
- **还在加配私募信贷**：Preqin 2025-11 LP 调查中 81% 机构 LP 计划 2026 年持有或增加私募信贷承诺 [低-中, AIN 上引]。逻辑是"浮动利率 + 优先受偿"在通胀环境下的防御性——**但养老金买的很多正是银行不愿做的那部分风险**（见 §四）。

### 3.2 延迟引信与传导步数

- **没有赎回 gate，因为根本不需要**：承诺制下 LP 钱已锁死 10 年。这条通道的"引信"不是流动性而是**估值滞后**：私募组合按季度、按管理人模型估值，损失确认滞后公开市场 2–4 个季度。2008–09 年公募跌完后私募估值才逐季追跌，养老金 funded ratio 的恶化在 2009–10 年才显形，直接引发随后五年的缴费率上调潮（底特律式财政压力）。本轮的重演形态：AI/软件贷款减值 2026 年发生，养老金报表 2027–28 年确认，**州和地方政府的补缴义务 2028–30 年落地——这是"损失落在纳税人身上"的通道**（Burry 2026-07 转推的学术论文正是论证这一点 [低-中, [Memeburn, 2026-07-29](https://memeburn.com/michael-burry-ai-private-credit-warning/)]）。
- **传导步数**：底层违约 → 基金 NAV 减值（滞后 2–4 季）→ LP 报表亏损 + funded ratio 下降 → 缴费率上调/福利冻结/发 pension obligation bond 补洞。**四步，每步以年计；对金融市场无急性冲击，对财政是慢性病。**

---

## 四、银行间接敞口："直接敞口低"叙事的解剖

### 4.1 官方叙事与数字

大行与监管的一致口径是"银行对私募信贷直接敞口很小"。可核验版本：

- Fed 2026-05《金融稳定报告》：私募信贷风险"limited and manageable"；银行对私募信贷基金与 BDC 的**直接信用敞口约 $950 亿**；2025 压力测试严重情景下银行资本比率下限 11.8% [高, Fed FSR 2026-05，转引自 [AIN, 2026-09-16](https://angelinvestorsnetwork.com/alternative-investments/private-credit-market-2026)]。
- Fed 研究笔记：银行对私募信贷部门持有约 $79B 循环授信 + $16B 定期贷款（2024 数据）[高, [FEDS Notes, 2025](https://www.federalreserve.gov/econres/notes/feds-notes/bank-lending-to-private-credit-size-characteristics-and-financial-stability-implications-20250523.html)]。

### 4.2 间接敞口：银行没有退出风险，只是往资本结构上爬了一层

直接敞口口径排除了银行的**批发融资者**角色。逐层列示：

1. **基金层面杠杆**：subscription line（以 LP 承诺为抵押）+ NAV loan（以底层组合为抵押）。至 2025 年中，银行对私募信贷基金的承诺额度估计 ~$445B [低-中, [MarketMinute, 2026-04-10](https://www.financialcontent.com/article/marketminute-2026-4-10-the-shadow-credit-conundrum-why-banks-11-trillion-bet-on-private-lending-faces-a-high-tech-reckoning)]。
2. **BDC 层面**：Moody's 对美国银行监管申报的分析：银行对 NBFI 贷款的约 25%（~$3,000 亿）流向 BDC，Wells Fargo 敞口最大 [中, [The Banker, 2026-04-01](https://www.thebanker.com/content/6e9c62ce-282d-4234-bcf3-29aa86cf02d0)]。个体口径（Q1'26 10-Q）：Citi 对私募信贷机构贷款 $220 亿、Wells Fargo $362 亿 [低-中, [Caproasia, 2026-04-16](https://www.caproasia.com/2026/04/16/private-credit-exposure-of-citigroup-wells-fargo-bank-of-america-1-citigroup-reports-22-billion-loan-exposure-to-private-credit-firms-2-wells-fargo-reports-36-2-billion-loan-exposure-to-priva/)]。
3. **NBFI 总量**：银行对非银金融机构贷款 2026-06 达 **$1.997T**，占全部商业银行贷款 14.4%（2023 年初以来翻倍以上；存款基数同期只增 1.x%）[中, [Rithm Capital 对 call report 的整理, 2026-08-27](https://www.rithmcap.com/insights/q2-check-in-on-nbfi-lending/)]。IMF：样本中约半数资产规模的美国银行 NBFI 敞口超过其一级资本 [中, The Banker 上引]。
4. **数据中心/AI 专项**：warehouse line（给数据中心建设贷做仓储融资）、对 neocloud GPU 抵押结构的高级档参与——CoreWeave 2026-03-31 的 $8.5B 投资级循环额度（Moody's A3，SOFR+225bp）由银团提供，此前这类风险只有私募信贷以 10–15% 溢价承接 [低-中, [Peony, 2026-08-19](https://www.peony.ink/blog/neocloud-capital-raise)]。**利差压缩轨迹本身就是银行顺着资本结构往下爬的证据。**

### 4.3 与 2007 SIV 流动性承诺的类比

2007 年银行表外 SIV/ABCP conduit 的"直接敞口"也很小——直到流动性承诺（liquidity backstop）被触发，风险一夜回表（Citi 2007-12 把 $49B SIV 资产并表是标志性事件）。类比映射：

- **subscription line / warehouse line = 本轮的流动性承诺**。它们在压力情景下的行为从未被测试：当 BDC gate、基金 LP 断供、数据中心租约违约同时发生时，银行面临的选择与 2007 年相同——**抽额度（逼死客户、坐实损失、引发传染）或展期（风险回表、资本占用上升）**。Acharya 等关于"contingent credit"的研究表明，信用额度在系统性压力中的集中支取本身就是传染渠道 [高（学术）, [Acharya et al., NYU](https://pages.stern.nyu.edu/~sternfin/vacharya/public_html/pdfs/working-papers/ARFE_ContingentCredit_AJS.pdf)]。
- **"直接敞口低"在 2007 年也是真的——直到它不是**。银行体系的真实风险不是持有的贷款，而是对整条影子信贷链的**或有融资义务**；这些义务不进 $950 亿口径。Fed 自己也承认软性一面：2026-05 FSR 在"manageable"之外补了一句"赎回与负面情绪可能导致部分借款人（尤其是信用风险较高者）可获得的信贷收缩" [高, Fed FSR 上引]——这句话翻译过来就是：**银行额度收缩是私募信贷危机的第一放大器**。
- **传导步数**：底层违约 → BDC/基金净值跌 → 银行上调抵押折扣率或缩减额度（crash-dynamics/02 §3.1 的 haircut spiral）→ 基金被迫卖贷 → 折价坐实全行业 NAV 下调 → 回到 §二、§三的赎回与估值引信。**银行通道不是损失的最终落点，却是把落点的速度放大四倍的涡轮。**

---

## 五、图①：损失传导链总图

```
AI 借款人违约（软件贷款 $600–750B 敞口 / 数据中心 SPV / neocloud GPU 抵押）
        │
        ▼
┌─────────────────────────────────────────────────────┐
│ 第一层：私募信贷基金 / BDC / CLO（NAV 减值，季度滞后）  │
│ 缓冲：优先受偿结构、管理人自注资（BCRED $4 亿先例）      │
│ 放大器：PIK 利息掩盖违约、管理人自报估值、2021 年份集中  │
└─────────────────────────────────────────────────────┘
        │ 分四路
        ▼
① 保险一般账户（Athene/GA 模式；Beignet 债经 PIMCO 分销）
   缓冲：surrender charge 7–10 年、FHLB 借款额度
   放大器：评级购物→资本少计（+2.74 notch）；离岸再保险透明度
   最终持有人：年金购买人 + FHLB（=政府隐性担保）
② 散户 evergreen BDC / interval fund / ETF
   缓冲：5% 季度 gate（对基金是缓冲，对散户是牢笼）
   放大器：媒体循环、赎回队列滚动累积、ETF 每日流动性幻觉
   最终持有人：散户 + 401(k) 参与者（管道铺设中）
③ 养老金/捐赠基金 LP
   缓冲：承诺制锁定、估值滞后（=延迟确认，不是不确认）
   放大器：NAV 贷款劣后化 LP 权益、continuation fund 自我交易
   最终持有人：公职人员养老金缴费人 + 纳税人（补缴义务）
④ 银行或有融资（subscription/NAV/warehouse line ~$445B+；NBFI 总 $2.0T）
   缓冲：优先抵押、压力测试 11.8% 下限
   放大器：折扣率螺旋、额度集中支取（SIV 式风险回表）
   最终持有人：银行股东 →（极端情景）存款保险/纳税人
        │
        ▼
汇合点：四通道在银行额度收缩处交叉——④一旦启动，①②③的资产端
被迫同时按市价重估，"私募信贷没有按市值计价"的防火墙消失。
```

---

## 六、图②：Reserve Primary 候选名单（排序与理由）

评选标准沿用 crash-dynamics/02：持有人把它当"类现金/类债券安全资产"、底层实际连着同一批雷、存在可行的挤兑或挤兑等价物。

| 排名 | 候选池子 | 为什么是它 | 距引爆的观测距离 |
|---|---|---|---|
| **1** | **散户非交易 BDC / interval fund 综合体**（~$2,500–4,000 亿永续型私募信贷） | 三条全中：(i) 销售话术=稳定收益类固收；(ii) 底层=软件/中型企业贷款，与 AI 颠覆敞口同源；(iii) 挤兑机制=赎回队列（慢速挤兑）。**前震已发生**：OBDC II 永久关门（2026-02）、ADS/ASIF/MS 基金集体 gate、OTIC 请求 40.7% | **已经发生小规模版本**；下一只 watch 对象：BCRED 若 Q3/Q4'26 再度请求 >5% 而 Blackstone 不再注资，或任何一只旗舰基金 NAV 单季下调 >3% |
| **2** | **私募信贷 ETF（PRIV 系）与每日流动性包装** | "每日赎回 + 7 年期非流动贷款"是全图谱最极端的错配；规模尚小（~$10 亿）但增速快、媒体可见度最高。折价螺旋一旦启动（ETF 市价 vs 管理人自报 NAV 脱锚），将成为**每日直播的"跌破面值"**——2008 年 Reserve Primary 的 $0.97 用了一天，ETF 版本会用一小时 | 观察点：PRIV 系 ETF 相对 NAV 折价 >1.5% 且持续；做市商报价价差突然走阔 |
| **3** | **年金-保险一般账户（Athene/GA 模式）** | 最像 Reserve Primary 的心理结构（"我的年金是保本的"），体量最大（$461B/年新增）。但不会 48 小时挤兑：surrender charge + 按季确认的偿付能力机制决定了它是**慢放版**。它的"跌破面值"等价物 = 财务实力评级下调潮 + NAIC 3-notch 挑战落地触发全组合资本重计 | 观察点：AM Best/S&P 对 PE 系寿险的评级行动；AG 55 首批报告（2026-04 起）暴露的离岸再保险资产质量问题；FHLB 预付款异常增长 |
| **4** | **持有数据中心/AI 应收的短期限载体**（数据中心 ABS、算力应收打包产品、任何把 OpenAI 链合同证券化的池子） | 2008 最贴脸的类比（CP/ABCP 冻结），但当前此类资产主要卖给机构而非货币基金，"类现金"持有人基础尚窄。若 2026–27 年有人把它装进货币基金/稳定币储备/短债 ETF，排名立即升至第一 | 观察点：数据中心 ABS 利差走阔 >100bp；首个 SPV 债（Beignet 类）评级行动 |
| **5** | **银行对私募信贷的或有融资网络** | 不是"池子"而是涡轮（§四）。单独列名是因为它的启动会把前四名同时引爆 | 观察点：大行季报 NDFI/PC 敞口环比收缩；warehouse line 折扣率上调的传闻 |

**排序结论**：Reserve Primary 最可能出现在**散户化通道**——不是因为它规模最大（保险通道更大），而是因为它唯一同时满足"持有人相信不会亏 + 有赎回窗口 + 已被 First Brands/Tricolor 预演过信心崩塌"三个条件，且 Q1 2026 的 gate 潮证明触发成本已经很低。保险通道是**损失的最大最终落点**，散户通道是**危机的第一个广播站**——2008 年 Reserve Primary（620 亿）之于货币基金（2.7 万亿）正是这个比例关系。

---

## 七、监管反身性：通道被挤压时监管会怎么反应

监管不是旁观者，是传导链上的应力集中点。三条线的预判与历史类比：

### 7.1 SEC ↔ BDC/散户通道

- **已做**：2025-08 放松合格投资者限制（方向是扩大准入，周期顶部的顺周期松绑）；gate 本身合法——非交易 BDC 的 5% 上限写在招募书里，SEC 无需也无法阻止基金"按合同关门"。
- **将做（按历史剧本）**：2008 年 Reserve Primary 后 SEC 的反应序列是 2010 改革（流动性底线）→ 2014 改革（机构 prime 基金浮动 NAV + gate 合法化）→ 2023 改革（流动性费）——**每一轮都把"挤兑的合法性"写得更清楚，同时把风险推向不受同一规则约束的载体**（资金从 prime 基金流向政府基金与后来的稳定币）。本轮的映射：对 BDC 分销佣金与"类固收"营销话术的销售行为执法（FINRA 层面已有诉讼潮），可能加赎回披露与压力测试披露；**净效果大概率是把散户从非交易 BDC 推向 ETF 包装——即把排名 1 的风险推向排名 2 的载体**。
- 反身性要点：监管执法本身成为新闻流，加速赎回请求（Q1 2026 的赎回潮与 First Brands 报道节奏高度同步）。

### 7.2 NAIC ↔ 保险通道

- **已做**：3-notch 挑战授权（2026-01 生效、执行推迟）、CRP 尽调框架（PwC）、AG 55 离岸再保险测试（首批 2026-04）、CLO 自建模型（延至 2026 底）。
- **结构性弱点**：NAIC 是州监管者的自愿联盟，无强制执法权，议程以年为单位推进（VOSTF 1907 年存在到 2025-12 才改组）。**它的时钟与危机时钟差一个数量级**。
- **将做（按历史剧本）**：2008 年 monoline/CDO 评级失效后，NAIC 的回应是自建 SVO 评估能力并引入模型估值——耗时 3–5 年。本轮已提前走完一半（报告、授权都有了），缺的是执行；**风险情景是顺周期补刀**：若 NAIC 在减值已经发生后落地 3-notch 挑战，保险公司被迫一次性上调资本计提，触发全组合卖出（IMR/AVR 机制会把 realized loss 摊销压力变成卖出压力），把"慢漏"变成"台阶式重估"。历史类比：2008–09 年寿险业在 CDO/次贷 MBS 减值后的评级下调潮（MetLife、Hartford 股价 -80%+，Hartford 最终接受 TARP）。
- 离岸监管套利是泄压阀：美国收紧 → 更多再保险去百慕大/开曼 → AG 55 的测试范围成为下一个监管战场。

### 7.3 Fed ↔ 银行通道

- **已做**：2026-05 FSR 口径"limited and manageable"（功能上与 2007-03 "contained" 同构——crash-dynamics/02 §4.4 的第一行）；FDIC 已要求 $100 亿以上银行把 NDFI 贷款拆成五类申报（数据基础设施先于政策）；2025 压力测试覆盖 NBFI 情景。
- **工具箱（历史剧本）**：Fed 不能直接救非银基金（无贴现窗口准入），13(3) 条款的先例是 2008 AMLF（为 ABCP 提供融资）与 2020-03 MMLF（货币基金流动性工具）——**若散户 BDC/ETF 通道引爆并冻结短期信贷，剧本大概率复用：先给"类现金"载体开流动性工具（对标 9-19 货币基金担保），再通过银行体系间接稳定私募信贷链**。约束条件与 crash-dynamics/02 §六.4 一致：2026 年通胀与鹰派 Fed 意味着三级跳会更慢更晚。
- **类比 2022 英国 LDI**：养老金通道的杠杆（NAV 贷款之于 LP 组合 ≈ LDI 之于英国 DB 养老金）在利率/利差冲击下触发保证金追缴，最后由央行买资产止血。BoE 2022-09 用了 13 天被迫入市；Fed 对私募信贷链没有等价授权，**干预门槛更高、时点更晚**。

### 7.4 反身性总括

三条线的共同结构：**监管反应本身改变损失在各通道间的分配**。SEC 执法把风险从 BDC 推向 ETF；NAIC 收紧把资产推向离岸与更不透明的评级安排；Fed 对银行额度的窗口指导把风险从受监管口径推向未申报口径。2008 年后的全部监管史表明这是常态而非失误——**对本仓库 watch 的操作含义：盯监管公告的"通道挤压效应"（哪条通道在被挤压、风险被推向哪条），比盯任何单一监管行动本身更早半拍。**

---

## 附注：口径说明

- **保险私募信贷占比**：6%（窄口径，truthonthemarket 引 NAIC/行业数据）与"三分之一"（宽口径，Altss 引 Moody's，含私募配售与 ABF）不可通约，正文并列。
- **NAV 贷款市场规模**：ILPA/FFA 口径 $100B（2024）→$600B（2030E）；17Capital/Oaktree 口径 $44B（2023）→$145B（2030E）。差异源于统计范围（仅 PE vs 含 PC/不动产），方向一致。
- **Blue Owl OBDC II 关门日期**：AIN 记 2026-02-19，A.L. Capital 记 2026-02-18"确认永久 gate"，疑为董事会决议日与公告日之别，正文采用 02-19。
- **BCRED Q1'26 赎回额**：$3.7B（jinlow）与 $3.8B（AIN）并存，均为 7.9% NAV。
- **银行对 PC 承诺额度 ~$445B**：单一来源（MarketMinute，低-中可信度），未见 Fed/IMF 原文确认，正文已标注。
- **Athene 百慕大偿付能力比率（285→242→202%）与 ACRA $142B/63% sidecar**：低可信度单一来源（zk2u 对 BMA 申报文件的整理），方向与 Royal Gazette 报道的 FHLB 借款激增互证，但具体数字待 BMA 原文核验。
- 本篇为结构分析，**不登记概率**；如需将"Reserve Primary 候选排序"转为可清算命题，走 ledger EXT/OUR 流程另行提名。

## 主要来源（节选）

- [高] Fed FSR 2026-05；FEDS Notes（银行对私募信贷敞口；寿险中介作用）；ILPA NAV Facilities Guidance（2024-07）；FSB《Report on Vulnerabilities in Private Credit》（2026-05-06："at its current size and scope has not been tested during a severe economic downturn"）；NAIC 会议纪要（Clifford Chance 整理）；State Street/Apollo ETF 公告；白宫 EO 14330 与 DOL 拟议规则（2026-03-30）；HBS WP 26-008
- [中] Bloomberg/Seattle Times（Beignet 债分销）；Reuters（Jefferies/First Brands）；WSJ（UBS O'Connor 敞口）；Morningstar DBRS（年金销售 $461B/私募非流动债 $807B）；BofA 研究（BDC 赎回峰值预测）；The Banker（Moody's/IMF 银行 NBFI 分析）；Royal Gazette（Athene FHLB $23.3B）；Allianz Research（分红率 8–10%）；Capstone（NAIC 106/109 评级复核）
- [低-中] AIN、Private Credit Pulse、jinlow、A.L. Capital、Caproasia、f1gmat、zk2u、MarketMinute、ECM Source（2026 年 BDC gate 潮细节、AMAPS 结构、百慕大数字；关键数字均已尽量与 [中]/[高] 来源交叉）
