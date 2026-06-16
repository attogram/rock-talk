# #7: C 3

Metadata:
- State: closed
- Author: attogram
- Created: 2026-06-13T16:23:38Z

## Description
## Proposal: Formal evaluation of bidirectional Rock Talk training vs. one-sided compression

### Background
Found a related project, **Caveman** (github.com/JuliusBrussee/caveman), a Claude Code skill/plugin implementing a similar core idea to Rock Talk: stripping filler, hedging, and pleasantries from model *output* while preserving technical accuracy.

Key data points from Caveman's own benchmarks (real Claude API token counts):
- ~65% average output token reduction across 10 prompts (range 22–87%)
- Only affects output/response tokens, not reasoning/thinking tokens
- Cites a March 2026 paper, "Brevity Constraints Reverse Performance Hierarchies in Language Models," showing forced brevity improved accuracy by 26pp on some benchmarks

Caveman is essentially a working *implementation* of one half of the Rock Talk thesis (model-side compression). Rock Talk's principles could extend this to a **bidirectional** protocol — compressing/structuring both user input and model output.

### Hypothesis
A more formal Rock Talk protocol that includes **training the user** on the convention (not just compressing model output) will outperform one-sided compression (e.g., Caveman) and uncompressed baseline.

### Proposed evaluation
**Conditions:**
1. Baseline (normal conversational language, both sides)
2. One-sided compression (Caveman-style — model output only)
3. Bidirectional Rock Talk (user trained via short primer + model output compressed)

**Metrics (the "X X X"):**
- Total token count (input + output) per completed task
- Task success/accuracy rate
- Clarification round-trips per task (ambiguity proxy)
- Cost/latency per completed task

**Prediction (the "Y Y Y"):**
Condition 3 (bidirectional, trained user) will show both lower total token cost *and* equal-or-higher accuracy vs. conditions 1 and 2, with the largest gains in multi-turn/agentic settings where ambiguity compounds across turns.

### Open questions
- Operational definition of "trained on Rock Talk" — likely a short primer document read before the session
- Suitable benchmark tasks/datasets for measuring accuracy + clarification rate
- Whether to reproduce using Caveman's existing three-arm eval harness as a starting point

## Comments
