---
name: ai-wechat-writer
description: Use when creating Chinese WeChat public account articles about recent AI news, AI knowledge, technology trends, personal growth, or aesthetic judgment, especially when the user wants a concise shareable viewpoint article and a matching cover image.
---

# AI 热点公众号创作

## Overview

把近期 AI 热点、审美或个人成长话题，转化为一篇只讲一个观点的微信公众号短文，并生成统一的标题摘要和暖白极简 3D 封面。

## Workflow

1. 确认用户给定的主题；未给定时，从 AI、Agent、AI+审美、AI+个人成长、审美判断、个人成长等方向随机选择一个可写入口。
2. 如果选择近期热点，优先使用官方发布、产品博客、研究论文等一手来源核实事实。区分已确认事实与个人推断。
3. 从热点、产品细节、生活观察或可验证事实入口中寻找普通人能理解的能力、工作或成长启发。不要写新闻汇总。
4. 只选择一个最清晰的观点，并用一句话表达。无法一句话表达时，继续收窄。
5. 按 `references/writing-style.md` 写文章。
6. 按 `references/visual-style.md` 设计单一视觉隐喻。用户需要图片时，使用 imagegen 生成封面。
7. 交付标题、25 字以内摘要、正文、封面图、封面提示词和事实来源链接。

## Topic Selection

优先选择具备至少一项特征的话题：

- 与 AI 直接相关，或能自然延伸到 AI 时代的工作、审美、判断力和个人成长
- 能与普通人的工作、成长或生活产生关系
- 能形成简单、清晰的类比
- 能从产品变化中提炼能力启发
- 能形成一句有判断力的结论
- 不需要大量背景知识也能读懂

主题优先级：AI 热点 > AI+个人成长 > AI+审美 > Agent/Token/Skill 等通俗类比 > 审美或个人成长。允许不直接结合 AI，但必须符合账号气质：克制、有判断、有启发。

避免直接选择纯参数对比、复杂技术教程、没有观点的新闻汇总、泛泛鸡汤或需要大量论证的行业分析。

## Output Requirements

- 正文只表达一个核心观点，通常控制在 150～500 字。
- 每次只生成一篇。批量产出节奏由外部自动化控制，不写进 skill 规则。
- 标题下方必须生成一句摘要，尽量不超过 25 个汉字。
- 使用短句、克制换行和重点加粗，语气直白、有判断，不写成鸡汤。
- 热点只做入口，个人能力、工作方式或成长判断才是落点。
- 结尾必须有一句可独立传播的总结。
- 封面必须与正文使用同一个核心隐喻，不直接复述完整标题。
- 对时效性事实提供来源链接，不虚构发布日期、产品能力或引用。

## Quality Check

交付前检查：

- 删除与核心观点无关的第二个观点。
- 删除空泛鼓励、夸张预测和不必要的专业术语。
- 确认文章不是换行后的新闻摘要。
- 确认连续问句、并列清单和递进短句没有被空行拆散。
- 确认核心判断句已用 `**加粗**` 标出，但全文不要过度加粗。
- 确认摘要不超过 25 字左右，不是标题复读，也不是正文长句硬摘。
- 确认封面没有科技蓝、霓虹、电路、机器人或密集文字。
- 确认图片文字少且准确，主体一眼可懂。

## References

- 写作规则、标题公式和案例：`references/writing-style.md`
- 封面视觉规则、提示词模板和样例说明：`references/visual-style.md`
- 已确认的参考封面：`assets/reference-covers/`
