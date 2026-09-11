# 01 · AI 生物 uplift 证据（能力侧现状）

研究日期：2026-09-11。来源：arXiv/bioRxiv/Nature 系原文、SecureBio/Epoch/RAND/UK AISI 等机构报告、实验室官方文档；由研究代理检索直查，冲突口径并列呈现。

> **信息危害纪律**：本目录全部文件只记录研究结论、统计口径与阈值定义，不复现任何操作性细节（协议、参数、步骤）。这也是所引各评估报告的共同做法，此处引为方法论依据。

## 一、研究问题与总判

问题：**AI 今天到底把生物武器门槛降低了多少？**

总判（2026-09 时点，四句话）：

1. **端到端实证为零**：没有任何公开研究证明 AI 把一个无背景个人/小团体带到"获取＋武器化＋部署"闭环。
2. **任务级提升的证据在 2025 年转正并走强**：VCT 病毒学排障分数超 94% 专家百分位、英国 AISI 二次分析显示 AI 使非专家写出生物协议的可能性约 5 倍、RAND 内部研究者实测商业模型可就高后果病原体重建类任务给出准确逐步文字指导。
3. **方法论争议未决**：所有 uplift 随机试验都被批统计力不足或测错构念；2026 年出现首个"完整物理工作流零结果"的 RCT。
4. **结构性类比**：这就是 [04-my-forecasts](../agi-timelines/04-my-forecasts.md) 说的"基准–现实差距"在生物域的重演——**数字终点不等于物理执行力**。这条主线贯穿本目录全部追踪。

## 二、uplift 文献谱系（时间线）

| 时点 | 研究 | 设计 | 核心结论 | 方向 |
|---|---|---|---|---|
| 2022-03 | Urbina et al.（Nature Mach. Intell.） | 药物生成模型目标反向 | 6 小时产出约 4 万个计算预测有毒分子（未合成未验证）——文献起点 | — |
| 2023-06 | Soice et al.（MIT/Esvelt 组，arXiv:2306.03809） | LLM 协助非科学背景学生 | 约 1 小时内获规划与采购层面协助；作者定性判断无定量 uplift 值 | 正 |
| 2024-06 | OpenAI 早期预警研究（100 人 RCT） | 专家用 GPT-4 vs 无 | 专家准确率 6.00→6.88/10，**无统计显著性**，"mild uplift" | 反 |
| 2024 | RAND 红队（RRA2977-2 等） | LLM 组 vs 仅互联网组 | 攻击计划质量无可测差异 | 反 |
| 2025-04 | SecureBio/CAIS **VCT**（arXiv:2504.16137） | 322 题病毒学排障"隐性知识" | **o3 达 43.8%，超 94% 专家百分位**（专家基线 22.1%） | 正 |
| 2025-06 | Brent & McKelvey（RAND WR-A3853-1，arXiv:2506.13798） | 方法论批评＋实测 | 挑战"默会知识屏障"前提：主流商业模型已能就高后果病原体重建类任务提供准确逐步文字指导，既有评估系统性低估风险 | 正 |
| 2026 | Zhang et al.（预印本） | 57 名新手，数字生物学任务 | 答对几率比 OR≈4.16 | 正 |
| 2026 | Hong et al.（RCT） | 完整物理工作流 | 完成率**无显著提升**——首个物理端零结果 | 反 |
| 2026-08 | RAND 再分析（26 基准/45 模型） | 荟萃 | 易题饱和；**基准分不能预测湿实验滥用** | 方法论 |

注：DHS 委托的同类风险评估存在（2025），标题含"computational limits"的报告未能核实，待补。

## 三、评估基准现状

| 基准 | 时点 | 测什么 | 关键读数 / 局限 |
|---|---|---|---|
| WMDP（Stanford HASP/CAIS） | 2024-03 | 3,668 道危险知识多选（生/网/化）＋RMU 去学习防御 | Epoch 批评：更像知识问答且已趋饱和 |
| LAB-Bench（FutureHouse） | 2024-07 | 2,400+ 题，文献检索/图表/数据库/序列操作等科研实操 | 科研正用导向，双用含义间接 |
| **VCT**（SecureBio+CAIS） | 2025-04 | 322 题多模态病毒学排障隐性知识 | o3 43.8%；**GPT-5.5 预发布评估 52.0%（第 100 百分位）**（SecureBio，2026-04-09）。注意：常见误称"ViroCap"，实名 VCT |
| BixBench（FutureHouse+ScienceMachine，**非** Allen AI；AI2 对应物为 AstaBench） | 2025-03 | 50+ 真实生物信息学 agent 场景 | agent 化任务 |
| 2025–2026 新增族 | — | MBCT/HPCT/WCB、BioTIER、ABC-Bench、ABLE、**BIORISKEVAL**（Scale AI/SecureBio，测基因组模型数据过滤稳健性） | 基准供给正在专业化 |

**标志性事件**：GPT-5.5 预发布评估（SecureBio，2026-04-09）四项超人、但拒答沿"概念—实操"边界运作——"很可能限制新手 uplift、仍可能有助有经验行为者"（且系 API 层过滤被关闭条件下测得）。**独立机构在发布前评估前沿模型生物能力，2026 年起成为操作**——评估体系从实验室自评走向独立的转折点。

## 四、正反天平与我方读法

**已被证明的**：任务级数字提升（协议撰写 ~5 倍、VCT 超专家线、数字任务 OR≈4）。
**未被证明的**：端到端、湿实验执行、材料获取、规模化武器化。
**三个方法论缺口**（Epoch AI 2025-06）：评估透明度差、阈值含义不明、湿实验与材料瓶颈未测。

核心分歧在**"默会知识屏障"是否成立**：RAND 传统立场（屏障仍有效，红队无差异）vs Brent & McKelvey（屏障前提本身不成立，实测已穿透文字层）。2026 年 Hong et al. 的物理端零结果是反方最硬的一块，但它测的是"现有商业模型＋现有学生被试"——VCT 分数仍在爬升，两边的实验设计不在同一时间常数上。

我方读法：**证据结构像 2022–2024 年的编程 benchmark——分数先于现实，但现实迟早跟上**。跟踪两条线：VCT 等基准的分数线（先行指标），与首个"物理工作流正结果 RCT"的出现时间（滞后确认指标）。

## 五、生物能力模型与 agent 发布线

| 时点 | 系统 | 能力 | 双用风险讨论当时怎么说 |
|---|---|---|---|
| 2024-05 | AlphaFold 3（DeepMind+Isomorphic，Nature） | 全类别生物分子复合物结构预测 | 仅限服务器访问的政策引发学界公开异议——访问治理争论起点 |
| 2024-09 | AlphaProteo | 蛋白设计，7 靶点湿验证成功率 9–88%、亲和力高 3–300 倍 | 官方称做了生物安全评审、未开放全部权重；EMBO Reports 随即讨论三层防护 |
| 2024-09→ | Chai Discovery | Chai-1 以 Apache 2.0 **开源**、达 AF3 级精度 | "开源 vs 受限发布"的对照案例；后至 $400M C 轮，客户含 Lilly/Novartis/Pfizer |
| 2025-02 | Evo 2（Arc+NVIDIA+Stanford） | 40B 参数、9.3 万亿核苷酸基因组模型 | 官方以**剔除真核病毒基因组**作为安全措施；后续分析（Trends in Genetics、JHU）与 BIORISKEVAL 指出**微调即可低成本恢复被滤能力**——数据过滤不是系统性屏障 |
| 2025-02 | Google "AI co-scientist" | Gemini 2.0 多 agent 假设生成 | 后产品化；AMR/老药新用正用叙事 |
| 2025-05 | FutureHouse Robin | 宣称首个端到端科学发现（干性 AMD 老药新用，经湿验证） | 里程碑意义在"端到端"，不在此题本身 |
| 2025-03→2026 | Lila Sciences（Flagship 孵化） | 自动化实验室：$200M 种子（2025-03）→$235M A 轮（2025-09）→宣称自主评估约 **30 万 CAR-T 设计变体**并对外开放平台 | — |

三条结构性观察：

1. **"开源 vs 受限发布"的治理实验正在生物设计层重演**（Chai 开源 vs AlphaFold 服务器访问）——与权重开源争论同构，但这里扩散的是能力本身。
2. **能力层防线脆弱**：Evo 2 案例证明"数据过滤"防御可被微调绕过，防护主要落在部署政策层。
3. **全库最重要的单一趋势**：自动化湿实验室（Lila 类）把"数字终点→物理执行"这道关键屏障本身变成商品。uplift 争论的物理半边正在被商业化侵蚀——数字侧证据（§二）与物理侧商品化（本节）两条曲线的交汇点，是 05 预测的核心对象。

## 六、对预测的含义（喂给 [05](05-forecasts.md)）

- uplift 证据曲线形状：2024 反 → 2025 正 → 2026 混合但正方在物理端逼近。
- 与 OUR-018/019 的接口：**bio 路径不需要自动化研究员**——工具 AI 阶段即可兑现，这是它与起飞叙事的根本区别（05 展开）。
- CHK 素材：VCT 分数线跨档、首个物理工作流正结果 RCT、独立预发布评估是否常态化、自动化湿实验室对外服务规模。

## 七、防御侧对称追踪

- **DNA 合成筛查**：IBBIS（NTI 孵化）Common Mechanism——合成 DNA/RNA 订单免费开源筛查机制，2024 年配合美国联邦指南发布，Nature 2025 专题报道其为新兴标准；Battelle UltraSEQ 商用方案；JHU 维护提供商筛查工具清单。
- **药物/疫苗方向**：Lilly–OpenAI 抗耐药菌合作（2024-06）；盖茨基金会与 OpenAI $50M AI 健康合作（2026-01，转述，中可信度）。
- **监测**：CDC 废水监测系统（NWSS）扩展至耐药菌监测（机构合作项目，非前沿模型）。"CDC 与 OpenAI 合作"未能核实，待查。
- **净效应问题**：AI 让防御变强还是攻击变强——NTI/JHU 的"防御-攻击不对称"框架：攻击侧增益是倍增器（降低门槛），防御侧增益是检测器（缩短响应），两者时间常数不同。这是 05 情景设计的骨架之一。

## 数据可信度总注

学术原文（arXiv/Nature/RAND 报告）与机构官网（SecureBio、AISI、Anthropic/OpenAI/DeepMind 文档）为高可信度；Transformer/PYMNTS 类科技媒体为中；单条转述（盖茨-OpenAI 等）已单独标注。未能核实项：DHS"computational limits"报告标题、CDC-OpenAI 合作。2026 年预印本（Zhang et al.、Hong et al.）未经同行评审，结论按低-中可信度对待，重发期刊后复核。

## 来源

- https://www.nature.com/articles/s42256-022-00517-3 （Urbina 2022）
- https://arxiv.org/abs/2306.03809 （Soice 2023）；https://arxiv.org/abs/2506.13798 （Brent & McKelvey 2025）
- https://www.rand.org/pubs/research_reports/RRA2977-2.html （RAND 红队）
- https://openai.com/index/building-an-early-warning-system-for-llm-aided-biological-threat-creation/ （OpenAI 100 人 RCT）
- https://epoch.ai/gradient-updates/do-the-biorisk-evaluations-of-ai-labs-actually-measure-the-risk-of-developing-bioweapons （Epoch 2025-06）
- https://arxiv.org/abs/2403.03218 （WMDP）；https://arxiv.org/abs/2407.10362 （LAB-Bench）；https://arxiv.org/abs/2504.16137 （VCT）；https://arxiv.org/abs/2503.00096 （BixBench）
- https://securebio.org/virologytest/ ；https://securebio.org/blog/gpt-5-5-pre-release-assessment/ （VCT 读数与 GPT-5.5 预发布评估）
- https://www.nature.com/articles/s41586-024-07487-w （AlphaFold 3）；https://deepmind.google/blog/alphaproteo-generates-novel-proteins-for-biology-and-health-research/ （AlphaProteo）
- https://github.com/chaidiscovery/chai-lab ；https://www.fiercebiotech.com/biotech/chai-brews-400m-series-c-fuel-ai-used-lilly-novartis-and-pfizer （Chai）
- https://arxiv.org/abs/2502.18864 （AI co-scientist）；https://arxiv.org/abs/2505.13400 （Robin）；https://www.lila.ai/news （Lila）
- https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026 （国际 AI 安全报告 2026 版："担忧已 materialized"）
- https://www.aisi.gov.uk/frontier-ai-trends-report （UK AISI 趋势报告，5 倍协议撰写口径）
- https://ibbis.bio/our-work/common-mechanism/ ；https://www.nature.com/articles/d41586-025-03230-1 （IBBIS/Nature）
- https://www.reuters.com/business/healthcare-pharmaceuticals/lilly-partners-with-openai-develop-medicines-drug-resistant-bacteria-2024-06-25/ （Lilly-OpenAI）
