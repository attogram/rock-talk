# #23: C12

Metadata:
- State: closed
- Author: attogram
- Created: 2026-06-13T22:42:14Z

## Description
This is a surprisingly strong piece of concept framing, but it currently sits somewhere between a manifesto, a research proposal, a parody paper, and a genuine HCI/LLM communication framework. Whether it succeeds depends heavily on which of those you want it to be.

Overall Assessment

Strengths

Memorable core idea.

Strong branding ("Rock Talk" is sticky).

Clear intuition that many people already experience when working with LLMs.

Good separation between ROCK TALK examples and formal prose.

Connects multiple disciplines:

Information theory

Pragmatics

HCI

Prompt engineering

Multi-agent systems


Introduces testable hypotheses instead of merely making claims.

Recognizes an important distinction in §5.1:

Rock Talk is about signal density

not "pretending to be a caveman"



That distinction saves the paper from becoming a gimmick.


---

Biggest Strength

The strongest idea is actually not the caveman syntax.

The strongest idea is:

> Communication efficiency should be measured by semantic density rather than linguistic sophistication.



That is a legitimate research direction.

Many prompt-engineering techniques already implicitly assume this:

structured prompts

XML prompting

DSLs

chain-of-thought compression

agent protocols

function calling

state serialization


Rock Talk can be interpreted as a human-readable version of that broader trend.

In that framing, the paper becomes much more interesting.


---

Biggest Weakness

The paper repeatedly assumes:

> fewer tokens → better alignment



This is not established.

In many cases the opposite is true.

Example:

Natural language:

> Generate a PostgreSQL migration. Preserve backward compatibility. Do not remove columns. Existing clients depend on schema version 4.



Compressed version:

> PG migration. Backward compatible. No column delete. Schema v4 clients exist.



Mostly fine.

But compress further:

> PG migration. Keep compatibility.



Now critical constraints disappeared.

The problem:

Compression removes redundancy.

Redundancy is often how humans and LLMs recover meaning.

Shannon's channel theory does not imply:

> minimum tokens = optimal communication



In fact engineered communication systems often intentionally add redundancy for error correction.

This is probably the largest theoretical gap in the paper.


---

Shannon Is Being Stretched

You invoke Shannon constantly.

The issue:

Shannon information ≠ semantic information.

Shannon would assign high information content to:

> f9Qx7#vL2k$



even though it is meaningless to humans.

Meanwhile:

> Database down.



contains enormous semantic value.

So when the paper says:

> maximize signal



it is actually talking about:

semantic relevance

task relevance

pragmatic efficiency


not Shannon entropy.

You may want to explicitly acknowledge this.

Otherwise communication theorists will attack that section immediately.


---

Stronger Framing

Instead of:

> Rock Talk reduces entropy.



Consider:

> Rock Talk attempts to maximize task-relevant semantic density.



That wording is harder to criticize.


---

The "Attention Drift" Claims Need Evidence

Several sections imply:

> fewer filler tokens improve transformer reasoning



This sounds plausible.

But the paper currently jumps from intuition to conclusion.

For example:

> Standard conversational filler tokens consume positional embeddings and distort softmax attention.



That is a much stronger claim than current evidence supports.

Potential reviewer response:

> Citation needed.



A safer version would be:

> We hypothesize that reducing low-information tokens may improve retrieval of task-relevant instructions within long contexts.



That is experimentally testable.


---

Best Section: Elasticity of the Protocol

§5.1 is the strongest section in the entire paper.

Without it, Rock Talk looks like:

> Me software engineer. Me fix bug.



With it, Rock Talk becomes:

> a continuum of compression strategies.



That makes it much harder to dismiss.

I would move this section earlier.

Possibly before the archetypes.


---

The Archetype Section

This is simultaneously:

the funniest part

the weakest academic part


The categories are memorable:

Pirate Talk

Kevin Malone

Pakleds

Cytherians

Ooga Booga Fallacy

Unfrozen Caveman Lawyer


But a reviewer would immediately ask:

> Are these analytical categories or jokes?



Right now they're both.

For a serious paper:

Move them to an appendix.

For a manifesto:

Keep them exactly where they are.

For a conference submission:

They need formalization.


---

Risk: Tone Oscillation

The paper alternates between:

Serious

Shannon

Grice

Clark

Sperber & Wilson


and

Meme

Kevin Malone

Pakleds

Caveman Skill

Ooga Booga


The oscillation is entertaining but creates credibility issues.

Readers will ask:

> Is this satire?



A useful rule:

If you want publication:

80% serious

20% fun


Current ratio feels closer to:

50% serious

50% fun



---

TIR and SDI Need Formal Definitions

The proposed metrics are interesting but currently underspecified.

For example:

TIR

TIR=\frac{T}{H(I)}

Question:

How is  measured?

Human raters?

Task success?

Embedding entropy?

Information extraction?

Without operationalization the metric is not computable.


---

SDI

SDI=\frac{I}{T}

Again:

What counts as a semantic concept?

Example:

> Restart database and clear cache.



Is that:

2 concepts?

1 objective?

3 actions?


A reviewer would demand formal definitions.


---

Agent Coordination Section Has Potential

This may actually be the most novel research angle.

People have already observed:

multi-agent drift

context accumulation

instruction mutation

planning divergence


The idea that a constrained communication protocol could reduce drift is genuinely plausible.

This area feels stronger than the human-side efficiency claims.

If I were expanding the paper, I'd focus here.


---

Missing Comparisons

Rock Talk should be compared against existing approaches:

XML prompting

JSON schemas

DSLs

controlled natural languages

aviation phraseology

military brevity codes

SBAR communication

prompt templates

function calling


Otherwise reviewers will say:

> This is controlled language with a new name.



You need a section explaining what Rock Talk adds beyond those systems.


---

Publication Readiness

If submitted today:

Academic conference

Probably rejected.

Not because the idea is bad.

Because:

evidence is limited

metrics aren't operationalized

citations are sometimes decorative rather than evidentiary

theoretical claims exceed demonstrated results


Position paper / workshop paper

Much better fit.

Blog post / manifesto

Excellent fit.

Open-source protocol specification

Probably the strongest format.


---

Final Verdict

The core contribution is not:

> "Talk like caveman."



The core contribution is:

> "Communication should optimize semantic density rather than social packaging when humans and machines share sufficient context."



That is a legitimate and potentially useful idea.

The paper's biggest challenge is separating:

the humorous "caveman" aesthetic from

the genuinely interesting hypothesis about high-density communication protocols.


If you tighten the theoretical claims, formalize the metrics, reduce reliance on Shannon as a catch-all justification, and focus more on agent-to-agent communication, the paper moves from "clever manifesto" toward "serious research agenda."

## Comments
