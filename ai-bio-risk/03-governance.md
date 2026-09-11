# 03 · 治理与政策（美 / 欧盟 / 英国 / 国际 / 中国）

研究日期：2026-09-11。来源：Federal Register/白宫/国会官网（一手）、EU digital-strategy、UNODA、英国 gov.uk、中国官方文件原文（中文一手）；由研究代理检索直查，立法进展以 congress.gov/CRS 口径为准。

## 一、总体形状：治理重心从"模型侧"移向"材料侧"

一句话总览：**美国把 AI 生物治理的重心从"模型报告义务"（已死）转向"合成 DNA 供给链筛查"（在途）；欧盟走模型侧义务路线；英国做评估与标准输出；国际条约层（BWC）原地踏步；中国走体系化立法＋AI 医药应用导向的另一轨道。** 四条轨道互不咬合——这是与 AI 治理本身（至少有峰会网络）相比更碎片化的格局。

## 二、美国

### 时间线

| 时点 | 事件 | 内容与现状 |
|---|---|---|
| 2023-10-30 | **EO 14110**《安全、可靠、可信的 AI》 | 依《国防生产法》要求大算力训练（>10^26 FLOPs 量级）报告；要求对具生物武器潜力的双用途基础模型红队测试后方可供联邦使用 |
| 2025-01-23 | **EO 14179** 撤销 EO 14110 | 训练算力/生物红队报告义务随之失效（FR 2025-02172）。**截至 2026-09 未见恢复该类报告义务的行政或立法动作**（未能核实存在） |
| 2024-10 → 2025 | HHS《核酸合成筛查框架》 | 自愿性指南（更新 2023-03 OSTP 版）；2025 年起联邦资助采购须来自筛查合规供应商；ASPR 正依 EO 14292 修订/替换该政策 |
| 2025-05-05 | **EO 14292**《改进生物研究安全》 | 要求制定含"全面、可扩展、可验证的核酸合成筛查"的战略，**覆盖非联邦资金场景**——联邦筛查约束的扩围起点 |
| 2025-07-23 | **America's AI Action Plan** | 要求受联邦资助机构使用实施 DNA 筛查的合成核酸供应商；强化商务部/**CAISI**（NIST 下属）对前沿模型（含生物风险）的评估 |
| 2026-09-03 | 《Ban ASI Act》提案（Sanders/Casar） | 本仓库时间线事件（见 [watch/capability 第二期](../watch/capability/2026-09-09-ai-timeline-watch.md)）：非生物专门立法，但为 AI 安全立法车辆的最新状态 |

### 国会

- 118 届：Peters S.2399《AI 与生物安全风险评估法》（2023-07-19，要求 ASPR 评估 AI 病原体风险）、Markey S.2400 等**均未通过**。注意：AI-bio 法案主发起人为 **Peters/Markey**（非 Wyden，常见误记）。
- 119 届：**S.3741《2026 生物安全现代化与创新法案》**（Cotton–Klobuchar，2026-01-29，CRS IF13269 跟踪）——要求商务部对核酸合成提供商及设备制造商立法规制，**首个获两党参议员支持的联邦强制筛查立法**，尚在委员会；另有 S.4069（AI 生物数据标准）。
- BARDA/ASPR：未发现专门命名的 AI×bio 项目（未能核实），角色主要是核酸筛查政策执行与 AI 辅助医药物资开发。

### 州与行业

- 州：纽约 A3283C/S9279A（基因合成供应商与设备制造商监管）**2026 年两院通过**（新增公共卫生法 32-B 条，授权州卫生厅发布筛查规程）——州长签署/生效日期未能核实；加州 AB 1864（2025）拟规管台式核酸合成设备。
- 行业自律：**IGSC**（国际基因合成联盟）成员逾 40 家、覆盖全球约 80% 商业合成产能，已发布《协调筛查协议 v3.0》；**IBBIS** 开源 Common Mechanism 筛查工具（≥50 nt）并于 2025-11 加入 IGSC 对接标准、发布客户筛查白皮书（与 [01 §七](01-uplift-evidence.md) 互链）。

## 三、欧盟

- AI Act 2024-08-01 生效，分阶段：**2025-08-02 GPAI 义务适用**（第 55 条系统性风险模型义务）；**2026-08-02 附件三高风险系统义务适用**；2027-08 起附件一嵌入式产品过渡。
- CBRN 落点：GPAI《行为准则》（2025-07-10 发布）"安全与保障"章节要求系统性风险提供方评估四类特定风险，**CBRN 为其一**（AI 降低化生放核攻击门槛或放大影响）；欧委会 AI Office 选定 SaferAI 提供 GPAI 模型 CBRN 风险评估技术支持（与 [02 §四](02-lab-thresholds.md) 的独立评估生态互链）。
- 截至 2026-09 **未见 CBRN 专项执法案例**；行为准则属自愿遵守的合规推定路径。

## 四、英国

- AISI→**AISA**（2025-02，DSIT 下属，转国家安全取向），化生放核滥用为核心领域之一；设 Chem-Bio 生物模型评估岗位，《Frontier AI Trends Report》（2025-12）显示生物基准已超 PhD 专家水平（见 [01](01-uplift-evidence.md)）；与 Apart Research 合办 2026-04 AIxBio 黑客松。
- 政策文件：《英国生物安全战略》（2023-06）＋三份实施报告（最近一份覆盖 2025-07~2026-07）；Alan Turing 研究所 CETaS《AI 与工程生物学：国家安全影响》（2026-06-25）提出"软主权框架"——建议加强生物数据治理、将英国打造为基因合成筛查与云实验室监管的标准输出国。

## 五、国际

- **BWC（生物武器公约）**：第九次审议大会（2022）设立"加强公约工作组"（2023–2026 政府间进程，mandate 覆盖遵约与核查）；第 5 次会议（2024-12）因俄罗斯阻止共识受挫；第 6 次（2025-08-11~22）、第 7 次（2025-12-08~12）举行；**第十次审议大会经 2022 年决定"不迟于 2027 年"在日内瓦举行**（精确日期未公布）。
- **WHO**：核心文件仍为《AI 大型多模态模型伦理与治理指南》（2024-01-18，40 余项建议）；2025–2026 未见专门的 AI×生物安全新文件（未能核实）。
- **峰会线**：Bletchley 宣言（2023-11）列生物风险；**首尔峰会（2024-05）16 家公司承诺前沿 AI 安全（含 CBRN 能力阈值、评估与红队）**——这是 [02](02-lab-thresholds.md) 三家阈值框架的政治源头；巴黎 AI 行动峰会（2025-02）宣言约 60 国签署（美英未签），AI×bio 议题主要经 NTI|bio–RAND、IBBIS 边会推进；《国际 AI 安全报告》（Bengio 主持，2025-01 首版/2026-02 二版）含生物风险章节，二版称相关担忧已"materialized into concrete developments"。

## 六、中国（中文一手源）

| 维度 | 现状 |
|---|---|
| 体系立法 | 《生物安全法》2020-10-17 通过、**2021-04-15 施行**（10 章 88 条）：生物技术研发按高/中/低风险分类管理，病原微生物实验室、人类遗传资源等制度 |
| 研发安全 | 科技部《生物技术研究开发安全管理办法》（2017-07，国科发社〔2017〕199 号）确立研发风险分级与机构自管（2019 年曾就上升为条例征求意见，未见落地） |
| 出口管制 | **《两用物项出口管制条例》（国务院令 792 号，2024-09-30 公布、2024-12-01 施行）**＋同步施行的含生物两用物项管制清单——管控生物物项跨境转移 |
| 实验室 | 《病原微生物实验室生物安全管理条例》（2004 颁布、2018 修订）继续作为实验室层级核心法规 |
| AI＋医药 | NMPA《药品监管人工智能典型应用场景清单》（2024-06，15 项）；卫健委等三部门《卫生健康行业人工智能应用场景参考指引》（2024-11，84 场景）；**NMPA《关于"人工智能+药品监管"的实施意见》（2026-04，七大方向、监管大模型部署）**——应用侧活跃、风险侧未见专门框架 |
| 国际立场 | 《全球人工智能治理倡议》（2023-10）；《新时代的中国军控、裁军与防扩散》白皮书（2025-11-27）主张 BWC 谈判达成**含有效核查机制、有法律约束力的议定书**，批评美国独家反对核查谈判 |

中国观察（与 [china-ai-race](../china-ai-race/README.md) 的方法论一致）：中国的生物安全治理是**立法先行、体系化**的（法＋条例＋清单三层），与美国的"政策摆动＋供给链筛查"形成对照；AI 侧监管资源集中在医药应用（NMPA 轨道），**前沿模型×生物风险的实验室自律框架在中国头部模型商中尚无公开对应物**（GLM/Qwen 未发布 RSP 类文档——待 watch/bio 按期核查）。**注意一个反直觉结构：BWC 核查问题上中国赞成、美国反对**——与 AI 条约谈判（OUR-021 的中美结构）方向相反，说明"谁要约束谁"在不同技术域完全不同。

## 七、对预测的含义（喂给 [05](05-forecasts.md)）

- 政策摆动信号本身可预测：模型侧义务恢复（低）、供给链筛查联邦强制（中-高，两党+两行政分支方向一致——S.3741 与 AI Action Plan/EO 14292 同向）。
- BWC 是"低配版 OUR-021"：结构相似（核查机制）、基率更差（30 年无果），作对照锚。
- 治理重心"从模型到材料"的迁移若持续，意味着**防线落在 DNA 合成筛查覆盖率上**——与 [01 §五](01-uplift-evidence.md) 自动化湿实验室扩散的赛跑，是净倾斜的关键变量。

## 数据可信度总注

Federal Register/白宫/国会/欧盟/UNODA/中国部委官网为一手（高）；CRS/CSET/CETaS 为研究机构二手（中-高）；medicaldaily 等转述已标注。**未能核实项**：恢复 EO 14110 式义务的任何动作（未发现）；BARDA 专门 AI×bio 项目（未发现）；欧盟 CBRN 执法案例（未发现）；WHO 2025-26 新文件（未发现）；纽约州法签署/生效细节；BWC 第十次审议大会精确日期；中国头部模型商有无 RSP 类内部框架（无公开文档）。

## 来源

- https://www.federalregister.gov/documents/2025/01/31/2025-02172/ （EO 14179，一手）
- https://www.whitehouse.gov/presidential-actions/2025/05/improving-the-safety-and-security-of-biological-research/ （EO 14292，一手）
- https://www.whitehouse.gov/wp-content/uploads/2025/07/Americas-AI-Action-Plan.pdf （一手）
- https://aspr.gov/readiness-response/medical-countermeasures-biodefense/s3/synthetic-nucleic-acid-screening （一手）
- https://www.congress.gov/bill/119th-congress/senate-bill/3741 ；https://www.congress.gov/bill/118th-congress/senate-bill/2399 （一手）
- https://www.nysenate.gov/legislation/bills/2025/A3283/amendment/C ；https://www.genesynthesisconsortium.org/ ；https://ibbis.bio/ibbis-joins-international-gene-synthesis-consortium/
- https://www.digital-strategy.ec.europa.eu/en/policies/contents-code-gpai ；https://www.digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai ；https://artificialintelligenceact.eu/code-of-practice-overview/ ；https://www.safer-ai.org/saferai-selected-to-support-eu-ai-act-implementation-through-cbrn-risk-assessment
- https://www.gov.uk/government/news/tackling-ai-security-risks-to-unleash-growth-and-deliver-plan-for-change ；https://www.aisi.gov.uk/frontier-ai-trends-report ；https://cetas.turing.ac.uk/publications/ai-and-engineering-biology
- https://docs-library.unoda.org/ （BWC/WG/7/CRP.1/Rev.1）；https://media-publications.unoda.org/documents/BWC_at_Fifty.pdf
- https://www.who.int/news/item/18-01-2024-... （LMM 指南）；https://www.gov.uk/government/publications/frontier-ai-safety-commitments-ai-seoul-summit-2024/
- https://www.nti.org/news/nti-bio-rand-advance-aixbio-safety-during-paris-ai-action-summit/
- 中国：http://www.npc.gov.cn （生物安全法）；https://www.most.gov.cn （研发安全管理办法）；https://www.mofcom.gov.cn/zcfb/dwmygl/ （两用物项条例）；https://www.nhc.gov.cn/guihuaxxs/c100133/202411/3dee425b8dc34f739d63483c4e5c334c.shtml ；https://www.nmpa.gov.cn/xxgk/fgwj/gzwj/gzwjzh/20260402091552114.html （2026-04 实施意见）；https://www.scio.gov.cn/zfbps/zfbps_2279/202511/t20251127_940277.html （军控白皮书）；https://www.mfa.gov.cn/ （全球 AI 治理倡议）
