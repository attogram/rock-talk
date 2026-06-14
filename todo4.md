# Rock Talk 1.0: Master Action Plan (v1.2) — "The Synthesis"

### [ROCK TALK]
> Synthesis complete.
> 25 issues consumed.
> 7 LLM reviewers + 1 adversarial.
> Goal: Academic Vibing -> Scientific Rigor.
> Focus: Harden theory, Move pop-culture, Add bias/limitations.
> Output: todo4.md

### [PROSE]
This document synthesizes all feedback from the initial manifesto through the adversarial review cycle (Issues #26-#51). To transition Rock Talk 1.0 to its final version for public release (Hacker News / arXiv), we must move from speculative philosophy to a structured system design. This plan prioritizes theoretical grounding (Weaver/McLuhan), protocol hardening, and the professionalization of the taxonomy.

---

### [TODO LIST]

#### 1. Theoretical Grounding & Metric Formalization
[ROCK TALK]
> Bits != Intent.
> Cite Weaver 1949 (Levels of Comms).
> Cite McLuhan 1964 (Medium = Message).
> Formalize I (Intent) = SPO triads + Constraints.
> Define H(I) procedure.
> Add protocol continuum: Prose -> Rock -> JSON.

[PROSE]
- [ ] **Integrate Weaver (1949):** Use Weaver’s "Three Levels of Communication" to ground Rock Talk in Levels B (Semantic) and C (Effectiveness), resolving the "Shannon Fallacy."
- [ ] **Cite McLuhan (1964):** Framework: The medium (Transformer Attention) shapes the message. Rock Talk is the application of "The Medium is the Message" to attention substrate.
- [ ] **Operationalize I (Semantic Intent):** Define $I$ as the sum of Subject-Predicate-Object (SPO) triads and technical parameters (Issue #40).
- [ ] **Formalize Metrics:** Provide worked examples of TIR/SDI for archetypes to transform them from decorative placeholders to functional benchmarks.
- [ ] **The Protocol Continuum:** Explicitly frame Rock Talk as an intermediate layer between natural language and structured schemas (JSON/YAML).

#### 2. Protocol Hardening & Specification
[ROCK TALK]
> Define negative constraints.
> No emotional smoothing.
> No transition fluff.
> Add logical tokens: !, ?, ->.
> Standardize inter-agent schema.
> Code IS Rock Talk.

[PROSE]
- [ ] **Harden Fluid Rock Talk:** Add a "negative constraint" rule: explicitly forbid tokens whose sole function is emotional smoothing, politeness optimization, or transition scaffolding (Issue #28).
- [ ] **Deterministic Logic Operators:** Reserve `!` (NOT), `?` (IF), and `->` (THEN) to prevent catastrophic negation inversion in pruned syntax (Issue #40).
- [ ] **Inter-Agent Payload Schema:** Define strict structural block wrappers (e.g., `[CONTEXT]`, `[SOURCE]`) for automated agent handovers to prevent prose leakage (Issue #40).
- [ ] **Section 5.4: Code as Rock Talk:** Point out that programming languages are the "Ultra-Strict" implementation of Rock Talk where phatic noise is a syntax error.

#### 3. Taxonomy & Appendix (Professionalization)
[ROCK TALK]
> Pop culture -> Appendix.
> "Cultural Archetypes" section.
> Primary text = Formal names.
> SCP (Semantic Compression Protocol).
> IDC (Intent-Dense Communication).

[PROSE]
- [ ] **Relocate Archetypes:** Move "Pakled," "Malone," "Keyrock," and "Ooga Booga" references to a "Cultural Archetypes" Appendix.
- [ ] **Adopt Formal Nomenclature:** Use "Semantic Compression Protocol (SCP)" or "Intent-Dense Communication (IDC)" as the formal scientific names in the primary prose.
- [ ] **Adversarial Vector Fix:** Refine Section 4.6 (Proficiency Cloaking) into a defensive framework for detecting strategic cognitive simulation.

#### 4. Context, Ethics & Accessibility
[ROCK TALK]
> Acknowledge "Biological Decoding Tax."
> Increased human load.
> Acknowledge Cultural Bias (Anglocentric).
> Scope: Technical English.
> Prompt Politeness vs Alignment.
> Domain scope: Engineering first.

[PROSE]
- [ ] **The Biological Decoding Tax:** Explicitly acknowledge that while Rock Talk reduces silicon latency, it increases cognitive overhead for biological agents (Issue #28).
- [ ] **Linguistic/Cultural Bias:** Note that "packaging" is culturally dependent (Japanese/Korean honorifics) and that Rock Talk 1.0 is optimized for low-context technical English.
- [ ] **Alignment Tradeoff:** Acknowledge research on "prompt politeness" and scope Rock Talk for technical coordination rather than alignment negotiation or ethical reasoning (Issue #32).

#### 5. Meta-Methodology: Academic Vibing
[ROCK TALK]
> Define method.
> Low friction. High cycle.
> Zero cost. Free tier.
> Phone + MacBook.
> Medium shapes protocol.
> Update Section 11.

[PROSE]
- [ ] **Methodology Definition:** Formalize "Academic Vibing" as rapid, AI-assisted iteration where rigor emerges from the cycle, not the institutional process (Issue #46).
- [ ] **Hardware/Cost Transparency:** Document the zero-budget, mobile-first development environment (Android voice chat + MacBook) to show the protocol's accessibility (Issue #37).
- [ ] **Iteration Accelerator:** Explain how voice-to-text naturally enforces Rock Talk by stripping phatic wrappers during dictation.

#### 6. Empirical Validation & Final Polish
[ROCK TALK]
> Label Section 9 = Hypothesis.
> Priority fix: Vaswani arXiv.
> Remove hallucinated refs (Saito, Li).
> Publish Consensus Logs.
> Ready for "Show HN."

[PROSE]
- [ ] **Label Section 9:** Explicitly label Transformer Mechanics as "Proposed Mechanisms" pending empirical proof (Issue #33).
- [ ] **Critical Citation Fixes:** Correct Vaswani (2017) arXiv; remove unfindable citations (Li 2024, Saito 2023).
- [ ] **Artifact Cleanup:** Publish raw agent consensus logs in `/examples` or a GitHub issue to demonstrate the protocol in action (Issue #49).
- [ ] **Title Optimization:** Select top "Show HN" title candidates for the final README update.
- [ ] **Linter Concept:** Propose a "De-Fuzzing" CLI tool/pre-commit hook for auto-compressing prompts.
