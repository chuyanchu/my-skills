# PPTX QA

Use this checklist before delivering a deck.

## Content QA

- Every slide has a clear claim or function.
- No paper claim, metric, venue, or year is invented.
- Technical terms are consistent across slides.
- Limitations are not hidden in speaker notes only.
- Follow-up ideas are feasible and testable.
- Citations or paper names are present where needed.

## Visual QA

- Title position and color are consistent.
- Body text is readable and not below 16 pt.
- No text overlaps, clipping, or overflow.
- Bullets fit within the content area.
- Tables are readable; if not, split or simplify.
- No red spell-check underlines, placeholder text, or broken glyphs.
- No decorative cards, gradients, or irrelevant images.
- If all slide elements appear near the top-left corner, the deck failed positioning. Rebuild with the Presentations `createSlideContext` helpers instead of raw compose positioning.

## Minimal Style QA

At contact-sheet size, the deck should look like:

- White pages.
- Strong dark-blue headings.
- Clean black academic notes.
- Distinct but restrained slide rhythms.
- No visual noise.

## Delivery QA

For actual PPTX creation:

- Render previews.
- Inspect at least the title slide, densest slide, table slide, and final slide.
- Iterate any slide with overflow or unreadable text.
- Export editable PPTX after visual checks pass.
