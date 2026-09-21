# yd-academic-ppt

一个用于创建、重设计和迭代打磨高质量演示文稿的 Codex Skill。它适用于学术汇报、论文解读、答辩、课程教学、技术报告、政策汇报，也支持黑客松、创业路演、产品发布和创意提案。

核心思路是：**先锁定叙事，再比较三套完整视觉方案，最后制作并验证 PPTX / PDF**。它不会把文档机械地切成一页页文字，也不会在没有用户选择的情况下直接套模板。

## 实际效果

下面是一次真实的“三方向视觉提案”输出：相同内容保持不变，同时给出官方模板融合、星际黑客松和山野晨光三种完整视觉系统。

![三套视觉方向对比](./docs/preview/three-concepts.png)

## 能做什么

- 从论文、报告、数据、讲稿或零散笔记中提炼一条可讲清楚的论证主线。
- 根据演讲时长规划页数和节奏，默认约为 3 分钟 8 页、5 分钟 12 页、10 分钟 20 页。
- 在同一份 Story Lock 上生成 A / B / C 三套完整全稿视觉预览。
- 为学术内容建立证据链、结论式标题、方法图、公式、图表、表格和局限讨论。
- 将选中的学术视觉方向重建为高保真、可编辑的 PowerPoint 对象。
- 将高冲击创意方向以完整页面视觉装配进 PPTX，保留舞台表现力。
- 输出匹配的 PPTX 和 PDF，并执行溢出、可读性、引用和一致性检查。
- 在 V1 后提出针对性问题，再交付经过系统修改的 V2。

## 三种模式

| 模式 | 适用场景 | 最终形式 |
| --- | --- | --- |
| 学术编辑模式 | 论文汇报、答辩、教学、研究、正式报告 | 原生可编辑文字、表格、图表、公式和简单图形 |
| 创意路演模式 | 黑客松、创业、游戏、文化产品、品牌提案 | 默认保留选中全页视觉，追求统一和冲击力 |
| 海报冲击模式 | 发布会、宣传型路演、强艺术字与密集视觉 | 以完整 16:9 页面图像为主，强调舞台效果 |

## 标准工作流

```text
输入论文 / 数据 / 需求
        ↓
确认受众、时长、证据要求与可编辑性
        ↓
锁定大纲、页序、结论标题和 Story Lock
        ↓
生成 A / B / C 三套全稿 Contact Sheet
        ↓
用户选择一种方向或明确混合规则
        ↓
制作 PPTX → 导出 PDF → 全页渲染 QA
        ↓
交付 V1 → 定向提问 → 全局修订 → 交付 V2
```

三个概念必须使用同一份故事线和页面顺序，差异只体现在视觉系统、版式语法和图像方向，避免“为了换风格把内容也换掉”。

## 安装

仓库中的可安装 Skill 位于 `yd-academic-ppt/` 子目录。

```bash
git clone https://github.com/xingchenyd/yd-academic-ppt.git
```

将子目录复制到 Codex Skills 目录：

```text
yd-academic-ppt/yd-academic-ppt/
            ↓
~/.codex/skills/yd-academic-ppt/
```

安装完成后，目标目录中应直接包含 `SKILL.md`、`agents/` 和 `references/`。

## 使用示例

### 学术汇报

```text
使用 yd-academic-ppt，把这四篇论文做成一份 15 分钟中文学术汇报。
先锁定大纲，再给我三套完整全稿视觉方向；我选择后制作高保真可编辑 PPTX，
导出 PDF，并在 V1 后向我提出针对性修改问题。
```

### 答辩

```text
使用 yd-academic-ppt，把我的论文和实验数据制作成 10 分钟答辩。
重点突出研究问题、方法贡献、关键结果、对比实验、局限与下一步。
```

### 创意路演

```text
使用 yd-academic-ppt，为这个环保游戏制作 5 分钟黑客松路演。
需要海报级视觉冲击、清楚的商业与社会价值、真实产品截图和最终 PPTX / PDF。
```

## 默认学术视觉系统

- 暖白底色，深海军蓝作为结构色，克制的暗红色负责结论与对比。
- 大号中文衬线标题、编号标记、短粗红色下划线。
- 稳定的顶部 / 底部导航框架、圆角卡片和紧凑编辑式表格。
- 正文使用清晰的中文无衬线字体，避免低对比灰字和大段堆字。
- 每页只承担一个任务，并使用结论式标题让标题序列本身形成演讲提纲。
- 图表必须包含单位、标签、来源和明确 takeaway，不允许伪造数据或引用。

## 质量门槛

- 不允许文字裁切、重叠、越界或小到无法投影阅读。
- 不允许未解决占位符、水印、模板残留和错误机构品牌。
- 不允许无来源事实、虚构数字、虚构引用或未标注推断。
- 学术模式中，可原生重建的文字、表格、图表、公式和简单图形不能只用截图代替。
- PPTX 与 PDF 必须逐页比对，确认导出后没有字体、布局或图像变化。
- 交付前必须检查全页渲染、缩略图节奏、内容密度和引用完整性。

## 输出文件

在视觉选择前：

```text
<topic>_outline.txt
<topic>_concept_A_contactsheet.png
<topic>_concept_B_contactsheet.png
<topic>_concept_C_contactsheet.png
```

正式交付：

```text
<topic>_YD_V1.pptx
<topic>_YD_V1_preview.pdf
<topic>_YD_V2.pptx
<topic>_YD_V2_preview.pdf
```

## 目录结构

```text
yd-academic-ppt/
├── README.md
├── docs/preview/three-concepts.png
└── yd-academic-ppt/
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
        ├── workflow.md
        ├── three-concept-preview.md
        ├── image-to-editable-reconstruction.md
        ├── design-system.md
        ├── academic-template-fidelity.md
        ├── layout-grammar.md
        ├── pitch-visual-systems.md
        ├── poster-impact-mode.md
        ├── evidence-and-research.md
        ├── duration-and-scenarios.md
        ├── intake-and-iteration.md
        ├── visual-generation-policy.md
        └── qa-rubric.md
```

## 设计边界

原始参考截图不随仓库发布，避免保留来源水印或品牌。Skill 保存的是从参考中提炼出的布局语法、视觉 token、制作流程和验证标准。所有事实、图表、论文插图、产品截图与 Logo 都必须来自真实来源或用户提供的材料，不能用生成内容冒充证据。
