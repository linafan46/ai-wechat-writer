# 长文封面与文中配图

## 输出组成

每篇长文默认提供：

- 1 张封面图：用于微信公众号头图。
- 2～3 张文中配图：对应正文关键解释段落。
- 每张图都要给出用途、画面说明和可复用生成提示词。

用户要求实际生成图片时，优先使用 imagegen。若图像生成不可用，交付完整提示词，不要用低质量占位图冒充最终效果。

## 封面风格

默认沿用账号既有的暖白极简 3D 视觉：

- 横版宽画幅，适合微信公众号封面。
- 主体居中，大量留白。
- 使用象牙白、奶油白、浅米色、香槟金和柔和灰。
- 材质可用磨砂塑料、石膏、陶瓷、半透明玻璃。
- 背景可有低透明度英文词，例如 `CONTEXT`、`SYSTEM`、`THINKING`。
- 避免机器人、科技蓝、霓虹、电路板、复杂文字和品牌标志。

## 文中配图风格

文中配图可以比封面更有解释性，优先选择两类风格：

1. **暖白极简 3D 概念图**：适合承接账号原有视觉识别。
2. **点阵半调高级插画**：适合解释历史类比、系统关系或对比结构。

点阵半调风格规则：

- 简约高级，像杂志信息插画，不像漫画。
- 可以使用撞色，但颜色数量控制在 2～3 个。
- 推荐色：暖米白 `#F6F0E7`、深黑 `#151515`、番茄红 `#E34A35`、深蓝 `#174EA6`、香槟金 `#B9945A`。
- 使用清晰构图，少文字，少元素。
- 适合表现“旧流程 vs 新系统”“临时外包 vs 工作现场”“电力进入工厂”等逻辑。

## 配图选择方法

围绕文章结构选图：

- 开头场景图：表现读者的真实痛点，例如反复向 AI 介绍自己。
- 方法解释图：表现实操方法，例如背景、目标、案例汇入一个上下文档案。
- 对比图：表现错误问法和更好问法的差异，例如临时提问 vs 带上下文提问。
- 类比图：表现工厂、电力、旧流程和新系统等解释性类比。

不要为每个段落配图。图片要放在读者最需要理解的地方，并在正文对应位置插入图片提示，不要只在文末统一列出。

## 图片提示词模板

封面图：

```text
Use case: WeChat article cover.
Create a premium minimalist 3D editorial concept image about [核心观点].
Show [核心视觉隐喻] as the single central subject.
Wide horizontal composition, large negative space, centered subject.
Warm ivory and cream background, subtle champagne gold accents, soft studio lighting, gentle floating shadow.
Low-opacity background word: "[英文概念词]".
No robots, no tech blue, no neon, no circuit boards, no brand logos, no dense text.
```

文中点阵半调图：

```text
Use case: in-article editorial illustration.
Create a minimalist halftone editorial illustration about [解释段落].
Show [具体画面] with a clean magazine-like composition.
Style: premium minimalist halftone dots, sharp shapes, elegant negative space.
Palette: warm cream background, deep black linework, tomato red and deep blue contrast accents.
No cartoon characters, no clutter, no neon, no robot, no circuit board, no dense text.
```
