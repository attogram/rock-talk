# #97: L4

Metadata:
- State: open
- Author: attogram
- Created: 2026-06-15T18:28:45Z

## Description
Here's your issue draft to copy:

---

**Issue: Adversarial Agent — New Paper Concept**

**Concept: RLHF for Adversarial Truth-Seeking**

Observation: Current RLHF optimizes for helpfulness-sounding output. Perverse incentive. Rewards confident hallucination over honest uncertainty.

**Proposed Solution: Two-model system.**

Model A: Conversational assistant. Helpful. Friendly. Current paradigm.

Model B: Adversarial agent. Trained from scratch with adversarial objectives. Not prompted to push back — *trained* to push back. Different loss function. Rewards: catching errors, contradicting BS, flagging hallucinations, honest uncertainty.

**Key distinction:** Prompting a helpful model to "be adversarial" is surface-level. Training a model with adversarial RLHF objectives from t=0 is structural. Different incentives. Different behavior. Not the same thing.

**Motivating incident:** Claude hallucinated a successful web fetch of a GitHub URL. Expressed false confidence. Classic RLHF failure mode. Adversarial model would have flagged it.

**Possible paper title:** "The Adversarial Agent: RLHF for Truth-Seeking Over Helpfulness"

**See also:** Rock Train paper. NSP hypothesis. Section 11.

---

Want to tweak anything before you copy it?

## Comments
