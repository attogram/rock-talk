# Operational Plan: Rock Talk 0.3 Evolution

## 1. Summary of Proposed Plan

The next phase of the project shifts from conceptual framing to **operational rigor and empirical validation**. We will build the tooling described in the "Phase L" issues, conduct formal compression studies using the existing papers as a corpus, and address the "sycophancy trap" by integrating adversarial peer-review logic.

### Key Objectives:
1. **Tooling**: Develop the Rock Talk Transpiler (RTS) specification.
2. **Validation**: Execute the 3-Arm Testing Architecture (Token Efficiency, Attention Drift, Cascade Failures).
3. **Refinement**: Integrate "Human as Transport Substrate" model to improve protocol resilience.
4. **Academics**: Finalize Rock Training and Rock Culture papers for 0.1 release.

---

## 2. Issues to Accept (Proposed for Immediate Execution)

These issues represent clear, non-conflicting improvements to the protocol and repository structure:

- **#111 (RTS)**: Define the universal document → Rock Talk transpiler logic.
- **#110 (Transport Substrate)**: Integrate the HTF (Human Transport Fidelity) metric into Section 2.1.
- **#109 & #108 (Compression Studies)**: Conduct the canonical artifact stress tests.
- **#107 (Image Standards)**: Apply the "Black Footer" attribution to all existing media assets.
- **#105, #103, #102 (Cultural Landmarks)**: Update `rock-culture.0.1.md` with The Martian, Arrival, and the "Watney Shift" / "Nathan Axiom" archetypes.
- **#101 (Global Pruning)**: Perform a repo-wide pass to enforce the 80-char limit and "no-fluff" prose.
- **#97 (Adversarial Agent)**: Begin drafting the "Adversarial Agent" blueprint (Model A/B system).

---

## 3. Issues with Conflicting Views (Needs Human Vibe)

These issues touch on the "soul" of the project vs. its "academic skin":

- **#96 (The "Shut the F* Up" Factor)**:
  - *Conflict*: Professional nomenclature (SCP/IDC) vs. raw, visceral developer origin story.
  - *Need*: Does the project want to lean into the "angry engineer" persona for brand signal, or move toward pure academic neutrality to maximize institutional adoption?
- **AV#6 (The CoT Contradiction)**:
  - *Conflict*: Rock Talk claims "less is more," while LLM reasoning (CoT) proves "more is more."
  - *Need*: How much should the protocol yield to the "computational scaffolding" requirement? Does Rock Talk become an *input/output* layer only, while leaving the *reasoning* layer verbose?

---

## 4. Edge Cases

- **Clipboard-Mediated Loss**: Transmitting dense Rock Talk through high-latency human interfaces (mobile apps, web UIs) often leads to truncation or "hallucinated reconstruction" by the human operator.
- **Cross-Lingual SCP**: How do SPO triads manifest in non-SVO (Subject-Verb-Object) languages like Japanese or Korean?
- **Sycophancy vs. Rigor**: Managing the "Helpfulness Bias" in agents (Jules included) when they are asked to review their own protocol. Integration of Issue #97 (Adversarial Agent) is the proposed fix.
- **Token budget "Phase Transitions"**: Identifying the exact point where a 32K context window becomes "saturated" by phatic noise.

---

## 5. Next Steps

1. Execute **#101** (Global Pruning) to stabilize the codebase.
2. Draft the **#111** (RTS) technical spec in `examples/`.
3. Update `papers/rock-culture/` with the new archetypes from **#102**.
4. Set up the **#109** benchmarking environment.
