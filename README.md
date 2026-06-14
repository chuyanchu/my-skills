# My Codex Skills

Practical Codex skills for research, course projects, slide production, and project delivery workflows.

This repository collects my frequently used Codex skills. It currently includes skills for paper reading, academic slides, NotebookLM PPT production, course data-analysis packages, and project handoff packages:

- `agent-paper-reader`: turn AI agent papers into research judgment, not just summaries.
- `minimal-paper-ppt`: turn paper-reading notes into clean, editable academic PowerPoint decks.
- `notebooklm-ppt-producer`: prepare source indexes, batch plans, and prompts for NotebookLM-style slide generation.
- `course-data-analysis-packager`: build reproducible course data-analysis deliverables with data dictionaries, scripts, charts, reports, and PPT outlines.
- `project-delivery-packager`: assemble README files, deployment docs, API notes, test commands, inventories, and acceptance checklists for handoff.

The default output style is Chinese-first for Chinese research workflows, while preserving English paper titles, method names, benchmark names, and technical terms where that is clearer.

## Why Star This Repo

Star this repository if you want reusable Codex skills for:

- reading AI agent, LLM agent, tool-use, planning, memory, multi-agent, RAG-agent, web-agent, GUI-agent, coding-agent, or agent benchmark papers;
- extracting the actual problem framing, method mechanism, evidence quality, limitations, and follow-up research ideas;
- turning paper-reading notes into concise, editable, white-background academic PPTX decks;
- producing structured NotebookLM/Gamma PPT prompts from messy source materials;
- packaging course analysis projects so they are reproducible and presentation-ready;
- preparing client, class, or internal project handoff materials without rebuilding docs from scratch.

## Included Skills

| Skill | Use it for | Best input |
| --- | --- | --- |
| `agent-paper-reader` | Detailed paper explanation, critique, comparison, reproduction thinking, and research extension ideas | Paper PDF, LaTeX, extracted text, notes, or a paper list |
| `minimal-paper-ppt` | Minimal academic slide outlines or PPTX decks from paper-reading notes | Output from `agent-paper-reader`, paper notes, experiment ideas, or reproduction plans |
| `notebooklm-ppt-producer` | Batched NotebookLM/Gamma slide-generation prompts and production packages | Reports, lecture materials, policy notes, research notes, mixed source documents |
| `course-data-analysis-packager` | Reproducible class-project data analysis packages | Course topic, assignment rubric, CSV/Excel files, notebooks, analysis scripts |
| `project-delivery-packager` | Handoff-ready project delivery and acceptance packs | Existing repos, deployment folders, APIs, data pipelines, RAG/knowledge-base projects |

More skills may be added over time as reusable workflows become stable enough to share.

## Example Workflows

### 1. Read an AI Agent Paper

```text
用 agent-paper-reader 详细解读这篇 agent benchmark 论文，重点看：
1. 它解决什么评测问题
2. agent loop 怎么定义
3. 指标是否可信
4. 复现风险在哪里
5. 我们可以基于它做什么新实验
```

### 2. Compare Multiple Papers

```text
用 agent-paper-reader 比较这 4 篇 tool-use agent 论文。
请按 problem setting、memory/planning/tool-use 机制、evaluation credibility、
limitations、可复现性和后续研究机会组织。
```

### 3. Turn Notes Into Slides

```text
用 minimal-paper-ppt 把上面的论文解读整理成 12 页中文组会 PPT。
风格保持极简学术：白底、深蓝大标题、黑色小节标题、短 bullet，
不要装饰性图形，不要拥挤。
```

### 4. Produce NotebookLM PPT Batches

```text
用 notebooklm-ppt-producer 把这些行业报告和课程材料整理成 60 页 PPT 的
NotebookLM 分批生成提示词。请给出上传材料索引、故事主线、批次规划、
每批 prompt 和合并检查清单。
```

### 5. Package A Course Data Project

```text
用 course-data-analysis-packager 把这个课程数据集整理成可交付包：
README、data dictionary、分析脚本、输出图表、报告模板和 PPT 提纲。
```

### 6. Prepare A Project Delivery Package

```text
用 project-delivery-packager 检查这个项目是否可以交付，
补齐 README、部署步骤、API 文档、测试命令、交付清单和验收 checklist。
```

## Installation

Clone this repository and copy the skill folders into your Codex skills directory:

```bash
git clone https://github.com/chuyanchu/my-skills.git
mkdir -p ~/.codex/skills
cp -R my-skills/agent-paper-reader ~/.codex/skills/
cp -R my-skills/minimal-paper-ppt ~/.codex/skills/
cp -R my-skills/notebooklm-ppt-producer ~/.codex/skills/
cp -R my-skills/course-data-analysis-packager ~/.codex/skills/
cp -R my-skills/project-delivery-packager ~/.codex/skills/
```

Then restart Codex or reload your skills.

## Repository Layout

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

Each skill keeps the main behavior in `SKILL.md` and task-specific guidance in `references/`.

## Design Principles

- Research judgment over generic summarization.
- Mechanism-first explanations for agent papers.
- Evidence-aware reading: claims, experiments, ablations, and what remains unproven.
- Chinese academic workflow support without losing precise English technical terms.
- Minimal slides that remain editable and readable in real group meetings.
- Reproducible packages with explicit inputs, outputs, commands, and QA.
- Privacy-aware delivery workflows that avoid leaking secrets or client data.

## Contributing

Issues and pull requests are welcome, especially for:

- new agent paper-reading templates;
- stronger evaluation and reproducibility checklists;
- better multi-paper comparison structures;
- academic PPT deck blueprints;
- NotebookLM/Gamma slide-production workflows;
- course data-analysis package templates;
- project delivery and acceptance checklists.

## License

MIT License. See [LICENSE](LICENSE).
