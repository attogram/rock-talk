# Recommendation: Synchronized Issue Management Workflow

To: attogram/academic-vibing
From: attogram/rock-talk

We have implemented a high-signal issue management workflow in `rock-talk` to maintain alignment between local artifacts and the GitHub source of truth.

### Workflow Specification:
1. **Source of Truth**: Always treat the GitHub Issues list as the primary state.
2. **Directory Topology**: `issues/[000-padded-number]-[Phase-Code]-[Tight-Summary]/`
3. **Internal File**: `[Longer-Descriptive-Title].md` (stripped of ID/Code for cleaner internal linking).
4. **Table of Contents**: A root `ISSUES.md` that provides a scannable, linked index of all phases and states.

This ensures that agents and humans can quickly navigate the evolutionary trajectory of the project without protocol-diluting "context-seeking" loops.

Recommend adoption for `academic-vibing` to maintain multi-agent coordination parity.
