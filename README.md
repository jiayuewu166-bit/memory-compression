# memory-compression
Answer to ai-engineer-challenge_question B
0.Overview

1.Problem Understanding
压缩是一种“决策保真”（decision-preserving）的过程，而不是单纯摘要。

2.Information Taxonomy & Prioritization
2.1 Information Categories
Goals（用户目标）
Constraints & Preferences（条件限制/偏好）
Key Facts（关键事实、数字、人物、决定）
Decisions（已确认的决定）
Action Items（待办任务）
2.2 Non-essential Information

3.Compression Strategy
3.1System Overview
Extraction → Aggregation → Semantic Compression → Token Check
3.2Structured Information Extraction结构化信息提取
分类每轮对话内容 提取内容并写入 5 类容器 避免早期丢失信息
3.3Aggregation & Deduplication
合并同义、重复、冗余的信息  对于冲突信息保留最新版本 对于长篇内容提取核心语义（什么技术呢？）
3.4Semantic Compression语义压缩
3.5Token Constraint Handling保留优先级
3.6Safety Hallucination Prevention
不新增事实  不推测对话中不存在的信息  “保留原话”中的关键字段

4.Evaluation Framework
4.1Q & A Consistency Test
4.2Fact coverage Analysis
4.3Decision Usefulness Test
4.4Token Efficiency

5.Example
6.Edge Cases

7.Limitations
8.Future Improvements

9.Implementation Notes
