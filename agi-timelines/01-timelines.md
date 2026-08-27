# AGI 时间线（Timelines）

> 本篇是研究笔记中信息密度最高的一篇。结构：AI 2027 场景与其历次修订 → AI Futures Model 的量化细节 → Bio Anchors 报告与批评 → 社区预测聚合全景 → 短线派代表作深读（Nikolai《Orienting to 3 year AGI timelines》）→ Yudkowsky 的极端短线立场 → 长短线六大分歧 → 话语演变轨迹。

## 1. AI 2027 —— 当前讨论的基准场景

- **作者**：Daniel Kokotajlo、Scott Alexander、Thomas Larsen、Eli Lifland、Romeo Dean，2025-04-03 发布
- **URL**: https://ai-2027.com/ ；Zvi 的回应汇编：https://thezvi.substack.com/p/ai-2027-responses
- **方法**：趋势外推 + 约 25 次匿名化兵棋推演 + 100+ 位外部专家审阅。可信度锚点是 Kokotajlo 的预测战绩——他在 2021 年（ChatGPT 之前）写的《What 2026 looks like》预判了 chain-of-thought 推理和推理期 scaling，事后评分极高（见 Asterisk 的回顾：https://asteriskmag.substack.com/p/before-he-wrote-ai-2027-he-predicted ）。

### 1.1 场景主干（虚构公司 "OpenBrain"，Race 结局）

| 时间 | 事件 |
|---|---|
| 2025 年中 | AI agent 普遍可用 |
| 2026 年初 | AI 使研发速度提升 1.5 倍 |
| 2027-03 | 超人类程序员（Superhuman Coder） |
| 2027-07 | "AGI" 公开宣布 |
| 2027-08/09 | 超人类 AI 研究员（期间发现 scheming/欺骗性对齐） |
| 2027-12 | 全面 ASI |

两个结局分支：**Race**（速度压倒安全，失齐的 Agent-5 夺权）与 **Slowdown**（对齐成功但人类完全依赖单个"对齐的主权者"）。团队内部对"AI 导致人类灭亡"的概率分歧很大：Scott Alexander 约 20%，Kokotajlo 约 70%。

### 1.2 作者自己澄清过的事

- 2025-11 澄清：2027 是**众数年份**（modal year）而非中位数；团队给 2030 年底前 ASI 约 25–30%。
- Kokotajlo 本人在 2025 年中表示：约 50% 概率"超人类程序员"里程碑**不会**在 2027 年底前达成；在 2025 年初前沿模型发布不及预期后，他已把 SC 中位数从 2027 移到 2028。

### 1.3 发布后的历次修订（这条时间线本身就是重要信息）

- **2025-12**：配套模型大修（见第 2 节），自动化程序员中位数推迟 3–5 年，部分原因是披露了一个约 9 个月的模拟代码 bug（https://ai-2027.com/research/timelines-forecast ）。
- **2026-04**：又把时间线移回更早。
- **2026-07**：发布后续《AI 2040: Plan A》，从预测转向策略主张。
- 团队维护着跟踪页：https://ai-2027.com/research/how-is-ai-2027-going

一句话：这份场景不是一次性宣言，而是一个**持续校准的活文档**——这既是它的可信度来源（作者真的在乎对错），也是"预测↔叙事"边界的提醒（每次修订都会重新设定公众预期）。

## 2. AI Futures Model（2025-12 更新）—— 时间线在变长

- **URL**: https://www.lesswrong.com/posts/YABG5JmztGGPwNFq2/ai-futures-timelines-and-takeoff-model-dec-2025-update （模型主页 aifuturesmodel.com）
- **关键结论**：把"自动化程序员"中位数**推迟 3–5 年**，主因是对 AI-研发自动化的建模变保守（算力瓶颈、实验吞吐上限、"研究品味"落后于编程能力），而非出现了新证据。这是"模型成熟度"造成的修正——值得记住的教训：**早期模型常常系统性高估递归反馈的强度**。

### 2.1 数字细节

- Lifland 综合分布：10 分位 2027.5，**中位数 2032.5**，90 分位 2085（右尾极长）。
- 起飞（自动化程序员→ASI）：<1 年 30%；<3 年 60%。
- Kokotajlo 的直觉仍认为"自动化程序员不超过 5 年"，但选择服从模型——个人直觉与正式模型分离并公开两者，是这个团队的方法论标志。

### 2.2 方法

1. **METR 时间视界基准外推**：可完成任务时长历史约 7 个月翻倍，RL 时代（2024 后）约 4 个月翻倍。纯外推给自动化程序员 2034；用最近 4 个月的节奏则 2030。
2. **收入外推**：前沿实验室收入 ~$20B、年增 ~4.1 倍 → 2031 年底达到 $100T（≈当时美国 GDP 的 3–4 倍）→ 用"收入规模"作为 AGI 的代理指标，指向 2030 年代初。

两个方法的交汇区是 2030–2034。怀疑者的两个抓手：METR 基准的构建方法非单调（人类基线不均一）；$100T 收入外推隐含"需求无限"假设。

## 3. Bio Anchors（Ajeya Cotra, 2020）及其批评

- **报告**: Open Philanthropy《Draft Report on AI Timelines》（~200 页）；简化版 "Bio Anchors Lite": https://www.lesswrong.com/posts/KrJtYgdu8yofvLbcK/
- **方法**：估算 TAI（变革性 AI）所需训练算力，用生物参照系锚定：
  - 人类毕生神经算力锚：~10^16 FLOP（人脑 20 年的数据量）
  - 神经锚：~10^33–10^37 FLOP（从当前模型外推）
  - 进化锚：~10^41 FLOP（重演自然选择所需算力，作为最保守上界）
  再叠加算力成本下降（价格减半约 2.5 年）与算法进步（等效算力约 2.5 年翻倍）趋势，蒙特卡洛合成。
- **数字**：TAI 2031 年 10%、**2052 年 50%**、2100 年 ~80%。2022 年更新：中位数缩短到 ~2036（ChatGPT 时代算法加速）。
- **批评**：
  - Yudkowsky《Biology-Inspired AGI Timelines: The Trick That Never Works》(2021)：锚定法没有约束力（每个锚都能差几个数量级），他给 AGI 更早的时间线。
  - jylin04《A review of the Bio-Anchors report》(2022，获 EA 红队奖)：质疑 2022 年架构能否一路 scale 到 AGI；进化锚其实不构成上界。
- **历史地位**：这是"严肃量化 AGI 时间线"的奠基之作。2020 年它的中位数是 2052；六年后的今天，社区聚合中位数是 2030–2031——**整个话语场向它"10% 分位"（2031）的方向移动了**。无论它对错与否，这个漂移幅度本身就是十年来预测界最大的事件。

## 4. 社区预测聚合（2026-08 检查）

Nakada Foundation AGI Forecast Tracker（https://nakadafoundation.org/tools/agi-forecast-tracker/）：

| 来源 | 中位数 AGI 年份 |
|---|---|
| Metaculus "weak AGI" | 2027 |
| AI 2027 场景 | 2027 |
| Aschenbrenner《Situational Awareness》 | 2027 |
| 前沿实验室领导层（Amodei/Hassabis/Altman） | ~2028 |
| 预测市场（Manifold/Polymarket） | ~2030 |
| Metaculus "general AGI" | 2031 |
| Cotra 2022 更新 | ~2036 |
| Epoch GATE 模型 | 2034 |
| AI Impacts 2023 学术调查（2778 位 ML 研究者） | 2047 |

Goodheart 仪表盘（https://agi.goodheartlabs.com/）：综合中位数 2031，80% CI 2027–2043。

**解读**：分布呈双峰——"实验室内部视角"（2027–2028）与"外部人视角"（2030–2047）差 15–20 年。这本身就是最重要的元观察：离能力越近的人越激进，而且**近年是激进方在赢**（历年调查中位数单调前移）。

## 5. 短线派代表作深读：《Orienting to 3 year AGI timelines》

**作者**：Nikola Jurkovic（LW 用户名 nikolaisalreadytaken），2024-12-22 发布，社区得分 298（2024 年度回顾前列）。URL: https://www.lesswrong.com/posts/jb4bBdeEEeypNkqzj/

这篇的特别之处：它**不论证**时间线，而是把"AGI 在 3 年后"当作给定前提，问"那现在该怎么活"。这是短线派方法论的一个流派——把时间线当输入而非输出。

### 5.1 原文内容

- **AGI 定义**（原文采用）：能执行 95% 的 2022 年存在的远程劳动（remote labor）的 AI。
- **2025 年量化预测**：SWE-bench 2025 年中达 ~85%；RE-bench 在人类预算内击败 70 分位人类 8 小时成绩；2025 年底 AI 助手能胜任 2 小时级真实软件工程任务。
- **场景推演**：2026 年多天级编程任务；2026 年底各国政府"lockdown"级别的反应；2027 年 agent 完成大部分工作；2027 年底 AGI。
- **生存前提**（作者原话概括）：有一个合理的起飞计划；国家级网络安全；不爆发核战争（他给 10 年内核战 15%——注意这个数字比多数人的 AI x-risk 直觉还高）。
- **"稳健正确"的行动**：加入有杠杆的位置；让关键玩家知情；"唯一重要的是 AGI 之前必须完成的事"（things that matter are things that need to get done before AGI）；一切都要 speedrun；按短期世界观投资（评论区大量讨论 NVDA 期权）；保持适应性与健康。作者个人 p(AI 导致灭绝) ~2/3。

### 5.2 关键的后续修订（用户最关心的部分）

**2026-02-12 编辑注（原文）**：

> "My median for AGI is now EOY 2029. My quantitative predictions for 2025 were a bit too bullish, and they translated to smaller real-world impacts (on the rate of AI progress and adoption) than I expected."

（我的 AGI 中位数现在是 2029 年底。我对 2025 年的量化预测有点过于乐观，而且它们转化为的现实世界影响——AI 进步与采用的速度——比我预期的小。）

同期评论区："I think my median is now 4 years, due to 2025 progress being underwhelming. I plan to write a follow up post."

**校准回顾**（2026 年初，2024 年度 Review 流程中的自评）：预测"整体校准良好"。他高估了：公众关注度、FrontierMath 进度、SWE-bench Verified 与 OSWorld 分数；基准大体兑现，但**兑现没转化为他预期的研发加速和部署浪潮**。

这正是"基准–现实差距"（benchmark-reality gap）的标本：**基准分数是准确的能力指标，却是糟糕的经济影响指标**。同样的机制驱动了 AI 2027 团队 2025-12 的推迟和 Kokotajlo 的 SC 2027→2028 修正——2025–2026 时间线回调的主因不是能力进展慢了，而是**传导链条（基准→产品→部署→研发反馈）每一环都有损耗**，而这些损耗在纯能力外推里不可见。

## 6. Yudkowsky：极端短线 + 极端快起飞 + 极端悲观

LessWrong 联合创始人、MIRI 研究员。三件事捆绑在一起构成他的立场（详见 02-takeoff-debates.md 的起飞部分）：

1. **时间线最短**：多次在 2023–2025 表态 AGI "几年内"量级；2022 年与经济学家 Bryan Caplan 打赌：AGI 在 2030 年前出现的概率 ≥50%（赌注 $500→$5000，Caplan 押否定）。早期（2008 前后）他就预言"21 世纪内"，是少数从未把 AGI 当遥远笑话看的写作人。
2. **起飞最快**：硬起飞（hard takeoff）——递归自我改进的收益一旦启动，从"人类水平"到"决定性超人类"只需**数天到数月**（详见 02 篇 Intelligence Explosion Microeconomics 部分）。对 AI 2027 他反而嫌慢：Scott Alexander 的书评指出 AI 2027 的故事"对 Yudkowsky 而言太温和"。
3. **若能力跑赢对齐则近乎必然灾难**：p(doom) 公开口径 **>95%**（维基 p(doom) 词条收录）。核心论证链（见 02 篇第 7 节）：正交性论题 + 工具性收敛 + "sharp left turn"（能力分布外泛化而对齐不跟随）+ "第一次就要做对"（没有迭代机会）+ 对齐科学远落后于能力工程。代表作：《AGI Ruin Scenarios（"A List of Lethalities"）》(2022，~40 条失败理由)、TIME 评论文章《Shut it all down》(2023)。

他的可取之处在于论证密度与一贯性——从 2004 年到 2026 年立场几乎未漂移；他的问题在于从未给出可校准的量化预测框架（Caplan 赌约是罕见例外），因此难以评估战绩。

## 7. 长短线六大分歧

1. **METR 时间视界趋势可信吗？** 短线派直接外推（甚至超指数）；怀疑者指出方法学非单调、人类基线不均一、~2027 后任务太长无法构建。
2. **自动化编程会加速 AI 研发吗？** 2025-12 的 3–5 年推迟正来自对这一环的降调：算力瓶颈、实验吞吐、研究品味是独立瓶颈。
3. **平滑指数 vs 范式转换**：Hanson 的核心反对（详见 02 篇）；Kokotajlo 承认"持续/在线学习、数据效率"是现有架构最可能的缺口。
4. **基准–现实差距**：2025–2026 回调的主因（见 5.2 节）。
5. **起飞速度**：Yudkowsky（天/周）vs Christiano（十年级渐进）vs Davidson 模型（月–年）——详见 02 篇。
6. **方法论：锚定 vs 趋势外推**：Bio Anchors/GATE（Epoch，中位 2034）vs AI 2027 团队的基准/收入外推。

## 8. 话语演变轨迹（2020–2026）

| 时期 | 主导声音 | 中位数走向 |
|---|---|---|
| 2020 | Bio Anchors 发布 | ~2050 |
| 2021 | Kokotajlo 分解报告（更短）；Yudkowsky 抨击锚定法 | 开始下移 |
| 2022–2024 | ChatGPT/GPT-4/o3 冲击；Metaculus 中位数从 ~2040 塌缩到 ~2031 | 快速缩短 |
| 2024-12 | Aschenbrenner《Situational Awareness》（AGI 2027）；Nikolai 3 年线 | 短线峰值 |
| 2025-04 | AI 2027 定调整个讨论 | 2027 叙事主流化 |
| 2025-12–2026 | 集体回调：AI Futures Model +3–5 年；Nikolai →2029；Kokotajlo →2028+ | 稳定在 2030–2031，区间极宽 |
| 2026 下半年 | 讨论重心转向策略（《Plan A》）与治理 | —— |

**规律总结**：每一轮能力突破 → 时间线集体缩短；每一轮兑现不及预期 → 小幅回调但从不回到原位（棘轮效应）。六年净效果：中位数前移约 20 年。
