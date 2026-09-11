# AI 生物安全风险研究（ai-bio-risk）

研究日期：2026-09-11。来源：Anthropic/OpenAI/DeepMind 官方政策文档与系统卡（一手）、arXiv/bioRxiv/Nature 系原文、RAND/SecureBio/NTI/JHU/Epoch 等机构报告、Metaculus/CDC/USDA 页面直查、Federal Register/白宫/国会/EU/UNODA/中国部委官网（一手）；四路并行研究代理建库，冲突口径并列呈现。

**定位：AI×生物安全是本仓库风险判断（p(doom) 12%）中唯一可能在"工具 AI 阶段"就兑现的灾难通道——它不依赖起飞、不依赖自动化研究员，因此与 [agi-timelines](../agi-timelines/README.md) 的时间线之争正交。本目录追踪三条线：能力侧（uplift 证据曲线）、实验室侧（阈值框架触及史）、治理侧（筛查/义务/条约），并以自然疫情（H5N1 等）为背景基线面。**

> **信息危害纪律**：本目录只记录研究结论、统计口径与阈值定义，不复现任何操作性细节（协议、参数、步骤）——与所引各评估报告的共同做法一致。

## 文件结构

| 文件 | 内容 |
|---|---|
| [01-uplift-evidence.md](01-uplift-evidence.md) | 能力侧现状：uplift 实证文献谱系（Urbina 2022→2026 物理端 RCT）、评估基准（WMDP/VCT/LAB-Bench 族）、正反证据天平、生物能力模型与 agent 发布线（AlphaFold 3→Evo 2→Lila 自动化湿实验室）、防御侧对称追踪 |
| [02-lab-thresholds.md](02-lab-thresholds.md) | 实验室侧：RSP/Preparedness/FSF 三家阈值框架对照（档位定义原文＋译述）、版本史与修订方向、生物档位触及事件史（ASL-3 首启→"预防性按 High 处理"→威胁情报报告）、官方评估机构（CAISI/AISA） |
| [03-governance.md](03-governance.md) | 治理侧：美（EO 14110 生死→EO 14292/AI Action Plan/S.3741 筛查立法）、EU AI Act、英国、国际（BWC 十审≤2027）、中国（生物安全法＋两用物项＋NMPA AI 医药轨道，中文一手源）——总形状：治理重心从模型侧移向材料侧 |
| [04-threat-base-rates.md](04-threat-base-rates.md) | 威胁面与基率：既有量化分层（Ord/XPT/Sandberg-Bostrom/Millett）、历史"三连败"（奥姆/炭疽信/Rajneeshee）、Metaculus 直查快照（含 Q38589 ASL-4 时点）、自然疫情基线面（H5N1 现状/防御基线）、AI 监测净效应 |
| [05-forecasts.md](05-forecasts.md) | 我方预测：A 阈值评估/B 治理/C 事件/D p(doom) 生物分解（~2.5pp，不双重计分）＋三情景（α 防线粘住 45%/β 灰色侵蚀 35%/γ 门槛击穿 20%）；权威登记在 [predictions/ledger.md](../predictions/ledger.md) OUR-047+ |

## 核心论点（约 400 字）

**"AI 显著降低生物武器门槛"在 2026-09 仍无端到端实证，但正方证据在 2025 年转正、在物理端逼近**：VCT 病毒学排障上 o3 超 94% 专家百分位、GPT-5.5 预发布评估达 52%（第 100 百分位）、英国 AISA 二次分析显示 AI 使非专家写出生物协议的可能性约 5 倍；反方仍有 2024 年两份"无可测差异"RCT 与 2026 年首个物理工作流零结果。同时，**数字侧证据与物理侧商品化两条曲线正在夹击同一道屏障**——Lila 类自动化湿实验室把"数字终点→物理执行"的门槛本身变成商品（2026 年已自主评估约 30 万 CAR-T 设计变体），而 Evo 2 案例证明"数据过滤"防御可被微调绕过。

实验室阈值体系（RSP/Preparedness/FSF）已从文档走到操作：Anthropic 2025-05 首次预防性启用 ASL-3、OpenAI GPT-5 系常态"按 High 处理"、2026-09 起威胁情报报告开创滥用尝试披露流——但**生物档至今零实测越线**（对照：网络域 Critical 已被 GPT-6 Astra 实触及）。治理重心从模型侧（EO 14110 已撤销）移向材料侧（DNA 合成筛查，S.3741 两党推进）；净倾斜取决于**筛查覆盖率与自动化实验室扩散速度的赛跑**。

我方分解：p(doom) 12% 中生物通道约 2–3pp；未来五年中心情景是"灰色侵蚀"（0.35）而非灾难或安全；关键清算观察点是 Metaculus Q38589（Anthropic 首次报告 ASL-4 级披露，社区中位 2027-07，我方 0.35）。

## 追踪安排：watch/bio 季刊

- **节奏**：季度刊，与季度校准回顾（每季度首月第一周）同周出刊；重大事件（实测越线披露、γ 情景触发、BWC 大会）随时特刊。**创刊号：2026-10 回顾周**，以本目录五篇为建库基线，此后只记漂移。
- **每期固定巡检**：阈值触及事件史（02 §三）追加行、Metaculus 生物问题族（04 §三）直查快照、威胁情报报告披露流、H5N1 基线面、立法进展（S.3741/纽约州生效细节）。

## 与其他目录的衔接

- [agi-timelines/04-my-forecasts.md §D](../agi-timelines/04-my-forecasts.md)：p(doom) 12% 与 OUR-019（风险集中起飞阶段 0.70）——本目录 05 §D 做通道分解并标注张力（OUR-057）。
- [watch/capability](../watch/capability/2026-09-09-ai-timeline-watch.md)：GPT-6 Astra 首触 PF Critical（网络域）是 02 的对照锚；HF 失控事件链与 OUR-020 的"失控"叙事在生物域的对应物是威胁情报报告。
- [china-ai-race](../china-ai-race/README.md)：中国生物安全立法体系与 BWC 立场（赞成核查、美国反对）是 03 §六的主题；后续 watch/bio 应核查中国头部模型商有无 RSP 类框架。
- [predictions/ledger.md](../predictions/ledger.md)：OUR-047~060、EXT-071~080、CHK-020~028 的唯一权威登记处。

## 数据可信度总注

实验室官网政策文档/系统卡、Federal Register/国会/中国部委原文、arXiv/Nature/RAND 原典、Metaculus/CDC/USDA/WHO 直查为高；NYT/BBC/FedScoop 高；Frontier Model Forum 汇编、governance.ai/Epoch/SecureBio 分析为中-高；Transformer/EA Forum/Zvi 及单条转述为中。各文件末尾附完整来源与"未能核实项"清单（合计约 20 项，最重要的三项：NTI–Palantir 合作传闻、GJO 当前值、纽约州法签署状态）。2026 年未经同行评审的预印本一律按低-中可信度对待。
