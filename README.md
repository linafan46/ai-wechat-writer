# AI 热点公众号创作

一个用于生成中文微信公众号 AI 短观点文章与配套封面图的 Codex Skill。

它会从近期 AI 热点、AI 知识、技术趋势或个人成长话题中，提炼一个普通读者能够理解和传播的观点，并生成统一的暖白极简 3D 风格封面。

## 能做什么

- 浏览并核实近期 AI 热点，优先使用官方发布、产品博客和研究论文
- 把热点转化为个人能力、工作方式或成长判断，而不是新闻摘要
- 生成 150～500 字的微信公众号短观点文章
- 为标题下方生成一句 25 字以内的摘要
- 使用短句、克制换行、重点加粗、对比和类比增强传播力
- 生成与文章观点一致的暖白极简 3D 概念封面
- 提供事实来源链接和可复用的封面提示词

## 输出风格

文章只讲一个核心观点：

```text
热点只是入口。
人的能力、判断和成长，才是落点。
```

版式强调公众号阅读体验：连续问句和并列短句放在一起，不机械空行；核心判断、关键转折和结尾金句用少量加粗突出。

每篇文章还会生成一句标题下方摘要，用于公众号卡片展示，例如：

```text
最近的 Agent 趋势，正在发生重要变化
```

封面使用暖白、象牙白、香槟金等低饱和配色，强调单一视觉隐喻、大量留白和柔和棚拍光，避免常见的科技蓝、霓虹、电路和机器人形象。

![参考封面：Thinking](assets/reference-covers/reference-01.png)

![参考封面：AI 越懂你越有用](assets/reference-covers/reference-05.png)

## 安装

将仓库克隆到 Codex skills 目录：

```bash
git clone https://github.com/linafan46/ai-wechat-writer.git ~/.codex/skills/ai-wechat-writer
```

安装完成后，重启 Codex 让 Skill 生效。

## 使用

直接调用 Skill：

```text
使用 $ai-wechat-writer 根据最近的 AI 热点生成一篇微信公众号短观点文章和封面图。
```

也可以指定主题：

```text
使用 $ai-wechat-writer 写一篇关于 Agent 记忆能力的微信公众号文章，并生成配套封面。
```

```text
使用 $ai-wechat-writer 从个人成长角度写一篇关于 AI 时代判断力的短文。
```

## 输出内容

Skill 默认交付：

1. 文章标题
2. 标题下方摘要
3. 正文
4. 封面图
5. 封面生成提示词
6. 热点事实来源链接

## 目录结构

```text
ai-wechat-writer/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── assets/
│   └── reference-covers/
└── references/
    ├── visual-style.md
    └── writing-style.md
```

## 风格参考

- [写作风格与案例](references/writing-style.md)
- [封面视觉规则与提示词模板](references/visual-style.md)

## 适合的话题

- AI 产品或模型变化带来的工作启发
- Agent、Token、Skill 等概念的通俗类比
- AI 时代的个人成长、判断力和审美
- 能够形成一句清晰观点的技术趋势

不适合直接用于复杂技术教程、纯参数对比、无观点的新闻汇总或需要大量论证的行业报告。
