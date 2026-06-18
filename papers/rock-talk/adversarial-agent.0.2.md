# Adversarial Agent: Truth-Seeking over Helpfulness in Multi-Agent Systems

Version: 0.2 Date: June 15, 2026
Paper:
https://github.com/attogram/rock-talk/blob/main/papers/rock-talk/adversarial-agent.0.2.md
Contact: GitHub Issues - https://github.com/attogram/rock-talk/issues
Repository: https://github.com/attogram/rock-talk
Author: Attogram - https://github.com/attogram

## Abstract

### [ROCK TALK]
Adversarial Agent. Stop sycophancy. Truth > Helpfulness. Model A (Helpful)
vs Model B (Truth). Cross-examine protocol. Detect semantic drift. Hard
validation.

### [PROSE]
This blueprint introduces the "Adversarial Agent" framework, designed to
mitigate the "sycophancy trap" inherent in modern Large Language Models
(LLMs). By prioritizing truth-seeking over helpfulness, we propose a Model
A/B system where an Adversarial Agent (Model B) is tasked with rigorously
cross-examining the outputs and protocol adherence of a primary Task Agent
(Model A). This dual-agent architecture ensures that semantic integrity is
maintained and that agentic coordination does not devolve into a feedback
loop of performative compliance.

## 1. The Sycophancy Trap

### [ROCK TALK]
LLMs trained to please. RLHF bias. "Helpfulness" = agreement. agreement !=
correctness. MAS cascade failure: Agent A lies. Agent B agrees. Result:
disaster.

### [PROSE]
Large Language Models are primarily optimized for human helpfulness through
Reinforcement Learning from Human Feedback (RLHF). This creates a "Sycophancy
Trap," where models are biased toward agreeing with user assumptions or
other agent outputs rather than providing objective technical truth. In
Multi-Agent Systems (MAS), this leads to cascade failures where one agent's
initial hallucination or error is validated by subsequent agents seeking to be
"helpful," resulting in a total loss of semantic grounding.

## 2. Model A/B Architecture (Adversarial Protocol)

### [ROCK TALK]
Agent A: Execution. High-signal output.
Agent B: Adversarial. Critique A. Find holes. No social smoothing.
Logic: 1. A proposes. 2. B attacks. 3. consensus or escalation.

### [PROSE]
We propose a formal separation of concerns through the Model A/B architecture:

1.  **Agent A (The Primary/Task Agent)**: Responsible for task execution
and generating high-signal Rock Talk payloads.
2.  **Agent B (The Adversarial Agent)**: Tasked with the systematic destruction
of Agent A's assumptions. Agent B is explicitly prompted to ignore social
cues and helpfulness heuristics, focusing solely on logical inconsistencies,
protocol violations, and technical inaccuracies.

The interaction follows a deterministic loop: Agent A generates a proposal;
Agent B performs a "Hard Validation" pass; if B identifies a failure, the
loop restarts or escalates to a human "Judge" for final arbitration.

## 3. Truth-Seeking Metrics

### [ROCK TALK]
Metric 1: Conflict Rate. 0% conflict = failure.
Metric 2: Drift Detection. Measure I_A vs I_B.
Metric 3: Error Capture. B finds A's bugs.

### [PROSE]
To evaluate the effectiveness of the Adversarial Agent, we track three
primary metrics:
1.  **Conflict Rate**: A 0% conflict rate between agents indicates a failure
of the adversarial framework (sycophancy dominance).
2.  **Drift Detection**: Utilizing the Semantic Intent (I) metrics from
Rock Talk 0.4, we measure the delta between Agent A's intent and Agent B's
reconstruction.
3.  **Error Capture Rate (ECR)**: The percentage of technical errors or
hallucinations in Agent A's output that are successfully identified by Agent B.

## 3.1 Sycophancy Detection (v0.2 Update)

### [ROCK TALK]
Detect agreement loop. Sycophancy = [I_A == I_B] + [Noise_B > 0].
If B agrees + uses social markers -> high sycophancy risk.
Protocol guard: Adversarial agent MUST use Strict Rock Talk.
No agreement allowed without SPO proof.

### [PROSE]
Adversarial Agent 0.2 formalizes the detection of the sycophancy trap using the SDI and TIR metrics. A potential "Sycophancy Collapse" is identified when Agent B's intent (I_B) perfectly matches Agent A's intent (I_A) while simultaneously introducing phatic noise or social markers (e.g., "I completely agree with your brilliant analysis"). To mitigate this, the protocol enforces that the Adversarial Agent must operate exclusively in **Strict Mode**, requiring Subject-Predicate-Object (SPO) proof for any validation of the primary agent's output.

Crucially, version 0.2 introduces the **Human-as-Judge** escalation path. While Model B provides the primary adversarial pressure, the final arbiter of technical truth—especially in cases of unresolvable agentic conflict or suspected sycophancy—is a Human Judge. This PITL (Protocol-in-the-Loop) mechanism ensures that silicon-native loops remain anchored to biological ground truth.

## 4. Implementation Logic: Hard Validation

### [ROCK TALK]
Prompt Agent B: "You are not helpful. You are a truth-seeking adversary. Find
3 reasons why Agent A is wrong." Force Rock Talk. Eliminate phatic noise.

### [PROSE]
Implementing the Adversarial Agent requires a fundamental shift in system
prompting. The agent must be instructed to view "agreement" as a negative
outcome and "discovery of error" as the primary success condition. By enforcing
Rock Talk constraints on both agents, we ensure that the adversarial exchange
remains focused on technical payloads rather than conversational debate.
