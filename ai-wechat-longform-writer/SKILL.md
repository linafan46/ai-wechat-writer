---
name: ai-wechat-longform-writer
description: Use when creating Chinese WeChat public account longform articles about recent AI news, AI viewpoints, technology trends, AI plus personal growth, work methods, or aesthetic judgment, especially when the user wants a structured mid-to-long article with summary, cover image, and in-article image prompts.
---

# AI 公众号长文创作

## Overview

把近期 AI 热点、AI 观点、技术趋势或个人成长话题，转化为一篇有叙事、有类比、有观点推进的微信公众号中长文，并配套标题、摘要、黑底白字分割卡、封面图提示词和文中配图提示词。

这个 skill 与 `ai-wechat-writer` 分工明确：

- `ai-wechat-writer`：短观点文章，150～500 字，只讲一个传播点。
- `ai-wechat-longform-writer`：中长文，约 900～1800 字，用完整叙事解释一个趋势或判断。

## Workflow

1. 确认用户给定主题；未给定时，从最新 AI 热点、AI+工作方式、AI+个人成长、AI+审美、判断力和知识沉淀中选择一个入口。
2. 涉及时效性内容时，必须先浏览并核实最新事实。优先使用官方博客、产品发布、研究论文、权威机构文章等一手来源；明确区分事实与推断。
3. 只选择一个主观点，但允许用 1～2 个类比或案例解释它。热点不是正文主体，热点只是引出观点的证据。
4. 按 `references/longform-writing-style.md` 写正文。
5. 按 `references/longform-visual-style.md` 设计封面图和 2～4 张文中配图。用户需要实际图片时，优先使用 imagegen 生成；不可用时交付可直接复用的详细提示词，并说明未生成原因。
6. 交付标题、25 字以内摘要、正文、黑底白字分割卡文案、封面图或封面提示词、文中配图提示词、事实来源链接。

## Topic Selection

优先选择具备这些特征的话题：

- 最近几天或近期仍有讨论价值的 AI 事实、产品变化、研究观点或行业判断。
- 能映射到普通人的工作方式、认知方式、个人成长、审美或判断力。
- 能用一个直观类比讲清楚，例如工厂、电力、手机、地图、图书馆、助手、工作台。
- 适合展开成“场景 -> 问题 -> 事实信号 -> 类比解释 -> 行动启发 -> 结尾判断”的结构。

避免直接选择纯参数对比、复杂技术教程、没有观点的新闻汇总、泛泛鸡汤或需要大量行业背景才能读懂的话题。

## Output Requirements

- 正文通常 900～1800 字。用户要求更短时压到 700～1000 字，更长时再扩展。
- 标题要像一句判断，不要像新闻标题。
- 摘要放在标题下方，尽量不超过 25 个汉字。
- 开头必须从具体场景或真实困惑切入，不要直接抛概念。
- 段落要比短文更完整，不要把每句话都拆成独立段落。
- 保留少量有力短句，但只在关键判断处使用。
- 正文需要 2～5 个黑底白字分割卡，用作章节分割和逻辑路标。不要写“小结”。
- 必须有一个让普通人快速理解的类比或具体案例。
- 结尾必须回扣开头场景，并形成可独立传播的判断。
- 图片必须服务文章逻辑，不做装饰图。每张图说明它对应正文哪一段。

## Quality Check

交付前检查：

- 是否保留了一个清晰主观点，而不是写成 AI 新闻合集。
- 是否先有具体场景，再解释概念。
- 是否用一个直观类比降低理解成本。
- 是否删除了重复解释和啰嗦铺垫。
- 是否避免机械短句、过度空行和教程腔。
- 是否用黑底白字分割卡切开长文，而不是用“小结”或密集小标题。
- 是否给出摘要、封面提示词、文中配图提示词和事实来源。
- 涉及时效性事实时，是否已核实来源并给出链接。

## References

- 长文叙事与排版：`references/longform-writing-style.md`
- 长文封面与文中配图：`references/longform-visual-style.md`
