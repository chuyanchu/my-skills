# Paper Reader Mapping

Use this reference when converting `$agent-paper-reader` output into PPT slides.

## Single Paper Mapping

```text
Reading Assumption -> speaker notes or title subtitle
Problem -> Problem slide
Gap in Existing Methods -> Motivation slide
Proposed Method -> Method overview slide
Agent loop -> Architecture/flow slide
Advantages and Evidence -> Evidence slide
Limitations and Hidden Assumptions -> Limitations slide
What We Can Do Next -> Follow-up experiment slide
Bottom Line -> Takeaway or closing slide
```

## Multi-Paper Mapping

```text
Comparison Assumption -> title subtitle or source note
One-Line Verdict for Each Paper -> paper map slide
Shared Research Problem -> cluster motivation slide
Method Difference Table -> method comparison slide
Evidence and Evaluation Comparison -> evaluation audit slide
Complementarity and Conflict -> synthesis slide
Research Gaps -> gap slide
Next Actions -> next reading/reproduction slide
Bottom Line -> closing slide
```

## Compression Rules

- Convert paragraphs into claims.
- Keep only what a listener must remember.
- Move caveats into limitations, not every slide.
- If a bullet contains "and", "but", or three commas, consider splitting it.
- If a slide needs more than 5 bullets, split it into two slides.
- If the source has uncertain evidence, write "尚未证明" or "证据不足" instead of overclaiming.

## Example Transformation

Source:

```text
The paper proposes a multi-agent framework where a planner decomposes tasks and multiple worker agents execute subtasks with tool calls. The paper reports improvement on benchmark X but does not control for number of calls.
```

Slide:

```text
方法：Planner-Worker 多智能体框架

• Planner 将任务拆成子任务
• Worker agents 调用工具完成局部任务
• 核心收益：并行化与角色分工
• 关键疑问：是否控制了调用次数和成本？
```

## Discussion Slide Prompts

Use 2-4 prompts:

- 这个方法的真实贡献是机制，还是工程编排？
- 如果固定 token/tool budget，多 agent 还会更好吗？
- 哪个模块最值得复现？
- 哪个失败模式最可能出现在我们的系统里？
