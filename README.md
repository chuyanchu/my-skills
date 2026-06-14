# My Codex Skills

Practical Codex skills for AI agent paper reading and minimalist academic presentation decks.

This repository currently includes two skills designed to work together:

- `agent-paper-reader`: turn AI agent papers into research judgment, not just summaries.
- `minimal-paper-ppt`: turn paper-reading notes into clean, editable academic PowerPoint decks.

The default output style is Chinese-first for Chinese research workflows, while preserving English paper titles, method names, benchmark names, and technical terms where that is clearer.

## Why Star This Repo

Star this repository if you want reusable Codex skills for:

- reading AI agent, LLM agent, tool-use, planning, memory, multi-agent, RAG-agent, web-agent, GUI-agent, coding-agent, or agent benchmark papers;
- extracting the actual problem framing, method mechanism, evidence quality, limitations, and follow-up research ideas;
- turning paper-reading notes into concise, editable, white-background academic PPTX decks;
- building a repeatable paper-reading and seminar workflow instead of rewriting prompts from scratch.

## Included Skills

| Skill | Use it for | Best input |
| --- | --- | --- |
| `agent-paper-reader` | Detailed paper explanation, critique, comparison, reproduction thinking, and research extension ideas | Paper PDF, LaTeX, extracted text, notes, or a paper list |
| `minimal-paper-ppt` | Minimal academic slide outlines or PPTX decks from paper-reading notes | Output from `agent-paper-reader`, paper notes, experiment ideas, or reproduction plans |

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

## Installation

Clone this repository and copy the skill folders into your Codex skills directory:

```bash
git clone https://github.com/chuyanchu/my-skills.git
mkdir -p ~/.codex/skills
cp -R my-skills/agent-paper-reader ~/.codex/skills/
cp -R my-skills/minimal-paper-ppt ~/.codex/skills/
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
```

Each skill keeps the main behavior in `SKILL.md` and task-specific guidance in `references/`.

## Design Principles

- Research judgment over generic summarization.
- Mechanism-first explanations for agent papers.
- Evidence-aware reading: claims, experiments, ablations, and what remains unproven.
- Chinese academic workflow support without losing precise English technical terms.
- Minimal slides that remain editable and readable in real group meetings.

## Contributing

Issues and pull requests are welcome, especially for:

- new agent paper-reading templates;
- stronger evaluation and reproducibility checklists;
- better multi-paper comparison structures;
- academic PPT deck blueprints;
- examples from real reading-group workflows.
