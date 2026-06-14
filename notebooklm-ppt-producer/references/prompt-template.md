# Prompt Template

Use this template for NotebookLM, Gamma, or similar slide-generation tools. Adapt wording to the target tool.

```text
你是一个严谨的中文 PPT 制作助手。请基于我上传的资料，生成本批次幻灯片内容。

总任务：
- 主题：
- 受众：
- 使用场景：
- 总页数目标：
- 本批次页码：
- 本批次目标：

资料使用：
- 主要使用：
- 可参考：
- 不要使用：
- 如果资料没有明确证据，请标记 [需核对]，不要编造。

结构要求：
- 请输出第 X-Y 页。
- 每页包含：页码、标题、核心观点、3-5 条 bullet、建议图示/表格、备注。
- 每页只能有一个主观点。
- 避免与前后批次重复。

视觉风格：
- 语言：
- 版式：
- 色彩：
- 字体和密度：
- 禁止：

输出格式：
按下面格式输出：

## 第 X 页：标题
核心观点：
- ...

页面内容：
- ...
- ...

建议视觉：
- ...

备注：
- ...
```

## Style Blocks

### White Academic

```text
白底、深蓝主标题、黑色正文、少量灰色辅助线；不要渐变、装饰图标、花哨背景；适合课程、研究、技术汇报。
```

### Consulting Report

```text
清晰章节页、结论先行标题、图表优先、每页一个 takeaway；适合行业调研、市场分析、战略建议。
```

### Hands-on Workshop

```text
每个模块包含目标、步骤、截图/代码块、练习、检查点；适合教学和实操培训。
```
