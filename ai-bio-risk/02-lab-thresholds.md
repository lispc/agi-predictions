# 02 · 实验室生物阈值框架（实验室侧现状）

研究日期：2026-09-11。来源：Anthropic/OpenAI/DeepMind 官方政策文档与系统卡（一手）、Frontier Model Forum 阈值汇编、SecureBio/Epoch/governance.ai 等第三方分析。档位定义给出英文关键措辞＋中文译述，冲突口径并列。

## 一、三家阈值框架对照

| 维度 | Anthropic RSP（v3.4） | OpenAI Preparedness Framework（v2） | Google DeepMind FSF（v3.1） |
|---|---|---|---|
| 首版 → 现行 | 2023-09-19 → 2026-07-08 生效 | 2023-10 概念 / 2023-12-18 Beta → 2025-04-15 v2 | 2024-05-17 → 2026-04-17 v3.1（引入 TCL） |
| 生物档位定义（原文关键句） | CBRN-3（ASL-3）："meaningfully uplift the ability of individuals or small groups…to acquire, weaponize, and deploy CBRN weapons **compared to a baseline of publicly available information**" | Critical："meaningfully uplifts actors with limited resources or expertise to create, obtain, or use high-impact bioweapons resulting in **100+ deaths**"；High："…approach **the frontier of publicly known science**" | CBRN Uplift 1："significantly uplift the ability of **low-resourced actors** to acquire, weaponize, and deploy biological and chemical weapons in a way that would cause **mass casualties**" |
| 中文译述 | 相对公开信息基线，显著提升个人/小团体获取、武器化、部署 CBRN 武器的能力（CBRN-4：使开发"新型"CBRN 武器成为可能） | Critical：显著提升资源/专业受限者造成百人以上死亡的能力；High：接近公开科学前沿（**唯一给出量化死亡门槛的框架**） | 显著提升低资源行为者造成大规模伤亡的生/化武器能力 |
| 触发处置 | ASL-3：分级访问＋强化尽调；部署安全措施（Constitutional Classifiers 等） | Medium/Low 方可部署；**Critical 不予部署** | CCL 触发→对应缓解措施与披露义务 |
| 公开触及史 | **2025-05-22 首次启用 ASL-3**（Opus 4 CBRN，预防性临时措施） | o3"濒临"High（2025-04）；GPT-5 系"treated as High…below Critical"（预防性归类） | 无；Gemini 3 Pro 首份评估（2025-11-18）：生物域未达 |

**共同结构**：三家都是"相对基线的 uplift"定义而非绝对能力定义——因此阈值判定高度依赖评估方法，而评估方法论本身正处争议中（见 [01 §四](01-uplift-evidence.md)）。**阈值体系与评估体系是互相悬置的两半**，这是跟踪的基本盘。

## 二、版本史与修订方向

**Anthropic RSP**：v1.0（2023-09-19）→ v2.0（2024-10-15，细化 ASL-3 预案）→ **v2.1（2025-03-31，新增"中等资源国家项目"阈值**："substantially uplift the development capabilities of moderately resourced state programs"——把国家级行为体写进框架）→ v2.2（2025-05-14）→ v3.0（2026-02-24，全面重写：Frontier Safety Roadmaps＋Risk Reports，新增超出 ASL-3 标准的 CBRN 阈值）→ v3.3（2026-05-26，修订"新型化生武器生产"阈值）→ v3.4（2026-07-08 现行）。

**OpenAI PF**：v0 概念（2023-10-25 DevDay）→ Beta（2023-12-18）→ v1（2024-05）→ **v2（2025-04-15，CBRN 收窄为"Biological and Chemical Capability"跟踪类别，新增 AI 自我改进类别**）。

**DeepMind FSF**：v1.0（2024-05-17）→ v2.0（2025-02-04）→ v3.0（2025-09-22）→ v3.1（2026-04-17，Tracked Capability Levels）。

修订方向的双向解读（并列，不裁决）：

- **强化侧**：Anthropic 两年内 7 版、v2.1 加国家级行为体、v3.x 细化新型武器阈值；OpenAI v2 新增自我改进跟踪；持续披露操作化（deploymentsafety.openai.com 持续更新 GPT-5.x 分级状态）。
- **弱化侧**：EA Forum 批评（2025，中可信度）指 Anthropic 阈值表述被软化、"quietly backpedalling"；PF v2 把 CBRN 收窄为"生＋化"两域；xAI/Mistral 干脆无框架。

## 三、生物档位触及事件史

| 时点 | 事件 | 性质 |
|---|---|---|
| 2025-04-16 | o3/o4-mini 系统卡：未达 High，但模型"on the cusp of being able to meaningfully help novices create known biological threats"（濒临显著帮助新手） | 首个"濒临"公开表述 |
| 2025-05-22 | **Anthropic 首次启用 ASL-3**：因 Claude Opus 4 的 CBRN 能力提升，"a precautionary and provisional action"（预防性、临时）；部署措施初期专注生物武器 | ASL 生物档首次动用 |
| 2025-07-10 | ChatGPT Agent 成为 OpenAI 首个被"按 High 处理"的生化能力模型（Transformer 报道，中） | 预防性行政分级 |
| 2025-08-07 | GPT-5 系统卡："we have decided to treat gpt-5-thinking as High capability in the Biological and Chemical domain"（一手） | 预防性归类，非实测越线 |
| 2025-11-18 | Gemini 3 Pro 首份 FSF 评估报告：生物与化学安全域"未发现达到该门槛的证据"（一手） | 明确未达 |
| 2026 年 | GPT-5.5/5.6 延续"treated as High…below Critical"（deploymentsafety.openai.com） | 常态化 |
| 2026-08-07 | Anthropic 发布"Improving Fable 5's biology safeguards"（标题经官网新闻列表核实，内容待读） | 部署后加固 |
| 2026-09-10 | **Anthropic 威胁情报报告**（覆盖 2025-12~2026-08）：披露阻断多起生物滥用图谋；NYT 报道其承认"could not always determine whether the research was legitimate or nefarious"（NYT/BBC，高可信度） | 首个公开的部署后滥用尝试数据流 |

**对照锚点（本仓库时间线）**：PF 的 Critical 档已被网络域**实触及**（GPT-6 Astra，2026-09-03，见 [watch/capability 第二期](../watch/capability/2026-09-09-ai-timeline-watch.md)）——生物域目前最高到"预防性按 High 处理"，**尚无任何实验室披露实测越过生物 Critical/ASL-4**。这条"网络先行、生物悬置"的错位是 CHK 设计的直接素材。

三条结构性观察：

1. **"预防性按 High 处理"成为常态**：实验室用行政分级替代评估裁决——好处是保守，代价是阈值信号退化（"按 High 处理"不再携带"测到了"的信息量）。
2. **触及披露全部自评**：独立预发布评估 2026 年才出现（SecureBio 对 GPT-5.5，2026-04，见 01 §三），覆盖一家、一次。
3. **威胁情报报告开创"滥用尝试"披露流**：这是未来观察"需求侧"（谁在试图用）的唯一天然数据源，值得按期跟踪。

## 四、其他实验室与官方评估机构

- **Meta**：2024-11-04 宣布 Llama 向美国政府/国防承包商开放（NYT/Guardian，高）；Llama 4 现行 AUP 仍禁止"Biological weapons synthesis or creation of bioweapons"（一手 developer.meta.com；与部分媒体"解除生化/军事禁令"说法**相左，并列存疑**，"删除"版本是否曾存在未能核实）。另有非阈值型 Frontier AI Framework（v1.1，含 High/Critical 风险类目）。
- **Microsoft**：Frontier Governance Framework（2025-02 首发，2026-02 更新），采用相对"marginal capability uplift"增量法；2025-05 声明"no novel high-impact capability identified"。
- **xAI / Mistral**：无已发布安全框架；Grok 4（2025-07）发布时缺系统卡文档遭批评（SecureBio/METR 综述，中）。
- **美国官方**：NIST AISI 于 2025-06 被商务部长 Lutnick 改组更名 **CAISI**（Center for AI Standards and Innovation，去掉"Safety"——Tech Policy Press 评论称非仅措辞变化，治理方向信号）。CAISI 与英国机构对 OpenAI 模型做过联合 pre-deployment 测试；o3/o4-mini 发布前获美 AISI（cyber/bio）＋英 AISI（cyber/chem/bio/autonomy）早期访问测试（一手系统卡）。**早期访问测试已成惯例**。
- **英国官方**：AISI→AISA（2025-02，转国家安全取向），SIGMA 安全小组聚焦 CBRN/网络（公告原文未能直核，中可信度）；《Frontier AI Trends Report》（2025-12）汇总 30+ 模型评测。
- **边缘变量**：五角大楼与 Anthropic 冲突（2026-01 起，FASCSA"供应链风险"认定→2026-03 初步禁令→2026-04 上诉被驳回，涉监控/自主武器而非生物，事件仍在演变）——不改变生物阈值事实，但影响"实验室-政府"信任结构与信息披露意愿。

## 五、方法论批评（与 01 §四 互链）

- **自评困境**：评估者与被评者利益一致；Gary Marcus 批 OpenAI 统计分析有误/样本不足（中）；SecureBio 自己也注明 uplift 研究统计方法受批评（专家 6.00→6.88/10 无显著性）。
- **Epoch AI（2025-06）**：各实验室生物评测透明度差、阈值含义不明、基准高分与武器化风险的映射未建立。
- **跨框架不可比**：三家用不同基线（公开信息基线/资源分层/低资源行为体）与不同门槛（100+ deaths/mass casualties/无量化）——**本库只做同实验室时间序列比较，不做跨实验室横比**。

## 六、对预测的含义（喂给 [05](05-forecasts.md)）

- **CHK 素材**：ASL-4 或 PF 生物 Critical 的首次实测披露＝重大信号；"预防性按 High 处理"的扩散范围；独立预发布评估是否从一家一次扩为惯例；威胁情报报告披露的滥用图谋数量趋势。
- **口径警示**：框架阈值是"实验室自设"信号，不等于客观风险——预测条目应绑定**披露事件**（可第三方核验）而非"真实能力"（不可核验）。这直接决定 ledger 清算标准的写法。

## 数据可信度总注

实验室官网政策文档/系统卡为一手（高）；Frontier Model Forum 汇编（2025-05-12）为行业级二手（中-高）；NYT/BBC/FedScoop 为高；Transformer/EA Forum/governance.ai/Zvi 为中。**未能核实项**：Anthropic 独立"customer screening"专项公告原文（仅见 RSP 尽调条款）；OpenAI"raised the bar"原句（博文标题已核实）；UK SIGMA 公告原文；Meta"删除生化禁令"报道的原始版本；Anthropic 2026-08-07 Fable 5 文帖正文（标题已核实，待读）。

## 来源

- https://www.anthropic.com/responsible-scaling-policy ；https://www.anthropic.com/news/activating-asl3-protections ；https://www.anthropic.com/aup ；https://www.anthropic.com/news/enterprise-frontier-safeguards ；https://www.anthropic.com/threat-intelligence-report-september-2026 （均一手）
- https://www.frontiermodelforum.org/issue-briefs/frontier-ai-biosafety-thresholds/ （阈值措辞汇编，2025-05-12）
- https://cdn.openai.com/pdf/18a02b5d-6b67-4cec-ab64-68cdfbddebcd/preparedness-framework-v2.pdf ；https://cdn.openai.com/pdf/2221c875-02dc-4789-800b-e7758f3722c1/o3-and-o4-mini-system-card.pdf ；https://openai.com/index/gpt-5-system-card/ ；https://deploymentsafety.openai.com/gpt-5-6/cybersecurity-capabilities （均一手）
- https://openai.com/index/a-practical-approach-to-building-safer-more-advanced-ai/ （2024-12-20 博文，一手）
- https://deepmind.google/frontier-safety/ ；https://deepmind.google/blog/strengthening-our-frontier-safety-framework/ ；https://storage.googleapis.com/deepmind-media/gemini/gemini_3_pro_fsf_report.pdf （一手，2025-11-18）
- https://www.about.fb.com/news/2024/11/open-source-ai-america-global-security/ ；https://developer.meta.com/ai/llama4/use-policy/ （一手）
- https://www.commerce.gov/news/press-releases/2025/06/statement-us-secretary-commerce-howard-lutnick-transforming-us-ai （一手）；https://www.nist.gov/caisi ；https://www.aisi.gov.uk/
- https://fedscoop.com/trump-administration-rebrands-ai-safety-institute-aisi-caisi/ （高）；https://www.nytimes.com/2026/09/10/us/politics/anthropic-ai-biological-weapons.html ；https://www.bbc.com/news/articles/cx2zrrpkx20o （高）
- https://epoch.ai/gradient-updates/do-the-biorisk-evaluations-of-ai-labs-actually-measure-the-risk-of-developing-bioweapons （中，2025-06）
- https://forum.effectivealtruism.org/posts/kMpf7nYRpTkGh2Qfa/anthropic-is-quietly-backpedalling-on-its-safety-commitments ；https://www.governance.ai/analysis/anthropics-rsp-v3-0-how-it-works-whats-changed-and-some-reflections ；https://thezvi.wordpress.com/2025/05/02/openai-preparedness-framework-2-0/ ；https://www.transformernews.ai/p/openai-hits-the-biorisk-alarm-chatgpt-agent ；https://securebio.org/benchmarks/models/ （中）
- https://en.wikipedia.org/wiki/Anthropic%E2%80%93United_States_Department_of_Defense_dispute （中，演变中）
