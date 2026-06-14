# Analysis Workflow

## Question Design

A good course analysis question should be:

- answerable with the available data;
- narrow enough for a course presentation;
- connected to comparison, ranking, segmentation, trend, relationship, or risk;
- honest about sampling and missing data.

Examples:

- Compare consumer attention topics across cities.
- Identify risk groups from weak behavioral signals.
- Summarize platform differences in review text.
- Explain which factors correlate with score or price.

## Script Stages

1. `extract_*`: convert teacher/source files into raw CSV when needed.
2. `clean_*`: normalize columns, missing values, text, dates, and categories.
3. `analyze_*`: compute tables, metrics, and summaries.
4. `visualize_*`: produce PPT-ready figures.

For small packages, combine stages into one script only when the flow remains readable.

## Chart Selection

- Count/ranking: bar chart.
- Distribution: histogram or box plot.
- Two numeric variables: scatter plot.
- Category vs metric: grouped bar chart.
- Text topics: topic frequency bar chart or table.
- Time trend: line chart, only when date coverage is reliable.

## Claim Discipline

- Use "shows", "suggests", or "is associated with" for descriptive evidence.
- Avoid "causes" unless the assignment explicitly supports causal analysis.
- Report missing values and sample bias.
- Keep every PPT conclusion tied to a table or figure.
