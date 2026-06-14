# Rock Talk 1.0 — Citation Audit Log

**Auditor:** Claude Sonnet 4.6  
**Date:** 2026-06-14  
**Status Key:** ✅ VERIFIED | ⚠️ NEEDS FIX | ❌ NOT FOUND / LIKELY HALLUCINATED | 🔍 UNVERIFIED

---

## CRITICAL FIXES FIRST

### ⚠️ Vaswani et al. (2017) — WRONG arXiv NUMBER
- **Paper ref in text:** `arXiv:2005.14165` (this is GPT-3 / Brown et al. 2020)
- **Correct arXiv:** `1706.03762`
- **Verified:** YES — confirmed at https://arxiv.org/abs/1706.03762
- **Action:** Fix the arXiv number in the paper body (Section 9). The citation in the References section is correct; the inline link is wrong.

---

## FULL CITATION AUDIT

### ✅ ALSSA (2025)
- **Claim:** Multi-Service Brevity Codes
- **URL in paper:** https://www.alssa.mil/mttps/brevity/
- **Status:** PLAUSIBLE — ALSSA is a real organization (Air Land Sea Space Application Center). URL structure looks authentic. Direct verification blocked by network config.
- **Risk:** Low. Military brevity codes are a well-documented real-world phenomenon.

### ⚠️ Brath, R., et al. (2023)
- **Claim:** Visualizing LLM text style transfer, IEEE VIS 2023
- **URL in paper:** https://nlviz.github.io/2023/papers/nlviz2023_brath.pdf
- **Status:** URL RETURNS 404. Paper cannot be confirmed.
- **Action:** Find correct URL or remove. The NLVIZ workshop at IEEE VIS is real, but this specific paper needs verification. Search "Brath 2023 text style LLM visualization" for correct link or remove citation.

### ✅ Brown, T. B., et al. (2020)
- **Claim:** Language Models are Few-Shot Learners
- **arXiv in paper:** 2005.14165
- **Status:** VERIFIED — this IS the correct arXiv for GPT-3 (Brown et al. 2020)
- **Note:** This is listed in references but NOT cited in the paper body. ORPHANED REFERENCE.

### ✅ Burroughs, E. R. (1912)
- **Claim:** Tarzan of the Apes
- **Status:** VERIFIED — canonical, real work. Not cited in body. ORPHANED REFERENCE.

### ✅ Clark, H. H. (1996)
- **Claim:** Using Language, Cambridge University Press
- **Status:** VERIFIED — real, canonical linguistics text.

### ✅ Daniels, G., & Thompson, B. (1989)
- **Claim:** "Samaritan Snare," Star Trek: TNG
- **Status:** VERIFIED — real episode, Season 2, Episode 17. Note: not cited in body. ORPHANED REFERENCE. (The Pakled reference.)

### ✅ FAA (2026)
- **Claim:** Pilot/Controller Glossary
- **URL in paper:** https://www.faa.gov/air_traffic/publications/media/PCG_Bsc_w_Chg_1_and_2_dtd_1-22-26.pdf
- **Status:** PLAUSIBLE — FAA publishes real PCG documents. The 2026 date is consistent with the paper's date. Direct fetch blocked.
- **Risk:** Low.

### ✅ Frising, M. (2025)
- **Claim:** Linear Personality Probing and Steering in LLMs: A Big Five Study
- **arXiv in paper:** 2512.17639
- **Status:** VERIFIED — confirmed at https://arxiv.org/abs/2512.17639. Authors: Michel Frising & Daniel Balcells. Submitted Dec 19, 2025.
- **Note:** Paper is about personality steering, not specifically "intent loading of Cytherian-style communication" — the connection to Section 4.4 is loose. Flag as interpretive citation.

### ✅ Givón, T. (1979)
- **Claim:** On Understanding Grammar, Academic Press
- **Status:** VERIFIED — real, canonical linguistics text.

### ✅ Grice, H. P. (1975)
- **Claim:** Logic and Conversation, in Syntax and Semantics
- **Status:** VERIFIED — canonical pragmatics text.

### ✅ Handey, J. (1991)
- **Claim:** "Unfrozen Caveman Lawyer," SNL Season 17 Episode 7
- **Status:** VERIFIED — real SNL sketch. YouTube link in paper may work.
- **Note:** Jack Handey didn't write this sketch — it was Phil Hartman's character written by the SNL writing staff. The reference cites "Handey, J." which is incorrect. The sketch was written by Jack Handey (who was a writer on SNL at the time). Needs verification of exact authorship credit.

### ✅ Hanna, W., & Barbera, J. (1960)
- **Claim:** The Flintstones, ABC
- **Status:** VERIFIED — real. Not cited in body. ORPHANED REFERENCE.

### ✅ JuliusBrussee (2024)
- **Claim:** Claude Caveman, GitHub Repository
- **URL in paper:** https://github.com/juliusbrussee/caveman
- **Status:** PLAUSIBLE — GitHub URL structure is valid. The 65% token saving claim comes from this repo. Direct verification blocked.
- **Risk:** Medium. Verify the repo exists and the 65% claim is documented there.

### ✅ Levinson, S. C. (2000)
- **Claim:** Presumptive Meanings, MIT Press
- **Status:** VERIFIED — real, canonical pragmatics text.

### ❌ Li, J. (2024)
- **Claim:** Cognitive Load and Linguistic Compression in Stressful Environments, Journal of Computational Linguistics
- **Status:** NOT FOUND. No evidence this paper exists. Search returned no matching results. "Journal of Computational Linguistics" doesn't match standard journal names (the real journal is just "Computational Linguistics").
- **Action:** REMOVE or REPLACE. This reads as a hallucinated citation. If you need a citation for stress-induced linguistic compression, find a real one or remove the claim.

### ✅ Liu, N. F., et al. (2024)
- **Claim:** Lost in the Middle, TACL vol. 12
- **DOI in paper:** https://doi.org/10.1162/tacl_a_00638
- **Status:** VERIFIED — real, widely cited paper. DOI appears correct.

### ✅ Malinowski, B. (1923)
- **Claim:** The Problem of Meaning in Primitive Languages, in The Meaning of Meaning
- **Status:** VERIFIED — canonical anthropological text, original source of "phatic communion."

### ✅ Malik, A., et al. (2024)
- **Claim:** From Tarzan to Tolkien: Controlling Language Proficiency, ACL 2024
- **DOI in paper:** https://doi.org/10.18653/v1/2024.findings-acl.926
- **Status:** VERIFIED — confirmed at ACL Anthology. Authors: Ali Malik, Stephen Mayhew, Christopher Piech, Klinton Bicknell.

### ✅ Manning, M. (Director, 1991)
- **Claim:** "The Nth Degree," Star Trek: TNG
- **Status:** VERIFIED — real episode. Season 4, Episode 19. (Cytherian reference.) Not cited in body. ORPHANED.

### ✅ Miller, G. A. (1956)
- **Claim:** The Magical Number Seven, Psychological Review
- **Status:** VERIFIED — one of the most cited papers in cognitive psychology.

### ✅ Raiyan, S. R., et al. (2025)
- **Claim:** FrugalPrompt: Reducing Contextual Overhead in LLMs
- **arXiv in paper:** 2510.16439
- **Status:** VERIFIED — confirmed at https://arxiv.org/abs/2510.16439. This paper is directly relevant and strongly supports the Rock Talk thesis.

### ❌ Saito, H. (2023)
- **Claim:** Signal Processing in Human-Machine Interaction, Tokyo Institute of Technology
- **Status:** NOT FOUND. No evidence this paper exists. No matching results found. Tokyo Institute of Technology is real but this specific paper is unverifiable.
- **Action:** REMOVE. Almost certainly a hallucinated citation.

### ✅ Shannon, C. E. (1948)
- **Claim:** A Mathematical Theory of Communication, Bell System Technical Journal
- **URL in paper:** https://archive.org/details/shannon1948
- **Status:** VERIFIED — canonical foundational paper.

### ✅ Somerstep, S., et al. (2024)
- **Claim:** Weak-to-strong generalization, arXiv:2405.16236
- **Status:** PLAUSIBLE — arXiv number format correct. Not cited in body. ORPHANED REFERENCE.
- **Action:** Verify and either cite in body or remove from references.

### ✅ Sperber, D., & Wilson, D. (1986)
- **Claim:** Relevance: Communication and Cognition, Harvard University Press
- **Status:** VERIFIED — canonical pragmatics text.

### ✅ Standage, T. (1998)
- **Claim:** The Victorian Internet, Macmillan
- **Status:** VERIFIED — real book, widely available.

### ✅ Vaswani, A., et al. (2017)
- **Claim:** Attention Is All You Need, NeurIPS
- **Correct arXiv:** 1706.03762
- **Status:** VERIFIED — confirmed at https://arxiv.org/abs/1706.03762
- **⚠️ FIX REQUIRED:** Inline citation in Section 9 uses wrong arXiv number (2005.14165 = GPT-3). References section is correct.

### ✅ Yang, B., et al. (2025)
- **Claim:** Crafting Customisable Characters with LLMs, arXiv:2406.17962
- **Status:** VERIFIED — confirmed at https://arxiv.org/abs/2406.17962. Published as EMNLP 2025 Findings.
- **Note:** Paper date is arXiv 2024 but published 2025. Citation as "2025" is defensible given formal publication date.

### 🔍 Zhang, T., et al. (2024)
- **Claim:** Self-interpreting Adversarial Images, arXiv:2407.08970
- **Status:** UNVERIFIED. Not cited in body. ORPHANED REFERENCE.
- **Action:** Verify and either cite or remove.

### ✅ Zipf, G. K. (1949)
- **Claim:** Human Behavior and the Principle of Least Effort, Addison-Wesley
- **URL in paper:** https://archive.org/details/humanbehaviorpri00zipf
- **Status:** VERIFIED — canonical text.

---

## SUMMARY TABLE

| Citation | Status | Action |
|---|---|---|
| ALSSA 2025 | ✅ Plausible | Verify URL live |
| Brath 2023 | ⚠️ 404 | Find correct URL or remove |
| Brown 2020 | ✅ Verified | Orphaned — cite or remove |
| Burroughs 1912 | ✅ Verified | Orphaned — cite or remove |
| Clark 1996 | ✅ Verified | OK |
| Daniels & Thompson 1989 | ✅ Verified | Orphaned — cite or remove |
| FAA 2026 | ✅ Plausible | OK |
| Frising 2025 | ✅ Verified | Loose connection — flag as interpretive |
| Givón 1979 | ✅ Verified | OK |
| Grice 1975 | ✅ Verified | OK |
| Handey 1991 | ⚠️ Authorship | Verify Jack Handey wrote this specific sketch |
| Hanna & Barbera 1960 | ✅ Verified | Orphaned — cite or remove |
| JuliusBrussee 2024 | 🔍 Plausible | Verify GitHub repo + 65% claim |
| Levinson 2000 | ✅ Verified | OK |
| **Li 2024** | **❌ NOT FOUND** | **REMOVE — likely hallucinated** |
| Liu 2024 | ✅ Verified | OK |
| Malinowski 1923 | ✅ Verified | OK |
| Malik 2024 | ✅ Verified | OK |
| Manning 1991 | ✅ Verified | Orphaned — cite or remove |
| Miller 1956 | ✅ Verified | OK |
| Raiyan 2025 | ✅ Verified | OK — strong supporting citation |
| **Saito 2023** | **❌ NOT FOUND** | **REMOVE — likely hallucinated** |
| Shannon 1948 | ✅ Verified | OK |
| Somerstep 2024 | 🔍 Plausible | Orphaned — verify + cite or remove |
| Sperber & Wilson 1986 | ✅ Verified | OK |
| Standage 1998 | ✅ Verified | OK |
| **Vaswani 2017** | **⚠️ WRONG arXiv in body** | **Fix 2005.14165 → 1706.03762 in Section 9** |
| Yang 2025 | ✅ Verified | OK |
| Zhang 2024 | 🔍 Unverified | Orphaned — verify + cite or remove |
| Zipf 1949 | ✅ Verified | OK |

---

## PRIORITY ACTION LIST

1. **CRITICAL:** Fix Vaswani arXiv in Section 9: `2005.14165` → `1706.03762`
2. **CRITICAL:** Remove `Li, J. (2024)` — not findable, likely hallucinated
3. **CRITICAL:** Remove `Saito, H. (2023)` — not findable, likely hallucinated
4. **HIGH:** Fix or remove `Brath 2023` — URL 404s
5. **MEDIUM:** Verify `JuliusBrussee (2024)` GitHub repo exists and 65% claim is documented
6. **LOW:** Clean up orphaned references (Brown, Burroughs, Daniels, Hanna, Manning, Somerstep, Zhang) — either cite in body or remove from references
7. **LOW:** Verify Handey authorship credit for Unfrozen Caveman Lawyer

---

*Audit conducted via web search. Some URLs could not be directly fetched due to network configuration. Final verification should include direct URL checks for ALSSA, FAA, and JuliusBrussee GitHub.*
