# 视频 12：Workflow of a data science project（数据科学项目工作流程）

整理日期：2026-11-06。依据公开英文字幕转录核对，中文归纳，非官方中文讲义或逐字字幕。

## 课程核心
吴恩达区分机器学习项目与数据科学项目：机器学习项目常交付模型或软件能力；数据科学项目常交付可行动洞见，帮助组织改变决策。数据科学项目不一定需要训练模型。

典型步骤：
1. 收集数据。
2. 分析数据，反复探索以获得洞见。
3. 提出假设和行动建议，实施改变，并定期重新分析新数据。

## 案例一：电商销售漏斗
顾客从访问网站、浏览商品、查看商品页、加入购物车到结账。团队收集页面访问、时间和地区等数据，分析用户在哪个环节流失。课程提出的可能解释包括国际运费、节假日购物习惯和不同地区的午休时段。这些只是待验证假设，不是数据本身已证明的原因。团队可以测试调整运费展示或广告时段，之后观察转化率、收入、利润和用户体验。

## 案例二：咖啡杯制造
生产包含混合黏土、塑形、上釉、烧制和质检。可以记录供应商、原料批次、混合时间、湿度、窑温、烧制时长和缺陷情况。数据团队分析哪些因素与裂纹或其他缺陷同时出现，提出调整生产参数的建议，再通过新数据检查良品率是否改善。相关性不自动等于因果关系，还要考虑原料、设备、人员、班次和季节等因素。

## 2026 年延伸学习
1. **从相关性走向因果验证**：运费高与弃单率高同时出现，不足以证明运费是原因。条件允许时使用随机分组的 A/B 测试；无法随机实验时，采用适当的因果推断设计并说明假设和局限。
2. **先定义指标**：预先确定主要指标、保护性指标、观察周期和统计口径。不要只挑选有利指标或把短期波动当成长期改善。
3. **数据治理**：记录数据来源、转换过程、访问权限和个人信息处理方式。NIST 差分隐私指南指出，涉及个人的数据分析有隐私风险，隐私增强技术需专业设计。
4. **生成式 AI 辅助分析**：大模型可协助拆解问题、草拟 SQL/Python、解释图表和提出假设，但可能写错查询或误读数据，必须核对数据口径、计算和来源。
5. **Agent 辅助分析**：可协助跨数据源整理信息，但业务关键操作应保留人工监督、最小权限和审批流程。先让 Agent 生成查询草稿和分析摘要，不直接让它修改生产数据或对外发布。

## 新旧方法对照
- 收集业务数据：今天还要做质量检查、来源追踪、权限和隐私治理。
- 反复分析找洞见：今天增加统计检验、因果推断和可复现流程。
- 提出行动：今天可用 A/B 测试或适当研究设计验证效果。
- 改变后复查：同时监控主要指标与利润、退款、投诉等保护性指标。

## 个人知识库应用
统计文件类型、目录、标签、更新时间和常见搜索问题；找出重复文件和检索失败类型；提出增加关键词索引等假设；先在一个分类小范围试验；用真实问题比较命中率、查找时间和误分类率。保留原文件和版本记录。

## 术语
- Data Science：利用数据、统计和领域知识发现规律并支持决策。
- Actionable Insights：能指导具体行动的分析结论。
- Sales Funnel：用户从接触到完成购买的一系列步骤。
- Hypothesis：可检验的解释或预测。
- A/B Test：比较不同方案效果的实验方法。
- Causal Inference：估计因果影响的方法。
- Data Lineage：数据来源、流转和转换记录。

## 复习题
1. 数据科学项目的典型交付物是什么？
2. 为什么销售漏斗需要反复分析？
3. 制造案例要收集哪些数据？
4. 为什么相关性不等于因果关系？
5. Agent 辅助分析为什么仍需人工核验？

## 来源
- Coursera 官方课程：https://www.coursera.org/learn/ai-for-everyone
- Filmot 英文字幕转录：https://filmot.com/sidebyside/cHNTwBrb-co/en/en/English/English/Lecture%2B2.3%2B%E2%80%94%2BWorkflow%2Bof%2Ba%2Bdata%2Bscience%2Bproject%2B%E2%80%94%2B%5BAI%2BFor%2BEveryone%2B%7C%2BAndrew%2BNg%5D
- Google Cloud Agentic analytics（2026-10-16 reviewed）：https://docs.cloud.google.com/architecture/agentic-ai-cross-cloud-analytics
- Google Cloud AI/ML operational excellence（2026-10-29 reviewed）：https://docs.cloud.google.com/architecture/framework/perspectives/ai-ml/operational-excellence
- Google Cloud AI/ML performance optimization：https://docs.cloud.google.com/architecture/framework/perspectives/ai-ml/performance-optimization
- NIST SP 800-226（2025-03）：https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-226.pdf

延伸资料检索日期：2026-11-06。中文内容为学习归纳，平台文档会持续更新。