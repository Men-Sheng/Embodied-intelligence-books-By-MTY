# 36 Game-Changing Claude Prompts for eBook Publishing
# 面向电子书出版的 36 条颠覆性 Claude 提示词

**英汉对照学习版 / Bilingual study edition (EN–ZH)**

- 原作者 / 出处：Tommi Pedruzzi — Nespola.io × PublishingOS
- 原结构：A Three-Hour Lecture in Ten Modules（三小时讲座 · 十个模块 · Prompt 1–36）
- 版式：每段先英文原文，紧接中文翻译
- 用途声明：本对照版仅供个人学习研究使用，请勿传播、公开或商用；版权属原作者 Nespola.io 所有
- 制作说明：原文取自作者免费发放的 PDF 版面。个别段落在源文件中存在重影/串行，已用文本层交叉核对复原；确实无法复原之处在文中标注 [原文残缺]

---

## 目录 / Table of Contents

| Module 模块 | Title 标题 | Prompts 提示词编号 |
|---|---|---|
| I | First Principles 第一性原理 | — |
| II | Market Intelligence 市场情报 | 1–5 |
| III | The GTS Engine GTS 引擎（概念—大纲—测试） | 6–9 |
| IV | The Production Line 生产线 | 10–16 |
| V | Visual Identity 视觉识别 | 17–19 |
| VI | The Storefront 店面（商品页） | 20–24 |
| VII | Launch Operations 上市运营 | 25–27 |
| VIII | The Advertising Engine 广告投放引擎 | 28–31 |
| IX | Scale Architecture 规模化架构 | 32–34 |
| X | The Content Flywheel 内容飞轮 | 35–36 |
| Closing | Synthesis & Implementation Roadmap 综合与落地路线图 | — |

---

# MODULE I — First Principles
# 模块一 — 第一性原理

**The AI-Augmented Publisher and the New Economics of Prompt-Driven Production**
AI 增强型出版者，以及提示词驱动生产的新经济学

*Estimated Duration: 20 minutes — 预计时长：20 分钟*

## 1.1 — Opening Provocation
## 1.1 — 开场的一记棒喝

The traditional self-publishing workflow requires competence across at least twelve distinct disciplines: market research, keyword analysis, competitive intelligence, content strategy, manuscript creation, developmental editing, cover design, interior formatting, listing copywriting, launch management, advertising operations, and portfolio analytics. Mastering even three of these disciplines takes years. Mastering all twelve is, for a solo operator, effectively impossible.

传统自费出版流程要求你至少在十二个互不相同的学科上具备胜任能力：市场调研、关键词分析、竞品情报、内容策略、书稿创作、发展性编辑、封面设计、内文排版、商品页文案、上市管理、广告投放运营、以及作品集数据分析。其中任意三个学科，光是精通就要花上好几年。而要把十二个全部精通，对一个人单干的操盘者来说，实际上是不可能的。

The AI-augmented publisher does not need to master these twelve disciplines. They need to master one meta-skill: the ability to instruct an AI system with sufficient precision that it performs each discipline at a professional level. That meta-skill is prompt engineering. The collection of prompts that covers the entire publishing workflow is, in effect, your operating system.

AI 增强型出版者并不需要精通这十二个学科。他需要精通的是一项**元技能**：以足够精确的方式指挥一个 AI 系统，让它在每个学科上都达到专业水准的产出。这项元技能就是提示词工程。而一套能够覆盖整条出版流程的提示词集合，本质上就是你的操作系统。

That is what PublishingOS means. It is not a metaphor. It is a literal description of what we are building today.

这就是 PublishingOS（出版操作系统）这个名字的含义。它不是修辞比喻，而是对我们今天在做的东西的字面描述。

## 1.2 — Why Claude, and Why Now
## 1.2 — 为什么是 Claude，为什么是现在

Three structural shifts have converged to make this lecture possible in 2026 and not before.

三股结构性变化汇流到了一起，才让这场讲座在 2026 年成为可能——早一年都不行。

**First, context window expansion.** Claude can now process and reason across extremely large documents — full manuscripts, competitive landscapes, entire keyword databases — in a single session.

**第一，上下文窗口的扩张。** Claude 如今已经能在单次会话中处理并对超长文档进行推理——整本稿件、整个竞争格局、乃至完整的关键词数据库。

**Second, tool integration.** Claude connects directly to Notion, Google Drive, Slack, and Gmail. The prompt becomes a trigger, not a container.

**第二，工具整合。** Claude 可以直接连上 Notion、Google Drive、Slack 和 Gmail。于是提示词变成了一个"触发器"，而不是一个"容器"。

**Third, reasoning depth.** A precise prompt, structured with the right constraints, context, and output format, produces work that would cost you five hundred to two thousand dollars if outsourced to a human specialist.

**第三，推理深度。** 一条精确的提示词，配上恰当的约束、上下文和输出格式，其产出质量相当于你花五百到两千美元外包给人类专家才能得到的成果。

## 1.3 — The Prompt Architecture Framework
## 1.3 — 提示词架构框架

Every effective prompt in this library follows a five-part architecture:

本库中每一条行之有效的提示词，都遵循一个五段式架构：

**PART 1 — Role Assignment.** Tell Claude who it is — specifically. "You are a senior Amazon KDP market analyst with ten years of experience" produces fundamentally different output than "help me find a book topic."

**第 1 部分 — 角色指派。** 明确告诉 Claude 它是谁，而且要具体。"你是一位有十年经验的亚马逊 KDP 资深市场分析师"，与"帮我找个书的选题"，两者产出的东西根本不在一个层次上。

**PART 2 — Context Injection.** Provide the raw material Claude needs: a keyword list, a competitive landscape, a manuscript draft, or a set of performance metrics. The more specific the context, the more precise the output.

**第 2 部分 — 上下文注入。** 把 Claude 需要的原材料喂给它：一份关键词清单、一个竞品格局、一版稿件草稿，或者一组表现数据。上下文越具体，输出越精准。

**PART 3 — Task Specification.** Define exactly what you want. Not "analyse this" but "produce a ranked list of the top five keyword opportunities, scored on a ten-point scale across four criteria."

**第 3 部分 — 任务规定。** 把你到底要什么写死。不要写"分析一下这个"，而要写"给出排名前五的关键词机会清单，按四项标准各打十分制分数并排序"。

**PART 4 — Constraint Setting.** Define the boundaries: word count limits, formatting requirements, tone of voice, things to avoid. Constraints are not limitations — they are precision tools.

**第 4 部分 — 约束设定。** 把边界划出来：字数上限、格式要求、语气风格、以及哪些不要碰。约束不是限制，约束是精修工具。

**PART 5 — Output Format.** Specify exactly how the deliverable should be structured. Tables, bullet points, numbered sections, markdown — define the shape of the answer before Claude begins producing it.

**第 5 部分 — 输出格式。** 明确交付物该长成什么结构。表格、要点、编号小节、markdown——在 Claude 开始动手之前，先把答案的形状定下来。

## 1.4 — How to Use This Library
## 1.4 — 如何使用本库

Each prompt is presented in a consistent structure: strategic purpose, the prompt itself (formatted for immediate copy-and-paste use), key variables to customise, and expected output quality standards.

每一条提示词都按统一结构呈现：战略目的、提示词正文（已排成可直接复制粘贴使用的格式）、需要自定义的关键变量、以及预期的输出质量标准。

Treat this library as a sequential system, not a collection of individual prompts. Start at Prompt One and work through to Prompt Thirty-Six for your first book. The library is designed to support both linear execution and modular reuse.

请把本库当成一套**顺序执行的系统**来用，而不是一堆彼此独立的提示词合集。做第一本书时，从 Prompt 1 一路做到 Prompt 36。整个库的设计同时支持"线性跑完"和"模块化取用"两种用法。

---

# MODULE II — Market Intelligence（Prompts 1–5）
# 模块二 — 市场情报（提示词 1–5）

**Niche Discovery, Keyword Analysis, and Competitive Validation**
利基发现、关键词分析与竞品验证

*Estimated Duration: 20 minutes — 预计时长：20 分钟*

The single most consequential decision in the entire publishing workflow is niche selection. Get it right and a mediocre book in a hungry market will generate consistent income. Get it wrong and a masterpiece in a dead market will earn nothing. The five prompts in this module replace what used to require three to five days of manual research with a structured, two-to-three-hour process that produces higher-quality intelligence.

整条出版流程里影响最大的一个决定，就是利基（细分市场）选择。选对了，一本平庸的书放在一个饥渴的市场里也能带来稳定收入；选错了，一部杰作扔进一个死掉的市场里也赚不到一分钱。本模块这五条提示词，把过去需要三到五天人工调研的工作，换成一套结构化的、两到三小时就能跑完的流程——而且产出的情报质量更高。

## PROMPT 1 — The Niche Discovery Engine
## 提示词 1 — 利基发现引擎

**Strategic Purpose:** Generate a prioritised list of profitable niche opportunities in a given category, filtered through the PublishingOS selection criteria.

**战略目的：** 在给定大类下，生成一份按优先级排列的高利润利基机会清单，并且已经用 PublishingOS 的筛选标准过了一遍。

**THE PROMPT / 提示词正文**

> You are a senior Amazon KDP market analyst specialising in non-fiction niche selection. You have 10 years of experience identifying underserved markets with strong buyer intent.
>
> I am exploring the `[BROAD CATEGORY]` space on Amazon KDP. I want to find 10–15 specific sub-niche keyword opportunities that meet ALL of the following criteria:
>
> - Evergreen demand — consistent year-round search interest, not seasonal or trend-dependent
> - Paperback non-fiction focus — the niche must support physical book formats at $14.99–$19.99 price points
> - Net margin of $5+ per copy after Amazon's printing costs and 60% royalty
> - Moderate competition — ideally fewer than 3,000 search results on Amazon for the primary keyword
> - Buyer intent — the keyword suggests the searcher wants a solution, not just information
> - Brand scalability — the niche can support 3–5 related titles, not just a single book
>
> For each opportunity, provide: the specific keyword phrase, why it meets the criteria, a confidence score from 1–10, and one related keyword that could become a companion book. Format the output as a numbered list sorted by confidence score. After the list, provide a 3-paragraph strategic summary explaining which 3 niches you would prioritise and why.

> 你是一位专注于非虚构类利基选择的亚马逊 KDP 资深市场分析师，有 10 年识别"供给不足但购买意图强烈"市场的经验。
>
> 我正在探索亚马逊 KDP 上的 `[BROAD CATEGORY]`（大类）领域。我要找出 10–15 个具体的**子利基关键词机会**，它们必须**同时**满足以下全部条件：
>
> - 常青需求 —— 全年搜索量稳定，不是季节性或靠热点撑起来的
> - 以平装非虚构为主 —— 这个利基必须撑得起纸质书形态，定价在 $14.99–$19.99
> - 扣除亚马逊印刷成本和 60% 版税之后，每本净毛利 ≥ $5
> - 竞争中等 —— 主关键词在亚马逊上的搜索结果最好在 3,000 条以内
> - 购买意图 —— 这个关键词说明搜索者想要的是一个"解决方案"，而不只是信息
> - 品牌可延展 —— 这个利基能支撑 3–5 本相关书目，而不是只能出一本
>
> 对每个机会，请给出：具体的关键词短语、它为什么满足上述条件、1–10 的置信度评分、以及一个可以做成配套书的相关关键词。输出格式为按置信度排序的编号清单。清单之后，再给一段 3 段的战略小结，说明你会优先做哪 3 个利基、为什么。

**Key Variables to Customise:** Replace `[BROAD CATEGORY]` with your target space. Adjust price points if targeting a different format. Add geographic market constraints if needed.

**需要自定义的关键变量：** 把 `[BROAD CATEGORY]` 换成你目标的大类领域。如果你做的是别的形态（精装/电子书），把价格档位相应调整。必要时补充地域市场限制。

**Expected Output:** A ranked list of ten to fifteen keyword opportunities with justifications, confidence scores, and a strategic recommendation. The output should read like a market research memo from a publishing consultancy.

**预期输出：** 一份 10 到 15 条关键词机会的排名清单，带论证理由、置信度评分和一个战略性建议。这份输出应该读起来像一家出版咨询公司出的市场调研备忘录。

## PROMPT 2 — The Keyword Deep-Dive Analyser
## 提示词 2 — 关键词深挖分析器

**Strategic Purpose:** Take a promising keyword from Prompt 1 and perform a detailed competitive and revenue analysis using data gathered from Amazon and your research tools (BookBeam, Publisher Rocket, KDP Champ).

**战略目的：** 从 Prompt 1 的结果里挑一个有前景的关键词，用你从亚马逊和调研工具（BookBeam、Publisher Rocket、KDP Champ）抓来的数据，做一次细致的竞争与营收分析。

> 〔注：源文件此处工具名被页面裁切，仅可辨认为 BookBeam / Publisher Rocket / …Champ，其余工具名以 [?] 处理。〕

**THE PROMPT / 提示词正文**

> You are an Amazon KDP competitive intelligence analyst. I am evaluating the keyword `[KEYWORD]` for a potential book publication. Below is the data I have collected from Amazon and my research tools.
>
> `[DATA]`
>
> Based on this data, produce a comprehensive keyword analysis report covering:
>
> - **Demand Assessment:** Estimate daily and monthly sales volume based on BSR data. Categorise demand as Strong (BSR < 50K), Moderate (50K–150K), or Weak (> 150K).
> - **Competition Assessment:** Evaluate the quality of existing competition. Rate competition intensity as Low, Medium, or High with specific evidence.
> - **Revenue Projection:** Based on a paperback at $`[PRICE]`, project monthly revenue at conservative (2 copies/day), moderate (4 copies/day), and optimistic (7 copies/day) sales rates.
> - **Differentiation Opportunities:** Identify 3 specific ways our book could outperform the current market.
> - **Risk Factors:** Identify any red flags — dominant publishers, trademark issues, declining search trends, or format saturation.
> - **Final Recommendation:** GO, CONDITIONAL GO, or NO GO. Justify in 2–3 sentences.
>
> Format with clear headers and bullet points. Include a summary table at the top with key metrics.

> 你是一位亚马逊 KDP 竞品情报分析师。我正在评估关键词 `[KEYWORD]` 是否值得为它出一本书。下面是我从亚马逊和自己的调研工具收集到的数据。
>
> `[DATA]`（数据）
>
> 请基于这些数据，产出一份完整的关键词分析报告，涵盖：
>
> - **需求评估：** 根据 BSR（畅销榜排名）数据估算日销量和月销量。把需求分为 Strong 强（BSR < 5 万）、Moderate 中（5 万–15 万）、Weak 弱（> 15 万）。
> - **竞争评估：** 评价现有竞品的质量。把竞争烈度评为 Low / Medium / High，并给出具体证据。
> - **营收预测：** 按平装书定价 $`[PRICE]` 计算，分别预测保守（2 本/天）、中等（4 本/天）、乐观（7 本/天）三档销量下的月收入。
> - **差异化机会：** 找出 3 个具体方式，让我们的书能打赢当前市场上的竞品。
> - **风险因素：** 指出任何红旗信号 —— 头部出版社垄断、商标问题、搜索趋势下行、或者形态饱和。
> - **最终建议：** GO（做）、CONDITIONAL GO（有条件做）、或 NO GO（不做）。用 2–3 句话给出理由。
>
> 用清晰的小标题和要点排版。在最上方放一个包含关键指标的数据总表。

**Key Variables to Customise:** Target keyword, price point, raw data from research tools.

**需要自定义的关键变量：** 目标关键词、定价档位、从调研工具导出的原始数据。

**Expected Output:** A structured intelligence report that gives you a clear go/no-go decision with the reasoning transparent enough to audit.

**预期输出：** 一份结构化的情报报告，给你一个明确的"做/不做"结论，且推理过程透明到可以被复盘审计。

## PROMPT 3 — The Trend Validator
## 提示词 3 — 趋势验证器

**Strategic Purpose:** Cross-reference a keyword against search patterns to confirm evergreen viability.

**战略目的：** 把一个关键词拿去和搜索曲线交叉比对，确认它是不是真的"常青"。

**THE PROMPT / 提示词正文**

> You are a market trends analyst specialising in consumer publishing behaviour. I am considering publishing a book targeting the keyword `[KEYWORD]`.
>
> Search the web for current data on this topic's search trends, seasonal patterns, and market trajectory. I need:
>
> - Is search interest for this topic stable year-round, or does it spike seasonally? If seasonal, which months peak and which are dead?
> - Is the overall trend growing, stable, or declining over the past 3 years?
> - Are there any current events or cultural shifts temporarily inflating interest? Will that interest persist?
> - Are there adjacent or emerging sub-topics that signal where demand is heading next?
>
> Based on your findings, classify this keyword as: ✅ EVERGREEN, ⚠️ SEASONAL, or 🔴 TREND-DEPENDENT. Provide a 1-page summary with specific data points, not general observations.

> 你是一位专注于消费者出版行为的市场趋势分析师。我在考虑出一本针对关键词 `[KEYWORD]` 的书。
>
> 请联网搜索这个主题当前的搜索趋势、季节性规律和市场走向数据。我需要知道：
>
> - 这个主题的搜索热度是全年稳定，还是季节性冲高？如果是季节性的，哪几个月是峰值、哪几个月是死期？
> - 过去 3 年，整体趋势是在涨、持平、还是在跌？
> - 有没有什么当下事件或文化风向在**暂时性**地抬高热度？这股热度会不会持续？
> - 有没有相邻的或正在冒头的子话题，能提示需求下一步往哪走？
>
> 根据你的发现，把这个关键词归类为：✅ 常青（EVERGREEN）、⚠️ 季节性（SEASONAL）、或 🔴 依赖热点（TREND-DEPENDENT）。给出一页纸的总结，要**具体数据点**，不要泛泛而谈。

**Expected Output:** A data-backed trend classification with specific evidence. Claude will use web search to pull current information — real-time market intelligence, not stale training data.

**预期输出：** 一个有数据支撑、带具体证据的趋势分类结论。Claude 会用联网搜索去拉取当下信息 —— 是实时市场情报，不是过时的训练数据。

## PROMPT 4 — The Competitor Teardown
## 提示词 4 — 竞品拆解

**Strategic Purpose:** Perform a deep-dive analysis of the top-performing book in the target niche to understand what is working and where opportunities exist.

**战略目的：** 对目标利基里卖得最好的那本书做一次深潜式拆解，搞清楚什么在起作用、机会缺口在哪里。

**THE PROMPT / 提示词正文**

> You are a competitive intelligence analyst for a publishing company. I want a detailed teardown of this competing book in my target niche:
>
> Title: `[COMPETITOR TITLE]` · Author/Publisher: `[NAME]` · ASIN: `[ASIN]` · Price: $`[PRICE]` · BSR: `[BSR]` · Reviews: `[NUMBER]` (avg: `[RATING]`) · Page count: `[PAGES]`
>
> Analyse the following:
>
> - **Listing Quality:** Rate the title, subtitle, description, and backend keyword strategy from 1–10. What are they doing well? What are they missing?
> - **Cover Analysis:** Rate it for genre compliance, thumbnail readability, professional quality, and emotional resonance. Score each 1–10.
> - **Content Strategy:** Based on the table of contents and/or Look Inside preview, evaluate depth, structure, and unique value proposition.
> - **Review Sentiment Mining:** Summarise key themes from positive reviews (what readers love) and negative reviews (what readers wish was different). These reader complaints are your product development roadmap.
> - **Advertising Signals:** Is this book likely running Amazon Ads? Estimate their ad strategy.
> - **Vulnerabilities:** List 3–5 specific weaknesses we can exploit with our book.
>
> Output as a structured report with a 3-sentence executive summary at the top.

> 你是一家出版公司的竞品情报分析师。我要对我目标利基里的这本竞品做一次详细拆解：
>
> 书名：`[COMPETITOR TITLE]` · 作者/出版方：`[NAME]` · ASIN：`[ASIN]` · 定价：$`[PRICE]` · BSR：`[BSR]` · 评论数：`[NUMBER]`（均分：`[RATING]`）· 页数：`[PAGES]`
>
> 请分析以下几点：
>
> - **商品页质量：** 给它的书名、副书名、描述文案和后台关键词策略各打 1–10 分。它哪里做得好？哪里漏了？
> - **封面分析：** 从"是否符合品类惯例、缩略图下是否清晰、专业度、情绪感染力"四个维度打分，各 1–10。
> - **内容策略：** 根据目录和/或"免费试读"预览，评估它的深度、结构和独特价值主张。
> - **评论情绪挖掘：** 分别总结好评（读者喜欢什么）和差评（读者希望它哪里不一样）的关键主题。**这些读者的抱怨，就是你的产品开发路线图。**
> - **广告投放信号：** 这本书大概率在投亚马逊广告吗？估算它的投放策略。
> - **薄弱环节：** 列出 3–5 个我们的书可以打的、具体的弱点。
>
> 输出一份结构化报告，最上方放一段 3 句话的执行摘要。

> 〔注：源文件此页底部的 Key Variables / Expected Output 落在重影带上，无法完整辨认。〕

## PROMPT 5 — The Niche Scorecard
## 提示词 5 — 利基记分卡

**Strategic Purpose:** Consolidate all research into a single decision-making framework — the final filter before committing to a niche.

**战略目的：** 把前面所有调研结果汇总进**一个**决策框架 —— 这是在押注某个利基之前的最后一道过滤器。

**THE PROMPT / 提示词正文**

> You are the Chief Strategy Officer of a digital publishing company. Based on the following research I have conducted for the keyword `[KEYWORD]`, produce a final Niche Scorecard.
>
> `[DATA]`
>
> Score the niche on each of the following criteria using a 1–10 scale:
>
> - Market Demand (search volume, BSR data, trend stability)
> - Competition Quality (how beatable are the current top 5 titles?)
> - Revenue Potential (net margin × realistic daily sales volume)
> - Differentiation Opportunity (can we be meaningfully better?)
> - Brand Scalability (can this become 3–5 books, not just one?)
> - International Potential (demand in UK, DE, FR, ES, IT, AU markets)
> - Advertising Viability (will Amazon Ads work profitably here?)
> - Production Feasibility (can we produce this book within 30 days?)
>
> Calculate a weighted total score where Market Demand and Revenue Potential are weighted 2x. Provide the total as X/100. Then provide: FINAL VERDICT (PUBLISH / CONDITIONAL / PASS), conditions if CONDITIONAL, and a 3-sentence rationale. Format as a clean scorecard table followed by the verdict section.

> 你是一家数字出版公司的首席战略官。基于我针对关键词 `[KEYWORD]` 所做的以下调研，请产出一份最终的"利基记分卡"。
>
> `[DATA]`（数据）
>
> 请用 1–10 分制，对这个利基在以下每一项标准上打分：
>
> - 市场需求（搜索量、BSR 数据、趋势稳定性）
> - 竞争质量（目前排名前五的书有多容易被打败？）
> - 营收潜力（单本净毛利 × 现实可行的日销量）
> - 差异化机会（我们能不能做出**实质性**的更好？）
> - 品牌延展性（这个能不能做成 3–5 本书，而不只是一本？）
> - 国际化潜力（在英国、德国、法国、西班牙、意大利、澳洲市场的需求）
> - 广告可行性（在这里投亚马逊广告能赚钱吗？）
> - 生产可行性（我们能在 30 天内把这本书做出来吗？）
>
> 计算一个加权总分，其中"市场需求"和"营收潜力"按 2 倍权重计。总分以 X/100 的形式给出。然后给出：最终裁定（PUBLISH 做 / CONDITIONAL 有条件做 / PASS 放弃）；若为 CONDITIONAL，列出条件；再附一段 3 句话的理由。排版为一张干净的记分卡表格，后接裁定部分。

---

# MODULE III — The GTS Engine（Prompts 6–9）
# 模块三 — GTS 引擎（提示词 6–9）

**Guided Topic Selection, Positioning, and Dream Reader Definition**
引导式选题、定位，与"梦想读者"定义

*Estimated Duration: 20 minutes — 预计时长：20 分钟*

You have now validated a niche. The research confirms demand, manageable competition, and viable unit economics. The next phase is the most creatively demanding: transforming a validated keyword into a specific book concept with a clear positioning, target reader, and strategic angle. This is where most publishers fail. They find a good niche and then produce a generic book. The prompts in this module force strategic specificity.

你现在已经验证了一个利基。调研确认了它的需求存在、竞争可控、单本经济模型可行。下一个阶段是整条流程里最吃创造力的：把一个已验证的关键词，转化成一个**具体的书的概念** —— 有清晰的定位、目标读者和战略切入角度。大多数出版者就是在这里翻车的：他们找到了一个好利基，然后做出一本毫无特色的书。本模块的提示词，就是用来逼出战略上的具体性。

## PROMPT 6 — The Dream Reader Persona
## 提示词 6 — 梦想读者画像

**Strategic Purpose:** Define the exact person who will buy your book — their pain points, desires, language, and purchase triggers.

**战略目的：** 把那个会真正掏钱买你书的人定义清楚 —— 他的痛点、他的渴望、他嘴里说的话、以及触发他下单的东西。

**THE PROMPT / 提示词正文**

> You are a consumer psychologist specialising in book-buying behaviour on Amazon. I am publishing a book in the `[NICHE/KEYWORD]` space.
>
> Create a detailed Dream Reader Persona covering:
>
> - **Demographics:** Age range, gender distribution, income level, education, occupation
> - **The Core Problem:** What specific pain, frustration, or gap is driving them to search for this book? Be precise — not "they want to be healthier" but "they have tried 3 diets in the past year and failed each time by week 4."
> - **The Desired Transformation:** What does success look like to them in 90 days? In 1 year?
> - **Language Patterns:** Exact phrases and vocabulary they would use to describe their problem. These are the words that must appear in your title, description, and content.
> - **Purchase Triggers:** What specific elements in a book description or cover would make them click "Buy Now" without hesitation?
> - **Anti-Persona:** Briefly describe who this book is NOT for — this helps sharpen positioning.
>
> Write this as a vivid, one-page profile I can pin to my wall and reference throughout the entire publishing process.

> 你是一位研究"亚马逊上买书行为"的消费者心理学家。我要在 `[NICHE/KEYWORD]` 这个领域出一本书。
>
> 请创建一份详细的"梦想读者画像"，涵盖：
>
> - **人口特征：** 年龄段、性别分布、收入水平、教育程度、职业
> - **核心问题：** 到底是什么具体的痛、具体的挫败、具体的缺口，在驱使他们搜索这本书？要精确 —— 不要写"他们想更健康"，而要写"他们在过去一年里试过 3 种节食法，每一次都在第 4 周失败"。
> - **渴望的转变：** 对他们来说，90 天后"成功"长什么样？1 年后呢？
> - **语言模式：** 他们描述自己这个问题时，会用的**确切短语和词汇**。这些词必须出现在你的书名、描述文案和正文里。
> - **购买触发点：** 书的描述或封面里，哪些具体元素会让他们毫不犹豫地点下"立即购买"？
> - **反面画像（Anti-Persona）：** 简要说明这本书**不是**写给谁的 —— 这能让定位更锋利。
>
> 请把它写成一页纸、有画面感的画像，让我能贴在墙上，在整个出版流程里随时对照。

## PROMPT 7 — The Positioning Statement
## 提示词 7 — 定位声明

**Strategic Purpose:** Define how your book will be different from — and better than — everything currently on the market.

**战略目的：** 说清楚你的书如何区别于——并且优于——市面上已有的所有同类书。

**THE PROMPT / 提示词正文**

> You are a brand strategist who specialises in positioning products in crowded markets. I am publishing a book targeting the keyword `[KEYWORD]` on Amazon KDP.
>
> Here are the top 5 competing titles currently ranking for this keyword: `[LIST: Title, author, price, review count, key strengths/weaknesses from Prompt 4]`
>
> And here is my Dream Reader Persona: `[PASTE output from Prompt 6]`
>
> Based on this competitive landscape and reader profile, generate:
>
> - **Positioning Statement:** "This is the only `[NICHE]` book that `[UNIQUE DIFFERENTIATOR]` for `[SPECIFIC AUDIENCE]`."
> - **Positioning Angles:** Three distinct strategic angles — each represent a different way to stand out, with trade-offs and which segment each best serves.
> - **Recommended Angle:** Which of the three you would choose and why.
> - **Book Promise:** A one-sentence promise the reader can hold you to — what they will be able to do after reading it that they cannot do now.
> - **Title + Subtitle Candidates:** 5 title/subtitle combinations that are keyword-rich for Amazon AND emotionally compelling for human readers.

> 你是一位品牌战略师，专长是在拥挤的市场里给产品做定位。我要在亚马逊 KDP 上出一本针对关键词 `[KEYWORD]` 的书。
>
> 下面是当前在这个关键词下排名前五的竞品书：`[清单：书名、作者、价格、评论数、来自 Prompt 4 的关键优劣势]`
>
> 然后这是我的梦想读者画像：`[粘贴 Prompt 6 的输出]`
>
> 基于这份竞争格局和读者画像，请生成：
>
> - **定位声明：** "这是唯一一本为 `[特定人群]` 提供 `[独特差异点]` 的 `[利基]` 书。"
> - **三个定位角度：** 三个彼此不同的战略角度 —— 每个代表一种不同的"站出来"的方式，写清各自的取舍，以及分别最适配哪个人群细分。
> - **推荐角度：** 三个里你会选哪个，以及为什么。
> - **本书承诺：** 一句读者可以拿来"追责"你的承诺 —— 读完之后，他们能做到哪一件现在做不到的事。
> - **书名 + 副书名候选：** 5 组书名/副书名组合，既要对亚马逊的关键词友好，又要对真人读者有情绪上的吸引力。

## PROMPT 8 — The Chapter Outline Architect
## 提示词 8 — 章节大纲架构师

**Strategic Purpose:** Generate a detailed, strategically sequenced chapter outline that serves both the reader's journey and Amazon's content expectations.

**战略目的：** 生成一份详细的、在顺序上有战略考量的章节大纲，同时满足读者的阅读旅程和亚马逊对内容的期待。

**THE PROMPT / 提示词正文**

> You are a developmental editor with 15 years of experience structuring non-fiction books for maximum reader satisfaction and Amazon review performance.
>
> Book specifications: Title: `[TITLE]` · Niche: `[NICHE]` · Target length: 25,000–35,000 words · Dream Reader: `[PERSONA]` · Positioning: `[STATEMENT]`
>
> Create a detailed chapter outline following these structural principles:
>
> - The book must open with a chapter that immediately validates the reader's decision to buy — address their core pain point within the first 3 pages
> - Chapters should follow a logical progression: foundational concepts → practical application → advanced strategies
> - Each chapter must include at least one actionable element (exercise, checklist, worksheet, template, or reflection prompt)
> - Include a "Quick Wins" chapter early (Chapters 2–3) that gives the reader an immediate, tangible result
> - The final chapter must create a bridge to the reader's next step (which could be another book in our portfolio)
> - Target 12–18 chapters at 1,500–2,500 words each
>
> For each chapter: chapter number and title, 2–3 sentence summary, key takeaway, actionable element, estimated word count. After the outline, explain how this structure supports 5-star reviews.

> 你是一位有 15 年经验的发展性编辑，专长是给非虚构类图书做结构，以最大化读者满意度和亚马逊评论表现。
>
> 图书规格：书名：`[TITLE]` · 利基：`[NICHE]` · 目标篇幅：25,000–35,000 词 · 梦想读者：`[PERSONA]` · 定位：`[STATEMENT]`
>
> 请按照以下结构原则，生成一份详细的章节大纲：
>
> - 开篇第一章必须立刻让读者觉得"买对了" —— 在前 3 页内命中他的核心痛点
> - 章节要遵循合乎逻辑的递进：基础概念 → 实操应用 → 进阶策略
> - 每一章必须至少包含一个可执行元素（练习、清单、工作表、模板或反思提示）
> - 在前部（第 2–3 章）安排一章"快速见效（Quick Wins）"，给读者一个即时、可触摸的成果
> - 最后一章必须为读者的下一步搭桥（这个下一步可以是我们书柜里的另一本书）
> - 目标 12–18 章，每章 1,500–2,500 词
>
> 每一章请给出：章节编号与标题、2–3 句摘要、关键收获、可执行元素、预计字数。大纲之后，再解释这个结构为什么能支撑五星评论。

## PROMPT 9 — The Content Brief Generator
## 提示词 9 — 内容简报生成器

**Strategic Purpose:** Produce a detailed creative brief that can be handed to a ghostwriter or AI writing assistant.

**战略目的：** 产出一份足够细的创意简报，可以直接交给代笔作者或 AI 写作助手。

**THE PROMPT / 提示词正文**

> You are a publishing project manager creating a content brief for a non-fiction book. This brief will be used as the master reference document throughout the writing process.
>
> Book specifications: Title: `[TITLE]` · Keyword: `[KEYWORD]` · Dream Reader: `[summary]` · Positioning: `[statement]` · Chapter Outline: `[from Prompt 8]`
>
> Create a comprehensive Content Brief covering:
>
> - **Voice & Tone Guidelines:** Reading level (grade 7–9 recommended), tone (e.g., "warm but authoritative, like a knowledgeable friend"), what to avoid
> - **Structural Standards:** Word count per chapter, paragraph length (2–4 sentences), use of subheadings (every 300–500 words), callout boxes, chapter summaries
> - **Content Requirements per Chapter:** Specific topics that MUST be covered, required examples or case studies, frameworks to reference
> - **Competitive Differentiation Notes:** 5 specific things this book must do better than what currently exists
> - **Amazon Review Optimisation:** 5 things to deliberately include that are known to trigger positive reviews
> - **Production Timeline:** A realistic day-by-day schedule for completing the manuscript in 21 days

> 你是一位出版项目经理，正在为一本非虚构书撰写内容简报。这份简报在整个写作过程中将作为**主参考文档**使用。
>
> 图书规格：书名：`[TITLE]` · 关键词：`[KEYWORD]` · 梦想读者：`[摘要]` · 定位：`[声明]` · 章节大纲：`[来自 Prompt 8]`
>
> 请创建一份全面的内容简报，涵盖：
>
> - **声音与语气规范：** 阅读难度（建议 7–9 年级水平）、语气（例如"温暖但权威，像一个懂行的朋友"）、以及哪些不要碰
> - **结构标准：** 每章字数、段落长度（2–4 句）、小标题的使用频率（每 300–500 词一个）、提示框（callout box）、章节小结
> - **每章的内容要求：** 必须覆盖的具体主题、需要给出的案例或实例、要引用的框架
> - **竞争差异化说明：** 这本书必须比现有同类做得更好 的 5 件具体事情
> - **亚马逊评论优化：** 5 个值得刻意写进去、且已知能触发好评的元素
> - **生产排期：** 一张现实的、逐日的排程表，在 21 天内完成书稿

> 〔注：源文件此条末尾的 Key Variables / Expected Output 落在重影带上，无法完整辨认。〕

---

# MODULE IV — The Production Line（Prompts 10–16）
# 模块四 — 生产线（提示词 10–16）

**AI-Assisted Book Creation, Editing, and Quality Assurance**
AI 辅助的图书创作、编辑与质量保证

*Estimated Duration: 25 minutes — 预计时长：25 分钟*

Claude AI is not your ghostwriter. It is your co-pilot. The PublishingOS model does not advocate publishing books that are entirely AI-generated — this approach carries both quality risks and potential account risks on Amazon KDP. What we advocate is an AI-augmented workflow where Claude accelerates research, drafting, structuring, and editing while the publisher provides strategic direction, domain-specific knowledge, and final quality control.

Claude 不是你的代笔人，它是你的副驾驶。PublishingOS 这套模式**不主张**出版"完全由 AI 生成"的书 —— 那种做法在亚马逊 KDP 上既带来质量风险，也带来账号风险。我们主张的是一条 AI 增强型工作流：由 Claude 加速调研、起草、结构搭建和编辑，而由出版者提供战略方向、领域专业知识和最终的质量把关。

> 〔排版说明：源文件中的填空位以下划线输入框形式呈现，本对照版统一记作 `[...]`，请按名填入。〕

## PROMPT 10 — The Chapter Drafter
## 提示词 10 — 章节起草手

**Strategic Purpose:** Generate a high-quality first draft of an individual chapter, guided by the content brief.

**战略目的：** 在内容简报的指引下，为单独一章生成高质量的初稿。

**THE PROMPT / 提示词正文**

> You are a professional non-fiction writer. I am writing Chapter `[N]`: "`[CHAPTER TITLE]`" of my book "`[BOOK TITLE]`" in the `[NICHE]` space.
>
> Context: Dream Reader: `[persona]` · Voice: `[voice]` · Chapter purpose: `[purpose]` · Key takeaway: `[takeaway]` · Actionable element: `[element]` · Target word count: `[N]` words · Previous chapter ended with: `[ending]`
>
> Write the full chapter following these rules:
>
> - Open with a hook — a story, statistic, or provocative question that makes the reader want to keep going
> - Use short paragraphs (2–4 sentences maximum)
> - Include subheadings every 300–500 words
> - Include at least one real-world example or analogy
> - Include the specified actionable element
> - Close with a 2–3 sentence bridge that naturally leads into the next chapter
> - Do NOT use AI-sounding phrases like "in today's fast-paced world", "it's important to note", "dive deep", "unlock your potential", or "game-changer"
> - Write as if you are explaining this to a smart friend over coffee — not lecturing from a podium

> 你是一位专业非虚构作者。我正在写我的书"`[BOOK TITLE]`"（属于 `[NICHE]` 领域）的第 `[N]` 章："`[CHAPTER TITLE]`"。
>
> 上下文：梦想读者：`[画像]` · 声音：`[语气]` · 本章目的：`[目的]` · 关键收获：`[收获]` · 可执行元素：`[元素]` · 目标字数：`[N]` 词 · 上一章结尾：`[结尾]`
>
> 请按以下规则写出完整一章：
>
> - 用一个钩子开场 —— 一个故事、一个数据、或一个挑衅性的问题，让读者想继续读下去
> - 段落要短（最多 2–4 句）
> - 每 300–500 词插入一个小标题
> - 至少给出一个现实世界的例子或类比
> - 包含指定的那个可执行元素
> - 用 2–3 句过渡收尾，自然地把读者带进下一章
> - **不要**使用一听就是 AI 的短语，比如"in today's fast-paced world"（在当今快节奏的世界里）、"it's important to note"（值得注意的是）、"dive deep"（深入探究）、"unlock your potential"（释放你的潜能）、"game-changer"（游戏规则改变者）
> - 写得像你在一杯咖啡的时间裡，把这件事讲给一个聪明的朋友听 —— 不是站在讲台上授课

**Key Variables to Customise:** Run this prompt once per chapter. Feed the output of each chapter back as context for the next to maintain narrative continuity.

**需要自定义的关键变量：** 这条提示词每章跑一次。把每一章的输出回灌进下一章的上下文里，以保持叙事连贯。

## PROMPT 11 — The Developmental Editor
## 提示词 11 — 发展性编辑

**Strategic Purpose:** Perform a structural and content-quality review of a completed chapter draft.

**战略目的：** 对一份已完成的书稿章节，做一次结构与内容质量的审读。

**THE PROMPT / 提示词正文**

> You are a developmental editor reviewing a chapter of a non-fiction book for commercial publication on Amazon KDP. This book targets `[NICHE/READER]` and must achieve a 4.5+ star average review rating.
>
> Here is the chapter draft: `[PASTE CHAPTER]`
>
> Evaluate the chapter on the following dimensions and score each 1–10:
>
> - Hook Quality: Does the opening grab attention within the first 3 sentences?
> - Reader Value: Will the Dream Reader feel they learned something genuinely useful?
> - Actionability: Is there at least one concrete action the reader can take immediately?
> - Flow & Structure: Do sections connect logically? Are transitions smooth?
> - Voice Consistency: Does the tone match [SPECIFIED VOICE] throughout?
> - Readability: Is the language accessible at grade 7–9 reading level?
> - AI Detection Risk: Does any section sound robotic or AI-generated? Flag specific passages.
> - Competitive Edge: Does this chapter deliver something the top 5 competing books do not?
>
> After scoring: a prioritised list of specific edits (show the exact sentences to change and what to change them to), an overall grade (PUBLISH-READY / NEEDS REVISION / MAJOR REWRITE), and the single most impactful improvement.

> 你是一位发展性编辑，正在为亚马逊 KDP 上的商业出版审读一本非虚构书的一章。这本书的目标是 `[利基/读者]`，必须达到 4.5 星以上的平均评分。
>
> 这是章节书稿：`[粘贴章节]`
>
> 请在以下维度上评估这一章，每项打 1–10 分：
>
> - 开场钩子质量：开头是否在前 3 句内就抓住注意力？
> - 读者价值：梦想读者会不会觉得自己学到了**真正有用**的东西？
> - 可执行性：是否至少有一个读者可以立刻上手的行动？
> - 流畅度与结构：各小节之间的衔接是否合乎逻辑？过渡是否顺滑？
> - 声音一致性：语气是否从头到尾与 `[指定语气]` 保持一致？
> - 可读性：语言是否达到 7–9 年级阅读水平就能读懂？
> - AI 痕迹风险：有没有哪一段读起来机械、像 AI 生成的？把具体段落标出来。
> - 竞争优势：这一章是否给出了排名前五的竞品书所没有的东西？
>
> 打分之后，给出：一份按优先级排列的具体修改清单（要显示**原句**和**改成什么**）、一个总体评级（PUBLISH-READY 可出版 / NEEDS REVISION 需修订 / MAJOR REWRITE 需大改）、以及单点影响最大的那一项改进。
>
> 你自己补充上面的提示词，对你对上边新写的这一章进行改进。

## PROMPT 12 — The Line Editor
## 提示词 12 — 行文编辑（语句级润色）

**Strategic Purpose:** Perform a sentence-level polish for clarity, rhythm, and professional quality.

**战略目的：** 做句子级的润色，提升清晰度、节奏感和专业质感。

**THE PROMPT / 提示词正文**

> You are a professional line editor. Edit the following chapter for:
>
> - Sentence clarity — every sentence should communicate one idea simply
> - Redundancy — remove repeated ideas, filler words, and unnecessary qualifiers
> - Rhythm — vary sentence length (short sentences for impact, longer ones for explanation)
> - Active voice — convert passive constructions to active wherever possible
> - Specificity — replace vague words with concrete ones ("many" → specific number, "improve" → specific outcome)
> - AI tells — eliminate any phrase that sounds generically AI-generated. Common offenders: "it's worth noting", "at the end of the day", "in today's world", "let's explore"
>
> `[PASTE CHAPTER]`
>
> Return the fully edited chapter with all changes applied. Then provide a summary of the 10 most significant changes you made and why.

> 你是一位专业的行文编辑（line editor）。请对下面这一章做编辑，目标是：
>
> - 句子清晰度 —— 每个句子只用简单的方式表达一个意思
> - 冗余 —— 删掉重复的观点、填充词、以及不必要的话术修饰
> - 节奏 —— 让句长有变化（短句制造冲击，长句承载解释）
> - 主动语态 —— 尽可能把被动句改成主动句
> - 具体性 —— 用确切的词换掉含糊的词（"很多"→ 具体数字；"改善"→ 具体结果）
> - AI 腔 —— 清除一切听起来像 AI 套话的表达。常见惯犯："it's worth noting"、"at the end of the day"、"in today's world"、"let's explore"
>
> `[粘贴章节]`
>
> 返回已应用全部修改的完整章节。然后总结你所做的 10 处最重要的修改，以及为什么改。
>
> 你自己补充上面的提示词，对你对上边新写的这一章进行改进。

## PROMPT 13 — The Fact-Checker
## 提示词 13 — 事实核查员

**Strategic Purpose:** Verify all factual claims, statistics, and references in the manuscript.

**战略目的：** 核查全稿中所有事实性陈述、统计数据和引用。

**THE PROMPT / 提示词正文**

> You are a research fact-checker for a non-fiction publisher. Review the following chapter for factual accuracy.
>
> `[PASTE CHAPTER]`
>
> For every factual claim, statistic, date, name, or reference in this text:
>
> - Verify whether it is accurate using web search
> - Flag any claim that is outdated, misleading, or unverifiable
> - For flagged items, provide the correct information with a source
> - Identify any claims that sound plausible but cannot be verified — mark these as "NEEDS MANUAL VERIFICATION"
>
> Format as a numbered list: [CLAIM] → [STATUS: Verified / Incorrect / Unverifiable] → [CORRECTION or SOURCE if needed]. At the end, provide a Factual Confidence Score from 1–10 for the overall chapter.

> 你是一家非虚构出版机构的研究事实核查员。请审查下面这一章的事实准确性。
>
> `[粘贴章节]`
>
> 对文中每一条事实性陈述、统计数据、日期、人名或引用：
>
> - 用联网搜索核实它是否准确
> - 把任何过时、有误导性、或无法核实的说法标出来
> - 对被标记的条目，给出正确信息并附上来源
> - 找出那些听起来合理但无法核实的说法 —— 把它们标为 "NEEDS MANUAL VERIFICATION"（需人工核实）
>
> 以编号清单格式输出：[说法] → [状态：已核实 / 有误 / 无法核实] → [更正值 或 来源（如需要）]。最后，为整章给出一个 1–10 的"事实可信度分数"。

## PROMPT 14 — The Introduction & Conclusion Writer
## 提示词 14 — 绪论与结论撰写者

**Strategic Purpose:** Write the two most conversion-critical sections of the book — the Introduction (which Amazon's Look Inside feature shows to prospective buyers) and the Conclusion (which drives reviews and repeat purchases).

**战略目的：** 写出全书对转化影响最大的两个部分 —— 绪论（亚马逊"免费试读"会把它展示给潜在买家）和结论（它决定评论数和复购）。

**THE PROMPT / 提示词正文**

> You are a bestselling non-fiction author known for opening chapters that are impossible to put down. I need you to write the Introduction and Conclusion for my book.
>
> Book: "`[TITLE]`" · Dream Reader: `[persona]` · The book covers: `[scope]` · Chapter outline: `[outline]`
>
> **INTRODUCTION (Target: 1,500–2,000 words):**
>
> - Must pass the "Look Inside Test" — this is the first content a buyer sees. If it does not hook them in 30 seconds, they leave.
> - Open with a story, scenario, or bold statement that makes the Dream Reader think: "This person understands my exact situation."
> - Address the core pain point directly within the first 300 words
> - Preview what the reader will gain — specific outcomes, not vague promises
> - Include a "How to use this book" section
> - End with a sentence that makes turning to Chapter 1 irresistible
>
> **CONCLUSION (Target: 1,000–1,500 words):**
>
> - Summarise the reader's journey — remind them how far they have come
> - Reinforce the single most important takeaway
> - Include a direct call-to-action: ask for a review (naturally, not desperately)
> - Tease the next book in the series (if applicable)
> - End with an emotional note that makes the reader feel the investment was worth it

> 你是一位畅销非虚构作者，以"让人放不下的开篇"著称。我需要你为我的书写绪论和结论。
>
> 书："`[书名]`" · 梦想读者：`[画像]` · 本书涵盖：`[范围]` · 章节大纲：`[大纲]`
>
> **绪论（目标：1,500–2,000 词）：**
>
> - 必须通过"试读测试"—— 这是买家看到的第一段内容。如果 30 秒内钩不住他，他就走了。
> - 用一个故事、一个场景或一个大胆论断开场，让梦想读者心里想："这个人懂我现在的处境，一模一样。"
> - 在前 300 词内正面命中那个核心痛点
> - 预告读者会得到什么 —— 要具体成果，不要含糊承诺
> - 包含一节"本书使用方法"
> - 用一句话收尾，让"翻到第一章"变成一件无法抗拒的事
>
> **结论（目标：1,000–1,500 词）：**
>
> - 回顾读者的旅程 —— 提醒他已经走了多远
> - 强化那个最重要的单一收获
> - 给出直接的行动号召：请求评论（要自然，不要可怜巴巴）
> - 预告系列里的下一本（如适用）
> - 用一个情绪落点收尾，让读者觉得这笔钱花得值

## PROMPT 15 — The Bonus Resource Creator
## 提示词 15 — 附加资源创造者

**Strategic Purpose:** Create high-value bonus materials that enhance the reader experience, drive email list sign-ups, and generate positive reviews.

**战略目的：** 制作高价值附加材料，用来提升读者体验、拉动邮件列表订阅、并催生好评。

**THE PROMPT / 提示词正文**

> You are a product designer creating bonus resources for a non-fiction book. These bonuses serve three purposes: (1) increase perceived value, (2) drive readers to our email list via a download link inside the book, and (3) give readers a reason to leave a positive review.
>
> Book: "`[TITLE]`" in the `[NICHE]` space · Dream Reader: `[persona]` · Chapter outline: `[outline]`
>
> Design the following bonus resources:
>
> - **Quick-Start Checklist:** A 1-page printable checklist that summarises the entire book's action steps — something the reader can pin to their wall and use as a daily reference.
> - **Companion Workbook Excerpt:** A 5–10 page workbook with exercises, templates, and fill-in sections. (We will offer the full workbook as a separate product.)
> - **Resource List:** A curated list of 15–20 tools, apps, books, and websites relevant to the reader's goals, with brief annotations explaining why each matters.
> - **Bonus Chapter Preview:** A 500-word preview of a "lost chapter" covering an advanced topic not in the main book — this creates desire for the next book in the series.
>
> For each resource, provide the full content ready for formatting. Include a CTA directing readers to `[URL]` to download.

> 你是一位产品设计师，为一本非虚构书设计附加资源。这些赠品服务三个目的：(1) 提升感知价值；(2) 通过书内的下载链接把读者导流到我们的邮件列表；(3) 给读者一个留下好评的理由。
>
> 书："`[书名]`"（`[利基]` 领域）· 梦想读者：`[画像]` · 章节大纲：`[大纲]`
>
> 请设计以下附加资源：
>
> - **快速上手清单：** 一页可打印清单，把全书的行动步骤浓缩进去 —— 读者可以贴在墙上每天对照。
> - **配套工作簿节选：** 一份 5–10 页的工作簿，含练习、模板和填空栏。（完整工作簿我们作为独立产品提供。）
> - **资源清单：** 一份精选的 15–20 项工具、App、书和网站清单，与读者目标相关，每项配一句说明为什么值得看。
> - **附加章节预告：** 一篇 500 词的"遗失章节"预告，讲一个正文里没有的进阶话题 —— 用它制造对系列下一本的渴望。
>
> 对每个资源，给出可直接排版的完整内容。并包含一个 CTA，引导读者到 `[URL]` 下载。

## PROMPT 16 — The Formatting Quality Checklist
## 提示词 16 — 排版质量检查清单

**Strategic Purpose:** Generate a pre-publication quality assurance checklist custom to your book's specifications.

**战略目的：** 生成一份贴合你这本书具体规格的、出版前的质量保证检查清单。

**THE PROMPT / 提示词正文**

> You are a production manager at a publishing house. I am about to format and upload my book to Amazon KDP. Create a comprehensive pre-publication checklist.
>
> Book specifications: Title: `[TITLE]` · Formats: Kindle eBook, Paperback, Hardcover · Paperback trim size: `[SIZE]` · Approximate page count: `[PAGES]` · Interior: Black and white / colour
>
> The checklist must cover:
>
> - **Manuscript QA:** Spell check, grammar check, formatting consistency, chapter heading styles, page breaks, table of contents accuracy
> - **eBook Specifics:** Hyperlink functionality, table of contents navigation, image resolution, responsive formatting
> - **Paperback Specifics:** Trim size compliance, margin settings, bleed requirements, spine width, ISBN placement, barcode area
> - **Hardcover Specifics:** Case wrap dimensions, spine text formatting, additional margin requirements
> - **Front & Back Matter:** Title page, copyright page, dedication, about the author, also-by page, review request, bonus resource CTA
> - **KDP Upload:** Category selection strategy (3 categories), keyword placement (7 keyword fields), pricing strategy across formats, publication date selection
>
> Format as a checkable list grouped by section. Flag the 5 most commonly missed items with a warning icon. ⚠

> 你是一家出版社的生产经理。我正准备把书排版并上传到亚马逊 KDP。请创建一份完整的出版前检查清单。
>
> 图书规格：书名：`[书名]` · 形态：Kindle 电子书、平装、精装 · 平装开本尺寸：`[尺寸]` · 大约页数：`[页数]` · 内文：黑白 / 彩色
>
> 清单必须覆盖：
>
> - **书稿质检：** 拼写检查、语法检查、格式一致性、章标题样式、分页、目录准确性
>   - **电子书专项：** 超链接是否可用、目录跳转、图片分辨率、响应式排版
>
> - **平装专项：** 开本尺寸合规、页边距设置、出血要求、书脊宽度、ISBN 位置、条码区
> - **精装专项：** 外壳包裹尺寸、书脊文字排版、额外的页边距要求
> - **前置与后置页：** 扉页、版权页、献词、作者简介、同作者作品页、求评论页、附加资源 CTA
> - **KDP 上传：** 分类选择策略（3 个分类）、关键词位（7 个关键词栏）、跨形态定价策略、出版日期选择
>
> 以分组的可勾选清单形式输出。把最常被漏掉的 5 项用警告图标标出来。⚠

---

# 模块五 — 视觉识别（Prompt 17–19）
### 原文锚点：MODULE V — Visual Identity ｜ Cover Design Strategy, AI Art Direction, and Ideogram Prompt Engineering ｜ 预计 20 分钟

**模块导语（中文）**：书的封面是它最重要的营销资产。在亚马逊上，买家大约在两秒内决定是否点进你的书 —— 而这个决定几乎完全是在**封面缩略图**上做出的。一个能在 100 像素宽度下同时传达"类型、质量、相关性"的专业封面，是不可妥协项。

---

### Prompt 17 — The Cover Design Brief（封面设计简报）
**战略目的**：生成一份完整的创意简报，用来指导后续 AI 生成的封面概念。

提示词要点（照此填即可用）：
- 角色：专精亚马逊 KDP 封面的美术总监，理解"封面必须先当 100px 缩略图用，其次才是大图"
- 输入：书名、副书名、作者/笔名、利基、梦想读者
- 先要求 Claude **联网搜索该利基下 Top 10 畅销书封面**，然后输出：
  1. **类型视觉语言**：哪些设计元素在告诉读者"这是一本 [某类] 书"（配色、图像类型、字体风格、版式规律）
  2. **3 个封面概念**：A 合规型（Genre-Compliant）、B 提升型（Elevated）、C 破位型（Disruptor）
  3. 每个概念都要给：**精确十六进制色值**的配色方案、字体建议、主图描述、版式结构、书脊设计、封底元素
  4. **缩略图测试标准**：在 100px 宽下书名还读得清吗？配色在亚马逊白色背景上跳不跳？
  5. 推荐概念 + 理由

---

### Prompt 18 — The Ideogram Prompt Engineer（Ideogram 提示词工程师）
**战略目的**：为 Ideogram 生成专业级封面图像，产出精确、经过优化的提示词。

提示词要点：
- 角色：专精为 Ideogram 写封面提示词的 AI 美术总监，懂 Ideogram 的强项是**文字渲染、干净构图、商业设计审美**
- 输入：Prompt 17 的封面简报
- 要求生成 **5 条 Ideogram 提示词**（同一概念的不同变体），每条必须：
  - 以方括号里的版式模板名开头：`[BOOK COVER]`、`[POSTER]` 或 `[TYPOGRAPHY]`
  - 把书名原文放进**引号**里（Ideogram 靠引号渲染文字）
  - 副书名单独一行，也放引号
  - 用精确的、电影感的语言描述画面构成
  - 指定配色、光线、风格（如 "flat design"、"3D render"、"watercolour illustration"）
  - 需要时加**负向提示词**（如 "no human faces"、"no cluttered elements"）
  - 以 "professional book cover design, high resolution, print-ready" 收尾
- 另外再给 **3 条**用于封底和书脊的提示词，保持与封面视觉一致

---

### Prompt 19 — The Cover A/B Testing Framework（封面 A/B 测试框架）
**战略目的**：建立一套系统化的测试框架，用数据（而非个人品味）选出转化最高的封面。

提示词要点：
- 角色：把 A/B 测试原则用在封面选择上的转化率优化专家
- 输入：已生成的封面概念数量、书名、各概念描述
- 要求产出"封面测试方案"，含 5 项：
  1. **缩略图模拟**：怎么在 100px 宽度下测每个封面；建一个 5 项标准、各 1–10 分的评分量表
  2. **受众测试方法**：用 [Instagram 投票 / PickFu / 小额投放] 设计 A/B 测试，给出**要问的确切问题**和结果解读方式
  3. **类型合规检查**：每个封面与该利基 Top 10 畅销书的吻合度，1–10 分
  4. **情绪反应测试**：这个封面应该在梦想读者身上触发什么情绪？各变体做到了吗？
  5. **最终选择矩阵**：把所有因子加权，得出一个明确赢家

> ☕ **BREAK — FIFTEEN-MINUTE INTERVAL**（源文件在此处插入 15 分钟休息）

---

# 模块六 — 店面（Prompt 20–24）
### 原文锚点：MODULE VI — The Storefront ｜ Amazon Listing Optimisation, Description Copywriting, and Backend Strategy ｜ 预计 25 分钟

**模块导语（中文）**：一本好书配一个差的商品页，表现会低于预期；一本普通的书配一个好的商品页，会卖得更好。这不是犬儒，这就是亚马逊市场机制的真实运作方式。你的商品页**同时**是两样东西：给人类买家看的销售页，以及给亚马逊搜索与推荐引擎看的算法信号。

---

### Prompt 20 — The Book Description Machine（图书描述文案机）
**战略目的**：用 AIDA-Proof-CTA 框架，写一段高转化的亚马逊图书描述。

提示词要点：
- 角色：专做亚马逊图书描述的直效文案（direct-response copywriter）。描述必须同时做到两件事：(1) 说服真人点"立即购买"；(2) 为亚马逊 A9 算法埋入战略关键词
- 输入：书名、利基关键词、梦想读者、本书承诺、关键章节/主题
- 按这个框架写：
  - **HOOK 钩子（2–3 句）**：用一个大胆的问题或论断开场，直击梦想读者的核心痛点。**用他自己在 Prompt 6 里的原话**
  - **AGITATE 加剧（3–4 句）**：描述"不解决这个问题"的后果，要具体、有画面感
  - **SOLUTION 方案（3–4 句）**：把这本书定位成"他现在所在"与"他想去的地方"之间的桥
  - **PROOF 证据 — 书里有什么（要点清单）**：列 8–12 条读者会发现的具体内容。每条以动词开头，并带一个引发好奇的具体细节
  - **CTA 行动号召（2–3 句）**：制造紧迫感但不油腻；提醒他"不行动的代价"；以明确的购买指令收尾
- 格式：用 HTML 加粗标签；总长控制在 4,000 字符内；自然融入 [关键词]
- 产出 **2 个变体**：A 版（情绪化、故事驱动）、B 版（直接、利益驱动）

---

### Prompt 21 — The Backend Keyword Strategist（后台关键词策略师）
**战略目的**：为亚马逊 KDP 的 7 个关键词字段，生成经过优化的关键词串。

提示词要点：
- 角色：亚马逊 SEO 专家，要填满 KDP 的 7 个后台关键词字段
- **规则（这部分是干货，务必照做）**：
  - 每个字段最多 50 字符
  - **不要用逗号**
  - **不要重复**书名或副书名里已经出现的词
  - 要包含常见搜索词的**拼错版本**
  - 用读者真正会搜的**长尾短语**
  - **不要**写竞品书名或作者名
- 输入：书名、利基
- 产出：
  1. 7 条优化关键词串，一字段一条，各 50 字符以内
  2. 逐字段说明它捕获的是什么搜索意图
  3. 另外一份 20 个关键词的补充清单，用于亚马逊广告投放

---

### Prompt 22 — The Category Selector（分类选择器）
**战略目的**：找出能让新书曝光与 Bestseller 潜力最大化的最优亚马逊分类组合。

提示词要点：
- 角色：亚马逊分类策略师（亚马逊允许 3 个浏览分类）
- 输入：书名、利基、内容摘要
- 要求先**联网查当前的分类结构**，然后对每个推荐分类给出：
  - 完整分类路径（例：Books > Business & Money > Personal Finance > Budgeting）
  - 该分类下的图书数量估算
  - **当前第一名畅销书的 BSR** —— 这个数字告诉你这个分类有多卷
  - 它是"大池塘"还是"小池塘"分类
- 推荐策略：**1 个高度相关的"大池塘"**拿流量，加 **1–2 个"小池塘"**（在那里我们现实地能冲到 #1 New Release 或 #1 Bestseller）。另外指出哪些分类需要**发邮件给亚马逊**申请纳入

---

### Prompt 23 — The Author Bio Generator（作者简介生成器）
**战略目的**：写一份有说服力的作者简介，支撑笔名策略与读者信任。

提示词要点：
- 角色：品牌文案，为笔名 `[PEN NAME]` 写亚马逊作者简介
- **重要前提**：这是一个笔名 —— 简介要可信、专业，但**不能做出无法验证的断言**
- 产出三个版本，且三者必须一致：
  1. **SHORT BIO（150 词）**：用于亚马逊作者页 —— 聚焦"读者能得到什么"，而不是作者履历
  2. **LONG BIO（300 词）**：用于书末 —— 加入个性、写作动机，以及与读者旅程的连接
  3. **"About the Author" 书内短版（50 词）**：有力、温暖、好记
- **不要**声称学位、证书或职业头衔。改用这些方式建立权威：个人经验年数、帮助过的人数、热情驱动的语言、以及具体性

---

### Prompt 24 — The A+ Content Architect（A+ 内容架构师）
**战略目的**：设计亚马逊 A+ 内容版式（需已注册 Brand Registry），用视觉强化商品页。

提示词要点：
- 角色：亚马逊 A+ 内容设计师
- 输入：书名、关键卖点、梦想读者
- 设计一个 **5 模块 A+ 版式**：
  1. **Hero Banner 主视觉横幅**：图 + 叠加标题文字，强化本书核心承诺
  2. **Comparison Chart 对比表**："为什么这本书不同" —— 与"泛泛的替代品"在 5 个维度上对比。**不要点名具体竞品**
  3. **What's Inside 书里有什么**：用图标 + 短描述做逐章视觉预览，列出最有吸引力的 6 章
  4. **Author Credibility 作者可信度**：可选放照片的模块，配作者简介 + 一段"Why I Wrote This"个人陈述
  5. **Cross-Sell 交叉销售**：展示你书柜里另外 2–3 本，配短描述并保持视觉统一
- 每个模块都要给：确切文字内容、图像描述、版式说明

---

# 模块七 — 上市运营（Prompt 25–27）
### 原文锚点：MODULE VII — Launch Operations ｜ Go-to-Market Execution, Review Strategy, and Launch Week Playbook ｜ 预计 15 分钟

**模块导语（中文）**：出版后的头 72 小时，重要性远超比例。亚马逊算法给新书一段"蜜月期"的额外曝光。你在这个窗口里做的事 —— 如何拉动初始销售速度、如何产生早期评论、如何向算法信号"这本书相关"—— 会决定你的书接下来几个月的走势。

---

### Prompt 25 — The Launch Playbook Generator（上市作战手册生成器）
**战略目的**：为出版后头 14 天，生成一份逐日的上市计划。

提示词要点：
- 角色：图书上市策略师
- 输入：书名、出版日期、形态、上市预算、已有资产（邮件列表、社媒账号等）
- 分三段：
  - **Day 1–3（上市窗口）**：最大化初始销售速度的确切动作、如何激活现有受众、促销站提交（列出**具体站点和时机**）、定价策略
  - **Day 4–7（动能积累）**：亚马逊广告启动（何时开、初始预算）、评论征集策略（**只用合规手段**）、社会证明放大
  - **Day 8–14（优化）**：第一次表现复盘 —— 看哪些指标、意味着什么；基于初期数据的商品页调整；广告活动精细化；长期销售速度策略
- 每一天都要给：具体行动项、耗时估计、预算分配

---

### Prompt 26 — The Review Request System（评论征集系统）
**战略目的**：生成合规、有效的评论请求文案与 ARC（Advance Copy）策略。

提示词要点：
- 角色：出版营销专家。要求一套**100% 符合亚马逊服务条款**的早期评论系统，并明确声明：**不买评论、不激励评论、不用评论互换服务**
- 产出：
  1. **书末评论请求**：一段温暖自然的文字，请读者留真实评论。写 **3 个变体** —— 真诚的、直接的、幽默的
  2. **给个人网络的邮件**：面向朋友、家人、行业联系人。必须强调你要的是**真实评论**，不是假五星
  3. **ARC 邮件模板**：向博主、社区成员、利基影响者分发"提前审阅本"的正式邮件。含 ARC 提供方式、时间预期，以及**提醒：评论必须披露"收到免费副本"**
  4. **跟进序列**：给 ARC 接收者的 3 封邮件 —— (1) 送达 + 阅读说明；(2) 第 7 天温和提醒；(3) 第 14 天最后提示并附具体评论链接
- 所有文案必须符合亚马逊评论政策。不激励、不交换。

---

### Prompt 27 — The Promotion Site Submitter（促销站提交器）
**战略目的**：为各图书促销网站生成可直接提交的提交文案，并给出最优提交时机。

提示词要点：
- 角色：图书促销协调员。各站格式要求不同
- 输入：书名、作者、ASIN、Kindle 价 / 平装价、分类、亚马逊链接
- 为下列站点分别生成定制提交文案：
  - **BookBub**（若符合条件）—— 400 字符描述
  - **Freebooksy / Bargain Booksy** —— 短促销语
  - **Book Gorilla** —— 针对分类的推介
  - **Robin Reads** —— 50 词促销文字
  - **Written Word Media** —— 推广描述
- 每一篇都要匹配**该平台表现最好的语气与格式**。另外标注：一周里哪一天、什么时间提交，曝光最大

---

# 模块八 — 广告投放引擎（Prompt 28–31）
### 原文锚点：MODULE VIII — The Advertising Engine ｜ Amazon Ads Strategy, Campaign Architecture, and Optimisation ｜ 预计 25 分钟

**模块导语（中文）**：亚马逊每年新增超过 140 万本自出版书，只靠自然曝光无法支撑"组合级"的收入。亚马逊广告是控制你书曝光量的主要杠杆。本模块四条提示词，把整套广告基础设施从关键词调研一路搭到投放优化。

---

### Prompt 28 — The Keyword Arsenal Builder（关键词弹药库构建器）
**战略目的**：为亚马逊广告投放，生成一份覆盖精确、词组、ASIN 定位与否定词的全面关键词清单。

提示词要点：
- 角色：专精图书广告的亚马逊广告关键词策略师
- 输入：书名、利基、主目标关键词、关键主题、Top 5 竞品书名
- 按类别生成：
  - **Exact Match Seeds 精确匹配种子（30 个）**：买家已经知道要什么时会搜的高意图短语
  - **Broad Match Discovery 词组匹配发现（30 个）**：捕获相邻需求的 Related 短语
  - **ASIN Targets ASIN 定位（15 个）**：你的广告该出现在哪些竞品书页面下，并逐条说明**为什么你的书是有说服力的替代选项**
  - **Category Targets 分类定位（5 个）**：广告该进入的亚马逊浏览分类
  - **Negative Keywords 否定词（20 个）**：看起来相关但会招来错误买家的词（如 "free"、"pdf"）—— 这些是保护预算的
- 每组关键词都要估：搜索量（高/中/低）、竞争程度、建议起始出价区间（$0.50–$1.50）
- 输出为可直接进表格的格式

---

### Prompt 29 — The Campaign Architect（广告活动架构师）
**战略目的**：为新书签发布设计完整的亚马逊广告活动结构。

提示词要点：
- 角色：亚马逊广告活动经理
- 输入：书名、日预算、上市日期、关键词清单（来自 Prompt 28）
- 设计四条活动，**预算配比是这一条的核心**：
  - **Campaign 1 — Auto Discovery 自动发现（预算 20%）**：自动定向，用来发现到底哪些词能转化。默认出价 $0.40
  - **Campaign 2 — Exact Match Performance 精确匹配主力（预算 40%）**：手动活动，用你置信度最高的 15 个词做精确匹配
  - **Campaign 3 — ASIN Targeting（预算 25%）**：在竞品书页面做商品定向
  - **Campaign 4 — Broad Match Discovery（预算 15%）**：宽泛匹配，捞长尾流量
- 每条活动给：命名规范、定向类型、预算分配、出价策略、否定词、何时启动、要盯的 KPI
- 另附 Week 1 / Week 2 / Week 4 优化检查清单

---

### Prompt 30 — The ACOS Optimisation Analyst（ACOS 优化分析师）
**战略目的**：分析现有广告表现数据，并给出具体、按优先级排列的优化动作。

提示词要点：
- 角色：亚马逊广告表现分析师。输入：过去 [N] 天的活动数据
- 分析并给出：
  1. **整体健康评估**：我的总 ACOS 可持续吗？（**目标：上市期低于 70%，稳态低于 40%**）以我每单版税 $[X] 计算，我的真实盈亏平衡 ACOS 是多少？
  2. **Winner Keywords 赢家词**：哪些词的 ACOS 低于盈亏平衡、应该加预算加价？
  3. **Loser Keywords 输家词**：哪些词已花超过 $[X] 却零销售？建议：暂停 / 降价 / 加入否定词
  4. **Opportunity Keywords 机会词**：哪些词 CTR 好但转化低？—— 这通常说明该优化的是**商品页**，不是关键词
  5. **Budget Reallocation 预算重分配**：日预算在各活动间怎么挪？给**具体金额**
  6. **Next Actions**：本周影响最大的 5 项改动，按预期收入影响排序

---

### Prompt 31 — The International Ads Launcher（国际广告启动器）
**战略目的**：把已验证有效的美国广告策略，适配到英国、德国、法国、西班牙、意大利、日本等亚马逊市场。

提示词要点：
- 角色：国际亚马逊广告策略师。输入：书名、美国市场表现指标、想扩张到的市场
- 对每个市场给出：
  1. **关键词翻译与本地化**：把 Top 10 美国关键词译成当地语言。**不要直接用谷歌翻译** —— 要按当地读者实际的搜法来改
  2. **预算建议**：按市场相对规模，给出"占美国花费百分比"形式的建议日预算
  3. **出价策略**：这个市场的 CPC 通常比美国高还是低？给建议起始出价
  4. **市场特定说明**：当地竞争水平、分类差异、季节规律等独特考量
  5. **活动结构**：每个市场起步时用简化的两活动结构（一自动、一手动）
- 给一份**分阶段铺开计划**：按收入潜力与进入难度，排第一、第二、第三该开哪个市场

---

# 模块九 — 规模化架构（Prompt 32–34）
### 原文锚点：MODULE IX — Scale Architecture ｜ Portfolio Expansion, Series Strategy, and International Growth ｜ 预计 20 分钟

**模块导语（中文）**：一本书是一个产品；十二本书的书柜才是一门生意。差别不只是算术上的 —— 而是**结构性的**。书柜把收入分散到多个关键词、多个分类、多个市场上，并创造出网络效应：每一本新书都会通过"Also By"页、亚马逊推荐引擎、以及 A+ 内容的交叉销售，把流量导回已有书目。

---

### Prompt 32 — The Series Strategy Planner（系列策略规划器）
**战略目的**：设计一个 3–5 本书的系列架构，让交叉销售与书柜收入最大化。

提示词要点：
- 角色：出版书柜策略师。输入：现有书名、利基、表现（BSR、定价）、想做的 3–5 本相关书
- 当前书信息：书名、覆盖主题、梦想读者、表现最好的关键词、评论里读者的常见请求
- 设计系列架构，**四本各有明确分工**：
  - **Book 2 — The Natural Sequel 自然续作**：读者接下来需要什么？要读完第一本后感觉"下一步显然是它"
  - **Book 3 — The Deep Dive 深潜**：对第一本里最受欢迎的那个子话题做专门深挖。受众更窄但购买意图更强
  - **Book 4 — The Companion Tool 配套工具**：工作簿、计划表、日志或模板合集。通常字数更少、定价更高、毛利极高
  - **Book 5（可选）— The Audience Expander 受众扩展**：把核心主题重新包装，给一个不同的人群
- 每本给：书名 + 副书名、目标关键词、预计制作时间、如何与已有书交叉销售、该攻哪些亚马逊分类
- 再排出最优的**出版顺序与时间表**

---

### Prompt 33 — The Translation Brief（翻译与本地化简报）
**战略目的**：为国际扩张，生成一份把该书翻译成另一种语言的详细简报。

提示词要点：
- 角色：出版本地化专家。目标：在 [某市场] 出版翻译版
- 输入：英文书名、副书名、字数、利基关键词
- 产出"翻译与本地化简报"，含 7 项：
  1. **书名改编**：**不要直译**英文书名。去调研当地亚马逊上的等价关键词短语是什么，提 3 组为当地搜索引擎优化的书名/副书名
  2. **关键词调研**：找出该利基在当地亚马逊站点的 Top 10 关键词
  3. **文化适配说明**：有哪些文化引用、习语、例子在当地**不会**产生共鸣？列出来并给当地替代方案
  4. **市场评估**：这个利基在当地站点竞争程度如何？
  5. **商品页文案**：为当地市场改写图书描述、后台关键词、作者简介
  6. **封面适配**：英文封面在当地市场行不行，还是类型惯例不同？
  7. **预算估算**：专业人工翻译的大致成本

---

### Prompt 34 — The Portfolio Performance Analyst（书柜表现分析师）
**战略目的**：分析整个书柜的表现数据，并给出战略性的增长与优化建议。

提示词要点：
- 角色：书柜投资分析师 —— 只不过分析的是书，不是股票。输入：当前 KDP 书柜的表现数据
- 产出"书柜表现报告"，含 6 项：
  1. **健康指标**：月总收入、总广告花费、书柜级 ACOS、单本收入、收入集中度
  2. **Star Performers 明星书**：哪几本在产生不成比例的回报？能从它们身上学到什么？
  3. **Underperformers 落后书**：哪几本在盈亏线下？诊断最可能的原因，并建议：修 / 减广告 / 接受它作为书柜分散配置的一部分
  4. **Portfolio Gaps 书柜缺口**：基于现有的利基与形态，明显的缺口在哪里？
  5. **国际扩张优先级**：哪本书该先翻成哪种语言？按预期 ROI 排序
  6. **90 天行动计划**：未来 90 天影响最大的 10 项行动，按优先级排，目标是书柜收入增长 30%+
- 格式：执行简报体 —— 顶部放仪表盘摘要，下面放详细分析

---

# 模块十 — 内容飞轮（Prompt 35–36）
### 原文锚点：MODULE X — The Content Flywheel ｜ Marketing, Social Proof, and Content Repurposing ｜ 预计 25 分钟

**模块导语（中文）**：书柜里的每一本书不只是一个产生收入的资产，它同时是一台**内容引擎**。一本 30,000 词的书，包含的材料足够喂养数月的社交媒体内容、邮件营销、博客文章和引流磁铁。本模块两条提示词，把你的书改造成一台把流量送回亚马逊商品页的营销机器。

---

### Prompt 35 — The Content Repurposing Engine（内容再利用引擎）
**战略目的**：把书里的内容提取并转化为可在社交媒体、邮件序列和博客上执行的计划。

提示词要点：
- 角色：内容策略师，专长是把长文内容改造成跨平台营销资产
- 输入：已出版的书名、利基、书的内容摘要
- 生成一份 **30 天内容日历**，产出量是这条提示词的关键：
  - **30 条 X/Twitter 帖**：每条从书里提取一个洞见、技巧或反直觉观点。格式 = 钩子行 + 2–3 句支撑 + CTA。混合配比：线程 3 条、单推 15 条、引言式 7 条、数据/统计 5 条
  - **8 条 LinkedIn 帖**：较长的思想领导力文章，把作者定位为专家。每条 200–300 词
  - **4 组 Instagram 轮播概念**：每组 7–10 张，覆盖一个关键主题，给出逐张文字内容
  - **4 封邮件培育序列**：给下载了免费附加资源的新订阅者。顺序 = 欢迎+快速见效 → 深潜洞见 → 常见错误 → 直接推介
  - **2 篇博客文章（各 1,500 词）**：SEO 优化，针对相关关键词，并链向书的亚马逊页面
- 日历要指明哪条内容放哪一天，以保持最优节奏

---

### Prompt 36 — The Social Proof Amplifier（社会证明放大器）
**战略目的**：把正面的读者评论转化为营销资产，用于列表页与广告投放。

提示词要点：
- 角色：社会证明营销专家。输入：这本书最新的评论与反馈
- 用这些社会证明产出 5 类营销资产：
  1. **Testimonial Highlight Reel 金句集锦**：挑 5 条最有力的引用，每条抽出**最好的一句**，做成可用于社媒图卡的引言块
  2. **Review Themes Analysis 评论主题分析**：读者最常夸的 3 件事是什么？把每个主题变成一句营销话术："Readers are saying [主题] — here's what they mean."
  3. **Objection-Handling Content 异议处理内容**：找出评论里的顾虑或轻度批评。针对每一条，做一个**主动回应**的内容件 —— 把异议转成卖点
  4. **Updated Book Description Insert 描述更新插入块**：基于最强的那几条评论，写一段 2–3 行的 "What Readers Are Saying"，加到亚马逊描述**最顶部**
  5. **"Wall of Love" 好评墙**：把所有最佳引用汇成一个可直接做视觉的文档，用于落地页、Skool 帖或社媒
- **红线**：所有内容由始至终**不得编造或美化评论** —— 用读者的原话，只是为冲击力重新排版

---

# 收尾 — 综合与落地路线图
### 原文锚点：CLOSING — Synthesis & Implementation Roadmap ｜ 预计 10 分钟

## 是系统，不是提示词（The System, Not the Prompts）

这才是我们说"出版操作系统"的意思。每一条提示词是一个**函数**。每个函数接收一个输入、产出一个输出。上一个函数的输出，变成下一个函数的输入。当整条链条顺畅跑起来时，你就拥有了一台机器：它把市场情报转化为已出版、已营销、正在产生收入的书的资产 —— 其速度与稳定性，在五年前是不可想象的。

## 时间压缩（The Time Compression）

压缩效应是**复利**的。你的第一本书要六周。第二本只要四周 —— 因为你已经打磨过提示词、建好了模板变体、并把整套流程内化了。到第五本，从调研到上市的周期是**三周**。到第十二本（也就是"最小可行书柜"）时，你已经用大约**十八个月的兼职工作**，建起一个十万美元年收入的资产。

按顺序使用这三十六条提示词，一个单干者每天投入三到四小时，从"我想在个人理财领域出一本书"到"我的书已在亚马逊上架、广告在跑、内容日历在执行"的完整旅程，大约**四到六周**可以完成。而同样的旅程，没有 AI 增强的话需要四到八个月 —— 生产周期被压缩了**三到五倍**。这不是渐进式改良，这是出版经济学的结构性转变。

## 落地建议（Implementation Recommendation）

源文件在这里给出一张周次路线图卡：

| 周次 | 要做的事 |
|---|---|
| WEEK 1 | GTS 引擎 —— 跑 Prompt 6–9，定义你的书的概念与大纲 |
| WEEKS 3–4 | 生产线 —— 跑 Prompt 10–16，产出书稿与附加材料 |
| WEEK 2 | 市场情报 —— 跑 Prompt 1–5 并选定你的利基 |
| WEEKS 5–6 | 上市 —— 跑 Prompt 25–27，执行你的 go-to-market 计划 |
| WEEK 4 | 封面设计 —— 与终稿并行跑 Prompt 17–19 |
| WEEK 5 | 商品页优化 —— 跑 Prompt 20–24，准备店面 |
| WEEK 6+ | 广告 —— 激活 Prompt 28–31，开始优化循环 |
| ONGOING | 规模化与飞轮 —— 在你通往"十二本最小可行书柜"的路上，部署 Prompt 32–36 |

## 最后的话

把这些提示词存进你的 Notion 工作区。每本书都重新定制变量。随着你弄清什么有效，**去迭代提示词本身**。这个库不是一份静态文档 —— 它是一套随着每一次使用而变好的活的系统。

The AI Publisher's Prompt Library was developed by the founding team at Nespola.io as part of the PublishingOS system. Every prompt in this library has been tested in the production of real book portfolios generating real revenue on Amazon KDP.

《AI 出版者提示词库》由 Nespola.io 创始团队开发，是 PublishingOS 体系的一部分。库中每一条提示词都在真实书柜的生产流程中测试过，这些书柜正在亚马逊 KDP 上产生真实收入。

If you are reading this as a member of the PublishingOS community, you have a structural advantage that most publishers do not: a system. Use it.

如果你是以 PublishingOS 社区成员的身份读到这份材料，你拥有多数出版者不具备的结构性优势：一套系统。用它。

> © 2026 Nespola.io — All rights reserved. PublishingOS is a product of Nespola.io.
> 本中文研读部分为个人学习用途整理，版权归 Nespola.io 所有，请勿传播或商用。

---

# 附：三十六条提示词速查表

| # | 名称 | 属于模块 | 一句话用途 |
|---|---|---|---|
| 1 | Niche Discovery Engine | II | 产出 10–15 个符合六项标准的子利基 |
| 2 | Keyword Deep-Dive Analyser | II | 单关键词的需求/竞争/营收/风险 → GO 或 NO GO |
| 3 | Trend Validator | II | 联网判：常青 / 季节性 / 靠热点 |
| 4 | Competitor Teardown | II | 拆解头部竞品，把差评变成你的产品路线图 |
| 5 | Niche Scorecard | II | 八维加权记分卡，利基最终裁定 |
| 6 | Dream Reader Persona | III | 一页纸读者画像（含反面画像） |
| 7 | Positioning Statement | III | 定位声明 + 3 个角度 + 5 组书名 |
| 8 | Chapter Outline Architect | III | 12–18 章、服务读者旅程与算法期待 |
| 9 | Content Brief Generator | III | 交给代笔/AI 的主参考文档 |
| 10 | Chapter Drafter | IV | 单章初稿（含 8 条硬规则，禁 AI 腔） |
| 11 | Developmental Editor | IV | 八维结构审读 + 可执行修改清单 |
| 12 | Line Editor | IV | 句子级润色：清晰/节奏/主动语态/去 AI 腔 |
| 13 | Fact-Checker | IV | 联网核查每条断言，给事实可信度分 |
| 14 | Introduction & Conclusion Writer | IV | 决定转化的绪论与结论 |
| 15 | Bonus Resource Creator | IV | 4 类赠品：拉订阅 + 催好评 |
| 16 | Formatting Quality Checklist | IV | 出版前 QA 清单（含 5 个最易漏项） |
| 17 | Cover Design Brief | V | 先搜 Top10 封面，再出 3 概念 + 色值 |
| 18 | Ideogram Prompt Engineer | V | 5 条封面提示词 + 3 条封底/书脊 |
| 19 | Cover A/B Testing Framework | V | 用数据而非品味选封面 |
| 20 | Book Description Machine | VI | HOOK-AGITATE-SOLUTION-PROOF-CTA，出 2 版 |
| 21 | Backend Keyword Strategist | VI | 填满 7 个后台字段（50 字符/无逗号/不重复） |
| 22 | Category Selector | VI | 1 个大池塘 + 1–2 个小池塘 |
| 23 | Author Bio Generator | VI | 笔名可用的三版简介，不声称头衔 |
| 24 | A+ Content Architect | VI | 5 模块 A+ 版式 |
| 25 | Launch Playbook Generator | VII | 上市 14 天逐日作战手册 |
| 26 | Review Request System | VII | 100% 合规的评论征集 + ARC 序列 |
| 27 | Promotion Site Submitter | VII | 5 个促销站的定制提交文案 |
| 28 | Keyword Arsenal Builder | VIII | 30+30+15+5+20 的广告关键词弹药库 |
| 29 | Campaign Architect | VIII | 四活动 + 20/40/25/15 预算配比 |
| 30 | ACOS Optimisation Analyst | VIII | 盈亏平衡 ACOS + 赢家/输家/机会词 |
| 31 | International Ads Launcher | VIII | 把美国打法搬到英德法西意日 |
| 32 | Series Strategy Planner | IX | Book 2–5 的系列分工架构 |
| 33 | Translation Brief | IX | 出海翻译与本地化简报（7 项） |
| 34 | Portfolio Performance Analyst | IX | 书柜级体检 + 90 天 30% 增长计划 |
| 35 | Content Repurposing Engine | X | 一本书 → 30 天跨平台内容日历 |
| 36 | Social Proof Amplifier | X | 把真实评论变成 5 类营销资产 |
