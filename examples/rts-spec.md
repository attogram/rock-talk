# RTS Spec: Universal Document → Rock Talk Transpiler

Version: 0.1 Date: June 14, 2026
Status: Specification

## 1. Objective
Define the logic for a universal transpiler that converts natural language
documents (Prose) into high-signal Rock Talk (SCP/IDC) formats.

## 2. Core Logic (The De-Fuzzing Algorithm)

### Phase 1: Structural Extraction
1.  **SPO Identification**: Identify all Subject-Predicate-Object triads.
2.  **Constraint Isolation**: Extract technical parameters (versions, ports,
error codes, logic gates).
3.  **Boundary Detection**: Map [CONTEXT], [SOURCE], and [TASK] blocks.

### Phase 2: Noise Elimination
1.  **Phatic Strip**: Remove emotional smoothing tokens (e.g., "I hope,"
"sincerely," "unfortunately").
2.  **Structural Collapse**: Remove redundant grammatical scaffolding (e.g.,
"The purpose of this document is to...").
3.  **Negation Verification**: Convert natural language negations into
deterministic logic operators (!).

### Phase 3: Semantic Compression
1.  **Token Weighting**: Replace multi-token phrases with high-weight single
tokens (e.g., "in order to facilitate" → "for").
2.  **Topology Mapping**: Format output into Stacked Imperatives (Ultra-Strict)
or Compressed Blocks (Fluid).

## 3. Reference Implementation (Pseudocode)

```python
def transpile_to_rock(prose_input):
    intent = extract_semantic_intent(prose_input)
    noise_reduced = strip_phatic_packaging(intent)
    operators_applied = apply_deterministic_logic(noise_reduced)
    return format_topology(operators_applied, mode="STRICT")
```

## 4. Metrics
- **Compression Ratio**: T_prose / T_rock.
- **SDI Score**: semantic_intent / token_count.
- **Transpilation Fidelity**: I_output / I_input (Target: 1.0).
