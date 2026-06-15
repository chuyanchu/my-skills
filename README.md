# 我的 Codex Skills

[English README](README_EN.md)

这是一个用于沉淀个人高频工作流的 Codex skills 仓库，覆盖科研阅读、课程项目、PPT 生产和项目交付。

当前包含两类 skill：一类是我已经真实使用过的稳定 skill，另一类是从历史重复流程里抽象出来、还需要真实任务继续打磨的实验性 skill。

- `agent-paper-reader`（Stable）：把 AI agent 论文读成研究判断，而不是普通摘要。
- `minimal-paper-ppt`（Stable）：把论文阅读笔记整理成干净、可编辑的极简学术 PPT。
- `notebooklm-ppt-producer`（Experimental）：为 NotebookLM/Gamma 这类工具准备资料索引、批次规划和分批生成 prompt。
- `course-data-analysis-packager`（Experimental）：为课程数据分析项目生成可复现交付包，包括数据字典、脚本、图表、报告模板和 PPT 提纲。
- `project-delivery-packager`（Experimental）：为项目交付整理 README、部署文档、API 说明、测试命令、交付清单和验收 checklist。

默认输出风格偏中文科研/课程工作流；论文标题、方法名、benchmark、数据集、技术术语等保留英文会更清楚时，不强行翻译。

## 为什么值得 Star

如果你也想把重复工作流固化成 Codex skill，这个仓库可以直接复用或改造：

- 阅读 AI agent、LLM agent、tool-use、planning、memory、multi-agent、RAG-agent、web-agent、GUI-agent、coding-agent 或 agent benchmark 论文；
- 从论文里提取问题定义、方法机制、证据质量、局限和后续研究方向；
- 把论文阅读笔记整理成简洁、白底、可编辑的学术 PPT；
- 把杂乱资料整理成 NotebookLM/Gamma 可用的分批 PPT 生成 prompt；
- 把课程数据分析项目整理成可复现、可展示、可交付的结构；
- 为客户、课程或内部项目补齐交付文档，避免每次从零写 README、部署说明和验收清单。

## Skill 列表

| Skill | 状态 | 用途 | 最适合的输入 |
| --- | --- | --- | --- |
| `agent-paper-reader` | Stable | 论文精读、批判、对比、复现思考和研究扩展 | Paper PDF、LaTeX、提取文本、阅读笔记、论文列表 |
| `minimal-paper-ppt` | Stable | 从论文笔记生成极简学术 PPT 大纲或 PPTX | `agent-paper-reader` 输出、论文笔记、实验想法、复现计划 |
| `notebooklm-ppt-producer` | Experimental | NotebookLM/Gamma 分批生成 PPT 的 prompt package | 行业报告、课程材料、政策材料、研究笔记、混合资料 |
| `course-data-analysis-packager` | Experimental | 课程/小组作业的数据分析交付包 | 课程题目、作业 rubric、CSV/Excel、notebook、分析脚本 |
| `project-delivery-packager` | Experimental | 项目交付、部署、验收和 handoff 材料 | 现有 repo、部署目录、API、数据管线、RAG/知识库项目 |

实验性 skill 应按 beta 工作流使用：先让它生成 plan、audit 或小范围初稿，再在真实任务中逐步修正。

## 示例用法

### 1. 阅读 AI Agent 论文

```text
用 agent-paper-reader 详细解读这篇 agent benchmark 论文，重点看：
1. 它解决什么评测问题
2. agent loop 怎么定义
3. 指标是否可信
4. 复现风险在哪里
5. 我们可以基于它做什么新实验
```

### 2. 对比多篇论文

```text
用 agent-paper-reader 比较这 4 篇 tool-use agent 论文。
请按 problem setting、memory/planning/tool-use 机制、evaluation credibility、
limitations、可复现性和后续研究机会组织。
```

### 3. 把论文笔记转成 PPT

```text
用 minimal-paper-ppt 把上面的论文解读整理成 12 页中文组会 PPT。
风格保持极简学术：白底、深蓝大标题、黑色小节标题、短 bullet，
不要装饰性图形，不要拥挤。
```

### 4. 生成 NotebookLM PPT 分批 Prompt

```text
用 notebooklm-ppt-producer 把这些行业报告和课程材料整理成 60 页 PPT 的
NotebookLM 分批生成提示词。请给出上传材料索引、故事主线、批次规划、
每批 prompt 和合并检查清单。
```

### 5. 整理课程数据分析交付包

```text
用 course-data-analysis-packager 把这个课程数据集整理成可交付包：
README、data dictionary、分析脚本、输出图表、报告模板和 PPT 提纲。
```

### 6. 准备项目交付包

```text
用 project-delivery-packager 检查这个项目是否可以交付，
补齐 README、部署步骤、API 文档、测试命令、交付清单和验收 checklist。
```

## 安装

克隆仓库后，只复制你需要的 skill 目录到 Codex skills 目录即可，不需要全部安装：

```bash
git clone https://github.com/chuyanchu/my-skills.git
mkdir -p ~/.codex/skills
```

安装单个 skill：

```bash
cp -R my-skills/agent-paper-reader ~/.codex/skills/
```

安装多个 skill：

```bash
cp -R my-skills/agent-paper-reader ~/.codex/skills/
cp -R my-skills/minimal-paper-ppt ~/.codex/skills/
```

安装全部 skill：

```bash
cp -R my-skills/agent-paper-reader ~/.codex/skills/
cp -R my-skills/minimal-paper-ppt ~/.codex/skills/
cp -R my-skills/notebooklm-ppt-producer ~/.codex/skills/
cp -R my-skills/course-data-analysis-packager ~/.codex/skills/
cp -R my-skills/project-delivery-packager ~/.codex/skills/
```

可用的 `<skill-name>` 见上方 Skill 列表。

然后重启 Codex 或重新加载 skills。

## 仓库结构

```text
agent-paper-reader/
  SKILL.md
  agents/
  references/

minimal-paper-ppt/
  SKILL.md
  agents/
  references/

notebooklm-ppt-producer/
  SKILL.md
  agents/
  references/

course-data-analysis-packager/
  SKILL.md
  agents/
  references/

project-delivery-packager/
  SKILL.md
  agents/
  references/
```

每个 skill 的主流程放在 `SKILL.md`，更细的模板、检查清单和参考材料放在 `references/`。

## 维护约定

新增或修改 skill 时，同一个 commit 里同步更新：

- `README.md`：中文说明
- `README_EN.md`：英文说明

实验性 skill 只有在真实任务中使用并确认流程稳定后，才应改为 `Stable`。

## 设计原则

- 重视研究判断，而不是泛泛总结。
- 解释 agent 论文时优先拆 mechanism 和 agent loop。
- 关注证据边界：claim、实验、消融、未证明内容要分清。
- 支持中文科研/课程工作流，同时保留必要英文技术术语。
- PPT 保持可编辑、可讨论、可复用，不追求装饰性。
- 交付包要有清晰的输入、输出、命令和 QA。
- 对外分享时注意脱敏，避免泄露密钥、客户数据或私有路径。

## 贡献

欢迎提 issue 或 pull request，尤其是：

- 新的 agent 论文阅读模板；
- 更强的评测和复现检查清单；
- 多论文对比结构；
- 学术 PPT deck blueprint；
- NotebookLM/Gamma PPT 生产流程；
- 课程数据分析交付包模板；
- 项目交付和验收 checklist。

## License

MIT License. See [LICENSE](LICENSE).
