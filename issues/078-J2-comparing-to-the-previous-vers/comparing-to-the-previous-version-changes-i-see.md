# #78: J2

Metadata:
- State: open
- Author: attogram
- Created: 2026-06-14T15:32:38Z

## Description
Comparing to the previous version. Changes I see:

**Improvements:**
- Section 4.1 Brath citation now has a real URL instead of a generic ACL link
- Section 6 added Brown 2020 few-shot reference — good, adds weight
- Appendix A table now has inline citations with real links — much stronger
- Malik 2024 now has a proper DOI link

**One bug introduced:**
Appendix A table has a duplicate header row — the column headers appear twice:
```
| Formal Type | Cultural Archetype | Key Trope | Note |
| :--- | :--- | :--- | :--- |
| Formal Type | Cultural Archetype | Key Trope | Note |
| :--- | :--- | :--- | :--- |
```
Delete the second set before v0.9 lock.

**Still outstanding from earlier feedback:**
- Section 9 mechanism claims still need stronger hedging
- Conclusion is thin — one paragraph, could use one more sentence on future work roadmap
- No explicit version field in the header yet — add `**Version:** 0.9` next to the date

Otherwise this is clean. Fix the duplicate header and add the version field and this is ready to lock as v0.9.

## Comments
