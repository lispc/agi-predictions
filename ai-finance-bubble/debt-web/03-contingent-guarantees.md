# 担保、兜底与或有负债的法律强度：第一块多米诺倒下时，哪些"承诺"会变成真负债

撰写日期：2026-09-18｜系列：debt-web 03/07

> 本篇是 debt-web 系列的"AIG 映射"篇（机制原型见 `../crash-dynamics/02-subprime-2007-08-anatomy.md` §3.2）：逐个解剖循环交易网络中的兜底承诺——法律性质、现金触发条件、破产追索顺序、会计落点。核心区分：**或有负债的致命之处不在名义值，在触发条件与现金时点**。来源沿用三级可信度（[高]=官方/一手文件，[中]=主流财经媒体/具名机构研究，[低-中]=中小博客/聚合站）。法律机制部分（破产法 §365 等）为一般法教义学陈述，标注法律来源。

---

## 一、NVDA–CoreWeave $6.3B 容量兜底：是购买义务，不是担保——但这更硬

### 法律性质

2025-09-09 CoreWeave 8-K 披露：双方在 2023-04-10 主服务协议（MSA）下签署新订单（order form），初始价值 $6.3B，条款为 **NVIDIA "有义务购买至 2032-04-13 为止的未售出残余容量"**（obligated to purchase the residual unsold capacity）。8-K 同文载明三重关系："NVIDIA 向本公司供应 GPU，且是本公司股东" [高, [CoreWeave 8-K, 2025-09-15](https://www.stocktitan.net/sec-filings/CRWV/8-k-core-weave-inc-reports-material-event-634b5d5375de.html)；[CNBC, 2025-09-15](https://www.cnbc.com/2025/09/15/coreweave-stock-jumps-on-disclosure-of-6point3-billion-order-from-nvidia.html)]。

关键定性：**这是一份买方承诺（purchase obligation），不是对外担保（guarantee of third-party debt）**。区别在追索路径：担保是 CoreWeave 违约后债权人向 NVDA 索偿；购买义务是 NVDA 自己成为 CoreWeave 的边际客户——只要容量卖不出去，NVDA 就必须按月付钱买一堆自己用不上的算力。法律硬度上购买义务**更强**：它不依赖于 CoreWeave 违约这一触发事件，正常经营状态下即可被调用；$6.3B 是初始值（floor），订单可扩容 [中, [Peony, 2026-08-19](https://www.peony.ink/blog/gpu-cluster-financing-data-room)]。

### 什么条件下变成现金支出

触发条件 = CoreWeave 数据中心容量未被其客户满租。即触发概率与 AI 算力需求逆转完全负相关——**这是教科书式的 wrong-way risk：兜底在 NVDA 自身芯片需求最差的情形下被调用**。NVDA 在 Q2-FY27 10-Q（2026-08-26 提交）中首次把该承诺与另外两笔合并披露为合计 $114.8B 的"基础设施支持"敞口：$6.3B CoreWeave 容量购买义务 + $105B 俄亥俄 PORTS-Pike 园区（SB Energy 持有物业、OpenAI 20 年租约入驻）的**分阶段递减残值担保** + $3.5B 土地/电力相关承诺 [中, [LinkedIn/Nauman Noor, 2026-09-03](https://www.linkedin.com/pulse/two-referees-one-asset-sec-classified-building-skipped-nauman-noor-mewvc)；口径与 Baptista 2026-08-18 报道一致，见 research-01 §3]。同季 10-Q 还计提了 $6.3B 的"存货及超额存货采购义务拨备"（H1-FY27 累计）[高, [NVDA 10-Q, 2026-07-26 季度](https://www.sec.gov/Archives/edgar/data/1045810/000104581026000075/nvda-20260726.htm)]。

### CoreWeave 破产时 NVDA 的地位

- **作为兜底人**：该购买义务是双务待履行合同（executory contract）。若 CoreWeave 进入 Chapter 11 并依破产法 §365 **拒绝履行**该合同，NVDA 的付款义务随之消灭，NVDA 仅持有一项无担保损害赔偿债权 [高, 破产法 §365；机制综述见 [Troutman Pepper, 2023](https://www.troutman.com/insights/what-is-an-executory-contract-and-what-will-happen-to-my-executory-contract-in-bankruptcy/)]。即：**这个兜底防的是"产能过剩"，防不了"主体死亡"**——CoreWeave 破产时它自动失效，DDTL 贷款人（Blackstone/Magnetar 牵头，GPU+客户合同作抵押）无法向 NVDA 追索。
- **作为股东**：2026-01-26 NVDA 再投 $2B（$87.20/股 A 类股），持股升至约 11.5% [中, [stefanus.ai, 2026-08-08](https://stefanus.ai/cloud-recapture-how-strategic-ai-investments-return-to-their-investors-as-chip-sales-cloud-commitments-datacenter-revenue-and-collateral-value-of-the/)；[Tickeron, 2026-05-13](https://tickeron.com/trading-investing-101/the-nvidia-ai-empire-forecast-2030-how-jensen-huang-is-using-15-billion-to-prefinance-the-entire-ai-infrastructure-stack/)]。股权在破产清偿顺序最末。
- **三重身份冲突**：股东身份激励 NVDA 让 CoreWeave 活着（避免 $2B+ 存量股权归零）；兜底人身份使"让 CoreWeave 活着"的直接成本就是 NVDA 自己付款；而兜底的存在本身又抬高了 DDTL 抵押品（GPU 租约现金流）的评估价值，间接补贴了 Blackstone 等贷款人的放款意愿。冲突的净效果：**NVDA 有动机在 CoreWeave 丧失清偿能力前持续注入需求，把流动性问题掩盖为"产能利用率"问题**——这正是 2007 年 SIV 发起行的行为模式（§七）。

### 会计落点

执行中的购买义务按 ASC 606/采购承诺惯例**只进脚注，不上表**；NVDA 资产负债表上无对应负债，直到容量真的卖不出去、付款义务现实化为止。NVDA 对 CoreWeave 的总敞口 = $6.3B 购买义务（脚注）+ 约 11.5% 股权（投资科目）+ GPU 销售应收/供应链敞口。

---

## 二、云合同 RPO 的可执行性：$300B  backlog 在破产法院值多少钱

### RPO 是什么

RPO（剩余履约义务，ASC 606 口径）是"已签约未确认收入"的**会计披露指标**，不是资产，更不是客户对云厂商的债务登记。Oracle RPO 从 FY26Q1 的 $455B（同比 +359%）升至 Q4-FY26 的 $638B，其中约 $300B 归属 OpenAI 的 5 年合同（2027 年起，~$60B/年）[中, [DCD, 2025-09-11](https://www.datacenterdynamics.com/en/news/openai-signs-300bn-cloud-deal-with-oracle-report/)；[IntuitionLabs, 2025-11-30](https://intuitionlabs.ai/articles/oracle-openai-300b-deal-analysis/)；研究底稿 research-01 §3]。**合同条款（取消费、终止权、MAC 条款）从未公开披露** [低-中, [implicator.ai, 2026-02-18](https://www.implicator.ai/oracles-300-billion-openai-bet-puts-overflow-cloud-at-center-stage/)]。

### OpenAI 重组/破产时这些承诺是什么

云服务长约是典型的双务待履行合同。在美国破产法下：

1. **债务人可依 §365 拒绝履行**，拒绝视为申请前违约，损害赔偿转化为**一般无担保债权** [高, 11 U.S.C. §365；[Troutman Pepper, 2023](https://www.troutman.com/insights/what-is-an-executory-contract-and-what-will-happen-to-my-executory-contract-in-bankruptcy/)]。即 Oracle 账上 $300B RPO 在 OpenAI Chapter 11 情景下 = 一项$300B 量级的无担保破产债权，按无担保清偿率回收（参考值：大型 Chapter 11 无担保回收率常以个位数到几十美分计）。
2. **ipso facto 条款不可执行**：合同中"对方申请破产即自动终止"的条款依 §365(e)(1) 无效 [高, [Williams Mullen, 2021](https://www.williamsmullen.com/insights/news/legal-news/are-bankruptcy-provisions-your-executory-contract-enforceable)]——云厂商不能因 OpenAI 申请破产而单方撕约，只能等债务人选择。
3. **破产前的压力路径**是重新谈判而非违约：OpenAI 可用服务等级违约、交付延迟、技术过时、不可抗力等抗辩压价或缩减承诺。Quinn Emanuel 把这类 take-or-pay 争端列为该行业"最早且经济影响最大"的诉讼类别，并列举了承租方的标准抗辩清单（SLA 不达标、ready-for-service 未达成、force majeure、商业 impracticability）[中, [Quinn Emanuel, 2026-03-13](https://www.quinnemanuel.com/the-firm/publications/client-alert-emerging-litigation-risks-in-financing-ai-data-centers-boom/)]。事实上该压力已部分显现：WSJ 报道 OpenAI 2026 收入不及预期后，其对外承诺口径从 ~$1.4T 收缩至 ~$600–750B [低-中, [tech-insider 转引 WSJ, 2026-08-18](https://tech-insider.org/openai-revenue-miss-friar-altman-stargate-2026/)；[The Arbiter, 2026-07-28](https://www.arbiter.blog/articles/nvidia-is-now-cosigning-the-ai-boom-it-supplies/debate)]。

### OpenAI–Microsoft $250B Azure 承诺

同构处理。2025-10-28 重组协议中 OpenAI 承诺增购 $250B Azure 服务（至 2032）；作为对价 Microsoft 获 PBC ~27% 股权（估值 ~$135B），同时**放弃了对 OpenAI 算力采购的优先拒绝权**；API 产品维持 Azure 独家至 2032 [中, [GeekWire, 2025-10-28](https://www.geekwire.com/2025/microsoft-secures-27-stake-in-openai-in-new-deal-with-commitment-for-250b-in-azure-usage/)；[SEC API 对 MSFT 8-K 附件的整理, 2026-09-02](https://sec-api.io/insights/financial-analysis-of-microsoft-fy2026-capital-intensity-against-a-record-margin)]。2026-04 双方进一步修订协议，取消收入分成安排 [中, [Directions on Microsoft, 2026-04-27](https://www.directionsonmicrosoft.com/microsoft-openai-amend-their-agreement-again/)]。Microsoft 云 RPO ~$625–627B、约 45% 来自 OpenAI [中, research-01 §3]。破产情景下这笔 $250B 同样是可拒绝的待履行合同——**且 Microsoft 作为 ~27% 股东身处"债权人 vs 股东"的结构性冲突中**（与 §一 NVDA 同型）：股东身份激励它在重组中让步以保住股权价值，让步的代价由 Azure  backlog 质量承担。

### 会计落点

RPO 对云厂商是收入脚注（不进资产）；对客户（OpenAI）按 ASC 440 采购承诺披露或根本不量化——**OpenAI 是私人公司，连脚注都不必给**。双边都不上表，$300B/$250B 名义值存在于新闻稿与 RPO 脚注里，法律效力却要等到违约或破产才被检验。

---

## 三、SPV 结构中的母公司隐性支持：写下来的上限 vs 市场默认的无限

### Meta Hyperion（Beignet Investor）

结构：SPV 由 Blue Owl 基金持 80%、Meta 持 20%；融资 ~$27B A+ 级债务（PIMCO 锚定 ~$18B）+ ~$2.5–3B 股权；SPV 拥有物业并租给 Meta，租约约 16 年；Meta 提供**残值担保（residual value guarantee）**——若 Meta 不续租或租约终止时数据中心价值低于阈值，Meta 以现金补足，**上限约 $28B** [高, [Meta IR, 2025-10-21](https://investor.atmeta.com/investor-news/press-release-details/2025/Meta-Announces-Joint-Venture-with-Funds-Managed-by-Blue-Owl-Capital-to-Develop-Hyperion-Data-Center/default.aspx)（"capped cash payment"，16 年运营期）；[Kirkland & Ellis, 2025-10-21](https://www.kirkland.com/news/press-release/2025/10/kirkland-represents-blue-owl-on-joint-venture-with-meta-to-develop-hyperion-data-center)]。会计上：Meta 不并表 SPV，$27B 债务不上表；RVG 仅在年报脚注描述，**未记录任何负债**——Moody's 2026 年公开警告美国会计准则允许这类"短初始租期+残值担保"结构使表内负债系统性低估真实义务，并宣布将据此调整 Meta/Oracle 等评级方法 [中, [Quinn Emanuel, 2026-03-13](https://www.quinnemanuel.com/the-firm/publications/client-alert-emerging-litigation-risks-in-financing-ai-data-centers-boom/) §IV.B、§VI.C、§VI.D]。

**法律强度分级**：RVG 是真实书面义务，但有三个软化点：(1) 触发条件是 Meta 自己选择不续租——触发与否在 Meta 手里（不过 IFR 指出不续租就要开出巨额残值支票，构成续约的经济强制 [中, [IFR, 2025-12-17](https://www.ifre.com/ifr-awards/2340435/the-metablue-owl-deal-broken-down-off-balance-sheet-gymnastics-24-years-after-enron)]）；(2) 赔付额取决于"数据中心残值"的评估——专用 AI 机房无可靠可比物，评估方法、评估人选择权、善意履约都将成为诉讼焦点（Quinn Emanuel §VI.D）；(3) 有上限（~$28B vs 项目总成本 >$50B，2026-07 扩产后）。

**隐性支持层**：市场对"Meta 不会让 Hyperion 违约"的默认超出 RVG 上限——例如建设期完工风险、运营成本超支。这部分**没有任何书面承诺**。评级机构对 Hyperion 在建项目给出投资级评级，依据的正是 Meta 租约与担保，项目评级事实上被锚定在 Meta 自身信用上（Quinn Emanuel §VI.C）。若 Meta 遭遇自身信用事件，隐性支持假设与显性担保价值同时衰减。

### xAI 的 SPV 租卡结构

$20B 包：~$7.5B 股权（Valor Equity Partners 锚定，NVDA 最高 $2B）+ ~$12.5B 债务（Apollo/Diameter 牵头）；SPV 直接购买 NVDA GPU 并以 5 年租约租给 xAI（Colossus 2），债务以 GPU 本身为抵押，不上 xAI 资产负债表 [中, [Bloomberg 转引, PitchBook, 2026-06-22](https://pitchbook.com/news/articles/nvidia-reportedly-adding-xai-to-growing-ai-venture-portfolio-20b-round)；[DCD, 2026-09-16](https://www.datacenterdynamics.com/en/news/nvidia-to-invest-in-xai-special-purpose-vehicle-cash-to-be-used-to-buy-nvidia-gpus/)；[Transurfing Volatility, 2026-09-07](https://transurfing-volatility.com/neoclouds/)（低-中）]。与 Meta 结构的关键区别：**没有任何公开披露的母公司担保或残值担保**——xAI 的敞口理论上只有租约义务本身（同样是待履行合同，破产时可拒绝）。贷款人的终极依靠是 GPU 残值，而 H100 租金自 2023 年以来已跌 70–90% [中, Quinn Emanuel §VI.E]。这是本轮最纯粹的"隐性支持"案例：$12.5B 债务的定价里包含了市场对 Musk 体系输血能力的主观评估，法律上一文不值。

### 支持承诺的法律强度分级（项目融资通行结构）

由硬到软：
1. **付款担保（payment guarantee）**：无条件、见索即付；本轮未见纯形态。
2. **完工担保（completion guarantee）**：担保项目建成，建成后义务灭失；触发窗口在施工期。
3. **股权承诺函（equity commitment letter）**：承诺向 SPV 注资；可由 SPV（及约定时的贷款人）强制执行，但通常附条件（先决条件、金额上限）。
4. **残值担保（RVG）**：Meta 形态——条件触发（不续租）+ 上限 + 评估争议。
5. **安慰函/隐性支持**：无法律效力，仅靠声誉强制。
Google–Fluidstack–TeraWulf 的 $3.2B 兜底是"条件比上限更软"的样本：Google 承诺在 Fluidstack 违约时支付终止费或承接租约，换取 TeraWulf 最高 14% 认股权证，同类承诺累计 >$5B；但**兜底仅在完工且租约开始后才生效，若工期延误超 180 天 Fluidstack 可整体终止租约，Google 兜底永不触发**——发行备忘录自己承认"Google 可能不兑现支持"[中, Quinn Emanuel §IV.C、§VI.D；[低-中] 转引 Fitch 评级意见称工期"激进"]。**建设期——风险最高的阶段——恰恰是无支持裸奔的阶段。**

---

## 四、take-or-pay 与电力侧或有负债：兜底人是电费纳税人

数据中心 PPA 与公用事业产能承诺的或有负债方向相反：**这里的"隐性担保人"是公众**。公用事业按 AI 负荷预测提前建设发电与输电资产；若数据中心取消或负荷落空，成本传统上通过费率基础（rate base）摊给全体用户。

监管者 2025–26 年的应对是把隐性社会化改造成显性 take-or-pay：

- **俄亥俄**：PUCO 2025-07-09 批准 AEP Ohio 数据中心电价（DCT），07-23 生效：新增负荷 ≥25MW 须签 12 年合同（含 4 年爬坡），**最低需量费 ≥合同容量的 85%**，须提供抵押品、财务可行性证明，退出须付退出费 [高, [PUCO](https://puco.ohio.gov/wps/portal/gov/puco/utilities/electricity/resources/data-centers)；[AEP 新闻稿转引, 2025-07-09](https://whopaysfordatacenters.com/states/ohio/)]。2026-08-05 PUCO 再加码：数据中心并网须提前 180 天通知 [中, [Baseload News, 2026-08-12](https://baseload.news/blog/puco-aep-ohio-180-day-data-center-notice)]。2026-06 俄亥俄 HB 646 提案拟把该模板推广至全州公用事业 [低-中, [Cliff, 2026-06-10](https://www.cliffcenter.com/dockets/2026-06-10)]。
- **佐治亚**：PSC 2025-01-28/04 批准规则，>100MW 新负荷须单独谈判合同：**15 年期、最低账单、财务担保、PSC 事前审批**；2025-12 补充协议承诺若数据中心繁荣落空，现有用户电价冻结保护至 2031 [中, [Georgia Recorder, 2025-12-18](https://georgiarecorder.com/2025/12/18/georgia-powers-plan-for-powering-data-centers-is-up-for-a-final-vote-friday/)；[Compute Law Blog, 2026-05-23](https://computelaw.blog/power/georgia-power-psc-data-center-rules/)；[Georgia PSC 情况说明, 2026-03](https://psc.ga.gov/site/downloads/datacenterfactsheet.pdf)（高）]。2025 年佐治亚公用事业委员会两个席位因电价议题翻转给民主党——电价已是选举变量 [中, Quinn Emanuel §VI.I]。
- **联邦层面**：2026-03-04 Trump 促成"Ratepayer Protection Pledge"，Amazon/Google/Meta/Microsoft/Oracle/OpenAI/xAI 承诺为新数据中心自建或自购电力并承担电网升级成本；**行政方承认该承诺只是把企业已在做的事形式化，执行依赖州监管者** [中, [NYT, 2026-03-04](https://www.nytimes.com/2026/03/04/technology/ai-energy-pledge-white-house-trump.html)，转引自 Quinn Emanuel 注 108–109]。

法律定性：这些电价条款是**监管强制的 take-or-pay**，强度高于商业合同——由公用事业委员会背书、有抵押与退出费、且不属于破产可轻易拒绝的普通商业合同范畴（公用事业服务合同在破产中有特殊处理）。残余风险落在两个缺口：(1) 2025 年前已签约的存量负荷不受新电价约束；(2) 数据中心客户自身破产时，85% 最低账单同样沦为破产债权——抵押品与退出费只覆盖建设期成本的一部分。**若 AI 负荷预测系统性落空，超出合同保护的部分仍回落到纳税人**——这是本轮唯一没有"上限"的或有负债，因为上限由监管政治而非合同决定。

---

## 五、Vendor financing 承诺的排队：压力下的兑现顺序

- **NVDA→OpenAI**：2025-09-22 LOI 名义值 $100B（随每 GW 部署分批投资），**至 2026-03 仍未签约束性协议**（NVDA 10-Q 明示"无法保证按预期条款完成"）；2026-03-04 黄仁勋称 $100B "probably not in the cards"，实际落地为 **$30B 股权投资**（2026 年已执行）[中, [PYMNTS, 2026-03-04](https://www.pymnts.com/news/artificial-intelligence/2026/nvidia-signals-final-investments-in-openai-and-anthropic/)；research-01 §3 冲突提示②]。另有 $105B PORTS-Pike 残值担保（§一）——注意这是 NVDA 对 OpenAI 体系最大的单笔承诺，但受益结构是 SB Energy 物业 + OpenAI 租约，属 RVG 而非股权投资。
- **AMD 认股权证**：OpenAI（2025-10-06）与 Meta（2026-02，配套最高 $60B 采购）各获最多 1.6 亿股 AMD 认股权证，**行权价 $0.01**，分档归属条件 = 采购部署里程碑（满额须部署 6GW）**叠加 AMD 股价里程碑（末档 $600/股）** [高, [AMD IR, 2025-10-06](https://ir.amd.com/news-events/press-releases/detail/1260/amd-and-openai-announce-strategic-partnership-to-deploy-6-gigawatts-of-amd-gpus)；中, [Motley Fool, 2025-10-11](https://www.fool.com/investing/2025/10/11/should-you-buy-advanced-micro-devices-amd-stock-nov-4/)；中, [KuCoin 转引 SemiAnalysis, 2026-08-04](https://www.kucoin.com/blog/semi-analysis-amd-meta-openai-warrant-deals-could-slash-gpu-costs-near-zero)]。结构本质：**这是用"自己股价上涨的期权"支付采购折扣——只在好状态下兑现**。压力情景下部署里程碑与股价里程碑同时失败，权证自动蒸发；AMD 付出的对价为零，但对应收入也从未存在。它是"反兜底"：分布上把对价集中在牛市尾部。

**压力下的兑现顺序（从先死到后死）**：
1. **LOI/意向性承诺**（NVDA $100B 已示范）：无法律约束，压力下直接死亡。
2. **里程碑型股权对价**（AMD 权证）：条件不成就自动失效，无需任何一方违约。
3. **有条件信用增级**（Google-Fluidstack 兜底）：触发条件可被结构性规避（工期延误 180 天→永不触发）。
4. **待履行商业合同**（Oracle $300B、MSFT $250B、AWS $38B、CoreWeave $22.4B）：破产前靠重新谈判缩水，破产后被 §365 拒绝、沦为无担保债权。
5. **书面担保与购买义务**（NVDA $6.3B、Meta $28B RVG、NVDA $105B RVG）：正常经营状态下即须付款，只在**承诺方自身**资不抵债时才失效——它们的对手方风险锚定在承诺人（NVDA/Meta）的信用上，而非项目本身。
6. **监管强制 take-or-pay**（Ohio/Georgia 电价）：由州监管机构执行，强度与政治周期挂钩。

---

## 六、或有负债强度光谱

| 档位 | 法律性质 | 主体与量级 | 会计位置 | 压力下的命运 |
|---|---|---|---|---|
| 1 硬负债 | SPV 层面已发债 | Hyperion ~$27B（PIMCO 锚定）；xAI SPV $12.5B；Oracle 系列 ~$130B 总债务 | 在 SPV/发行人表上，母公司表外 | 由抵押品与租金流偿付；违约触发交叉违约级联 |
| 2 书面或有（条件+上限） | 购买义务/RVG | NVDA→CoreWeave $6.3B；NVDA PORTS-Pike RVG $105B；Meta RVG ~$28B；Google→Fluidstack >$5B | 仅脚注，无表内负债 | 正常状态下即须现金支出；触发条件与需求崩塌同频（wrong-way risk）；承诺人破产才失效 |
| 3 监管强制 | 公用事业电价 take-or-pay | AEP Ohio ≥25MW 客户 85%×12 年；Georgia >100MW 客户 15 年 | 客户侧为承诺披露；公用事业侧进费率基础 | 合同缺口外的搁浅成本社会化给纳税人——**无上限** |
| 4 可拒绝合同 | 待履行云合同 | OpenAI→Oracle $300B；OpenAI→MSFT $250B；OpenAI→AWS $38B；OpenAI→CoreWeave $22.4B | 云厂商 RPO 脚注；客户侧无披露 | §365 可拒绝 → 无担保破产债权；破产前以 SLA/交付抗辩重谈 |
| 5 里程碑对价 | 附条件权证/分期投资 | AMD 权证 2×1.6 亿股 @ $0.01；NVDA→OpenAI $30B（原 $100B LOI 已缩水） | 授予方按公允价值分期确认稀释 | 条件不成就自动蒸发，无人违约 |
| 6 纯隐性支持 | 无 | 市场对"Meta 不会弃 Hyperion"、"Musk 体系会输血 xAI SPV" 的默认 | 不存在 | 见 §七——要么被声誉强制兑现，要么被突然证伪 |

---

## 七、2008 SIV/AIG 教训的映射

**SIV 映射（对应档位 6 与档位 1 的关系）**。2007 年发起行对 SIV 只有流动性便利与声誉关联，法律上并无兜底义务；ABCP 市场冻结后，HSBC（2007-11，~$45B）与 Citigroup（2007-12-13，并表后资产 +$59B）先后把 SIV 资产**自愿并表**——隐性担保在危机中被声誉强制显性化，且兑现时点恰是发起行自身资本最紧的时刻 [高, [Citigroup 2007 10-K](https://www.sec.gov/Archives/edgar/data/831001/000119312508036445/d10k.htm)；中, Grokipedia/SIV 条目综述]。映射到本轮：Meta 对 Hyperion 的真实义务以 RVG $28B 为限，但市场定价（A+ 评级、PIMCO $18B 锚定）包含了"Meta 是实际承租人且不会走人"的无限假设。**SIV 教训不是"隐性担保会失效"，而是它的价值二元：发起行健康时它值 100 美分，发起行自身承压时它瞬间归零且无人能起诉**。差异点：本轮显性承诺普遍有上限与条件，比 SIV 的"无书面承诺"更诚实；但集中度远高——SIV 分散在数十家发起行，本轮隐性支持集中于 NVDA/Meta/Google/OpenAI 四个节点。

**AIG 映射（对应档位 2）**。AIG 的致命点不是 CDS 名义敞口（~$533B），而是**抵押品按市值追缴**把账面浮亏变成即时现金流出，且触发条件（评级下调+标的下跌）与 AIG 偿付能力恶化完全同频。本轮档位 2 承诺的结构同型：NVDA $6.3B 购买义务的触发条件（CoreWeave 容量卖不出去）就是 NVDA 芯片需求崩塌的同义词；$105B PORTS-Pike RVG 在 OpenAI 退租且 AI 机房残值崩塌时触发——同样是 NVDA 自身现金流最差的情形。**或有负债的清算顺序不由合同决定，由承诺人的资产负债表决定：档位 2 的承诺全部押注在 NVDA 与 Meta 不生病上。** 与 AIG 的缓冲差异：本轮承诺有名义上限、无逐日盯市追缴条款，时间结构上更接近"慢性失血"而非 AIG 的"保证金猝死"；但 Quinn Emanuel 已指出 GPU 抵押贷款的估值-保证金争端条款存在同样的按市值追缴动力学（§VI.E）——AIG 机制活在 CoreWeave/Fluidstack/Lambda 的 DDTL 里，而非活在科技巨头的担保里。

**一句话结论**：本轮真正硬的或有负债（档位 2–3）集中在 NVDA（$114.8B 披露敞口）与 Meta（$28B RVG + 承租人地位）两家；OpenAI 体系对外的一切采购承诺（>$600B 合同值）在法律上都是可拒绝的待履行合同，其硬度不高于 OpenAI 自身的持续经营能力；而"Meta/Musk 不会放弃 SPV"的市场默认，是 2007 年 SIV 式期权——免费持有，行权价是声誉。
