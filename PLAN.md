# Operational Plan: Rock Talk 0.5 — The Empirical Phase

## 1. Summary of Proposed Plan

The 0.5 phase transitions Rock Talk from a theoretical framework into a **rigorously tested and tool-supported protocol**. We will execute the 3-Arm Testing Architecture defined in `rock-talk.0.4.md`, develop the first functional prototype of the De-Fuzzing Linter, and initiate the Native Semantic Pre-training (NSP) corpus generation.

### Key Objectives:
1.  **Validation**: Execute formal benchmarks for Token Efficiency (Arm 1) and Attention Drift (Arm 2).
2.  **Tooling**: Build the `rt-lint` CLI prototype for real-time SDI/TIR calculation.
3.  **Expansion**: Spec out the NSP training corpus and multi-lingual adaptation strategies.
4.  **Resilience**: Conduct "Format Collapse" tests to identify the limits of semantic compression.

---

## 2. Issues to Accept (Proposed for Immediate Execution)

These issues represent the core work for the 0.5 cycle:

- **#113 (Arm 1: Token Efficiency)**: Implement the testing environment using 100 complex technical tasks.
- **#114 (Arm 2: Attention Drift)**: Set up Softmax entropy visualization for needle-in-haystack tests.
- **#116 (De-Fuzzing Linter)**: Develop a basic CLI that identifies phatic noise and calculates SDI.
- **#118 (NSP Corpus)**: Generate the first syntax-stripped training dataset from the existing papers.
- **#120 (Semantic Intent Calculator)**: Automate the SPO triad extraction process for TIR benchmarking.

---

## 3. Issues with Conflicting Views (Needs Human Vibe)

- **#117 (Multi-lingual Adaptation)**:
  - *Conflict*: Strict Rock Talk vs. Cultural Register Shifts.
  - *Need*: Should the protocol adapt to Japanese/Korean honorific structures, or should it remain a "technical-only" dialect that bypasses these social layers entirely?
- **#115 (Arm 3: Cascade Failures)**:
  - *Conflict*: Measuring "Understanding" vs. "Output Similarity".
  - *Need*: How do we verify that Sub-agent C truly "understood" the intent vs. just mimicking the compressed pattern?

---

## 4. Edge Cases

- **Hallucinated Reconstruction**: Cases where high compression causes an LLM to "fill in the blanks" with incorrect technical assumptions.
- **Linter Over-optimization**: The risk of the linter suggesting changes that technically increase SDI but break logical coherence.
- **NSP Gradient Instability**: Technical risk that the syntax-stripped corpus leads to non-convergent training runs.

---

## 5. Next Steps

1.  Initialize the **#113** benchmarking suite in a new `benchmarks/` directory.
2.  Draft the `rt-lint` logic in `examples/linter-prototype.py`.
3.  Update **#118** with a sample of the syntax-stripped NSP corpus.
4.  Prepare the 0.5 release notes.
