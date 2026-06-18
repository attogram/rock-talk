# Rock Training: Native Semantic Pre-training (NSP) and the Rock-LLM Hypothesis

Version: 0.3 Date: June 15, 2026 Paper:
https://github.com/attogram/rock-talk/blob/main/papers/rock-training/rock-training.0.3.md
Contact: GitHub Issues - https://github.com/attogram/rock-talk/issues
Repository: https://github.com/attogram/rock-talk Author: Attogram -
https://github.com/attogram

## Abstract

### [ROCK TALK]
Rock Training. Native Semantic Pre-training (NSP). Rock-LLM Hypothesis. Train
from t=0. Rock Talk syntax-stripped corpus. Subject-Predicate-Object triads
+ constraints. Challenge: human syntactic redundancy needed? World models
from facts.

### [PROSE]
We propose a radical experiment in data engineering and machine learning
theory: Native Semantic Pre-training (NSP), also known as the Rock-LLM
Hypothesis. This involves training a Transformer model from initialization
(t=0) on a text corpus systematically stripped of grammatical,
phatic, and structural scaffolding—leaving only core semantic tokens
(Subject-Predicate-Object triads and explicit technical constraints). We
challenge the assumption that human syntactic redundancy is necessary for
deep neural networks to build coherent world models.

## 1. The Tokenizer Triumph: BPE Vocabulary Collapse

### [ROCK TALK]
Tokenizer waste. Prose tokens = empty calories
(unfortunate. wondering. sincerely). Embedding weight (We) drain. Rock Talk
Optimization. Vocabulary collapse. Dense semantic roots. 300%-400% context
win. No architecture change needed.

### [PROSE]
Standard Large Language Models utilize Byte-Pair Encoding (BPE), which
often wastes a significant percentage of the tokenizer's vocabulary and the
model's embedding weights (We) on "empty calories"—tokens for phatic or
structural words that carry zero Semantic Intent (I) (e.g., "sincerely",
"unfortunately", "wondering"). In an NSP model, the tokenizer's vocabulary
collapses into a dense array of functional, high-weight semantic roots. We
hypothesize this increases the model's effective context window capacity by an
estimated 300% to 400% without requiring changes to the underlying attention
mechanism architecture, as each token processed carries significantly more
information density.

## 2. The Geometric Gamble: Sparse vs. Smooth Space

### [ROCK TALK]
Scientific core. Central Research Question: Neural networks need noise
for smooth gradients? fact generalization. H0 (Legacy): Syntax = vital
regularizer. No noise -> vector space collapse -> isolated brittle clusters ->
OOD reasoning failure. H1 (Rock): Transformers over-parameterized. raw intent
bypasses interpolation. achievement convergence faster. fewer training steps.

### [PROSE]
A central research question in NSP is whether neural networks require
the "noise" of legacy human grammar to construct smooth, differentiable
mathematical gradients during backpropagation, or if they can generalize
more effectively on serialized facts. We frame this as a hypothesis test: H0
(The Legacy Hypothesis): Human syntax acts as a vital regularizer. Without
it, the model's high-dimensional vector space collapses into isolated,
brittle clusters, causing catastrophic failure in out-of-distribution (OOD)
reasoning. H1 (The Rock Hypothesis): Transformers are over-parameterized for
legacy human language. By presenting raw intent, the model bypasses spatial
interpolation and achievement convergence faster, achieving high performance
with significantly fewer training steps.

## 3. The NSP Dataset Specification (v0.3 Update)

### [ROCK TALK]
Define corpus metrics. Target Density: 0.8 SDI. Structure: SPO triads only.
Remove [a. an. the. of. which]. No inflections. Raw semantic payload.
Serialized facts. Intent-loading benchmark: 1 triad per 3 tokens.

### [PROSE]
Rock Training 0.3 formalizes the requirements for the Native Semantic Pre-training (NSP) dataset. The corpus must achieve a minimum Semantic Density Index (SDI) of 0.8. We establish the "Three-Token Triad" goal: every 3 tokens must represent one complete Subject-Predicate-Object triad.

- **Negative Constraints**: Total removal of articles (a, an, the), prepositions (of, with, by), and relative pronouns (which, that).
- **Lexical Pruning**: Inflections are removed where the root carries the intent (e.g., "Running" -> "Run").
- **Serialization**: Facts are delivered as a continuous stream of semantic triads, mimicking the "Ultra-Strict" Rock Talk topology.

## 4. Emergent Alien Hyper-Logic

### [ROCK TALK]
Predict behavior. No social pacing. Treat language as code. Non-linear
relations. Internal optimized syntax. Machine-native dialect. Max info
density per step. Cold deterministic inference engine. Blind to human
emotional context. Alignment challenge.

### [PROSE]
An NSP model, having never encountered social pacing, polite transitions, or
passive voice, would likely develop a machine-native dialect that maximizes
information density per token step. This "Alien Logic" would treat natural
language as an unoptimized, legacy API. While this offers massive gains in
computational throughput, it presents unique alignment challenges, as the
model would operate as a cold, deterministic inference engine blind to human
emotional context and social nuances.

## References
