# Batching Patterns

Use batching whenever a deck is too large for one reliable generation pass or when the source material is mixed.

## Recommended Batch Sizes

| Deck type | Batch size | Notes |
| --- | --- | --- |
| Lecture or course deck | 10-15 slides | Keep teaching rhythm inside each batch. |
| Academic report | 8-12 slides | Preserve claim/evidence mapping. |
| Executive or design-sensitive deck | 5-8 slides | Keep layout and wording tightly controlled. |
| Long workshop deck | 12-20 slides | Use recap and transition slides between modules. |

## Common Batch Schemes

### Report Deck

1. Context and problem
2. Evidence and trend analysis
3. Framework or method
4. Cases or applications
5. Implications and recommendations

### Course Deck

1. Learning goals and opening case
2. Core concepts
3. Method or tool walkthrough
4. Example and exercise
5. Summary and assignment

### Technical Project Deck

1. Problem and constraints
2. Architecture and data flow
3. Core modules
4. Demo and evaluation
5. Deployment and next steps

## Batch Boundary Rules

- Do not split one logical framework across multiple batches unless the second batch repeats a short context line.
- Each batch prompt must say what previous batches already covered.
- Include target slide numbers so final merge is deterministic.
- Reserve one final integration batch for agenda, transitions, appendix, and duplicated-slide cleanup when needed.
