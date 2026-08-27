# 方法论、共识与调查

## A. 预测方法论

1. **生物锚定法（Bio Anchors）**——Cotra 2020（详见 01-timelines.md）：以生物参照（人脑毕生算力、进化搜索）锚定 TAI 所需算力，对照算力成本与预算趋势。中位 ~2050（2020 假设）。
2. **分解法（forecast decomposition）**——Kokotajlo《Draft report on AI timelines》(2021)：https://www.lesswrong.com/s/EcKbpm4f7fBwhxRZs/p/KrJfoZzpSDpnrv9va —— 把时间线问题拆成子问题（算力需求、算法进步、支出、部署），逐项给概率再合成。这是社区的招牌技术：显式蒙特卡洛模型（Guesstimate/Squiggle）上的参数分布，而非单点猜测。
3. **学术侧**：《Forecasting AI Progress: A Research Agenda》（Gruetzemacher 等, 2020, arXiv:2008.01848）：Delphi 专家法；配套调查（arXiv:2206.04132）：HLMI 50% by 2060。
4. **超级预测术 / 外部 vs 内部视角**：Tetlock 式参照类预测（外部视角）与机制分析（内部视角）结合，惯例是外部视角起步、向内调整。代表性争论：Karnofsky 的 outside view 论 vs Muehlhauser 对"史无前例技术没有参照类"的批评。社区组织：Samotsvety、Metaculus、LW 预测线程。
5. **基准/收入外推**（AI 2027 团队）：METR 时间视界 + 前沿收入曲线，是分解法在数据丰富化后的新形态。

**方法论谱系（我的概括）**：外部视角调查（AI Impacts）→ 分解式半内部视角模型（Bio Anchors、Kokotajlo）→ 内生增长/起飞仿真（Davidson）。三层互相校准。

## B. 共识与调查

- **AI Impacts 2023 专家调查**（2778 名已发表 ML 研究者，https://wiki.aiimpacts.org/...2023_expert_survey_on_progress_in_ai）：
  - HLMI 50% by **2047**（比 2022 调查的 2060 提前 13 年）；全面劳动自动化 2116。
  - HLMI 影响"极坏（如人类灭绝）"：中位 5%、均值 9%。
  - 智能爆炸可能：~29%；认为社会应更重视 AI 安全：70%。
- **AI 安全社区调查**（AI Impacts 2019/2021；~117 名 AI 风险从业者）：mean p(x-risk) ~30–40%，**中位 ~20–30%**。https://www.lesswrong.com/posts/QvwSr5LsxyDePK5s/
- **LW 社区普查**（2023，558 人）：AGI 时间线中位约 2030s 末–2040s，p(doom) 普遍两位数——显著高于主流研究者。
- **Conjecture 内部调查**：灭绝风险聚在 60–80%。
- **主流 vs 社区的鸿沟**：《Why Do AI Researchers Rate the Probability of Doom So Low?》（https://www.lesswrong.com/posts/727sAH7RWsxgg93Xz/）；学术分析 arXiv:2502.14870。

**共识图景**：主流研究者 p(doom) ~5–10%；LW/安全社区 20–40%+（极端到 80%）。时间线共识在快速收敛于"本十年到 2030 年代初"，但分布右尾极长。

## C. ASI / RSI 概念

- **超智能（Bostrom, 2014）**："在几乎所有领域大幅超越最好人类大脑的智能"；三分类：速度、集体、质量超智能。
- **RSI（递归自我改进）**：谱系从 Yudkowsky 2013 微观经济学 → Bostrom 起飞分析 → Davidson 软件反馈量化模型 → AI 2027 场景。2023 学术调查 ~29% "智能爆炸可能"标志此观点在主流的边界。
- **"工业爆炸"论证**：由 Davidson 的爆炸性增长模型（GWP 翻倍期缩至月/年级）+ Hanson《Age of Em》的增长模式转换框架承载。
