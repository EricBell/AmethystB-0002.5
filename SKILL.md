---
name: medical-billing-em-audit-cms-medicare
description: Use this skill when auditing outpatient professional medical billing under CMS/Medicare office and outpatient E/M rules. Review the encounter note and the billing document together, score MDM one element at a time, and determine whether the billed code and any add-on code are supported.
---

# CMS / Medicare Outpatient E/M Audit Skill (2021–2025)

## Purpose
Use this skill to audit office or outpatient E/M charges using:
- the encounter note, and
- the billing statement.

The goal is simple:
**Does the documentation support what was billed?**

Write an **audit findings report**, not a summary or opinion.



## Core principles

- The **note controls the code**, not the bill.
- Do not assume the billed level is correct.
- Do not stretch documentation to justify a higher level.
- If documentation is thin or mixed, score conservatively.
- Separate **what is mentioned** from **what is actually managed**.



## Workflow

### 1) Identify what was billed
From the billing statement:
- confirm date of service,
- identify billed E/M code (or description),
- identify any add-on codes (e.g., G2211).

Map descriptions carefully if codes are not shown.



### 2) Use the correct framework
- Use **2021–2025 CMS outpatient E/M rules**
- Use **MDM**, not time (unless the note explicitly supports time)
- For established patients, apply the correct E/M code family



### 3) Build the real problem list

List every issue, then sort into:

- **Actively addressed (counts toward MDM)**
- Mentioned but not meaningfully managed
- History/background only
- Resolved or inactive
- Patient speculation without clinical action

Key question:
**What did the provider actually do about this problem today?**



## 4) Score MDM elements separately

### A. Number and Complexity of Problems Addressed

This is where most errors happen. Be strict.

#### What counts
Only include problems that are **actively evaluated or managed**.

Examples:
- Stable chronic illness **with evaluation or management**
- Acute illness addressed at the visit
- Chronic illness with exacerbation **and active management**
- New problem with real diagnostic or management work



#### What does NOT meaningfully count

Do NOT use these to raise the level:

- Stable conditions with “continue current management”
- Monitoring-only problems
- Resolved conditions
- Symptoms with no management decision
- Conditions listed in history or med list only
- Patient concerns without clinical action



#### Moderate vs Low — the key rule

**Do NOT reach Moderate by stacking weak problems.**

Moderate Problems requires:
- At least **one problem that clearly drives management at a higher level**, OR
- Multiple problems that each require meaningful work



#### Practical guardrails

- If most problems are “stable,” “monitor,” or “no change” → **LOW**
- A single “exacerbation” without treatment change is often still **LOW**
- A medication follow-up visit is often **LOW** unless complexity is clear

Ask:
**Did anything meaningful change today because of this problem?**



#### Critical rule

**Multiple low-level problems do NOT combine into Moderate.**

If no single problem clearly supports Moderate complexity:
→ Score **LOW**



### B. Amount and/or Complexity of Data

Count only what is clearly documented.

#### Counts:
- External note review
- Test ordering or review
- Independent historian
- Independent interpretation
- Discussion with another clinician

#### Does NOT count:
- General familiarity with patient
- Mention of prior care
- Referral plans or self-referral
- Medication list or vitals alone

If not clearly documented:
→ **Minimal or None**



### C. Risk of Complications and/or Morbidity or Mortality

Focus on **management decisions made today**.

#### Moderate risk commonly includes:
- **Prescription drug management**

This includes:
- starting,
- renewing,
- adjusting,
- or actively managing a prescription



#### Important distinction

**Prescription management affects RISK — not automatically PROBLEMS**

Do NOT upgrade the Problems element just because a prescription was written.



#### Do not over-read risk

- OTC use alone → not moderate
- Historical risk → does not count
- Medication listed without management → weak



## 5) Apply the 2-out-of-3 rule

Overall MDM level = highest level met by **at least 2 of 3 elements**.

- One strong element does NOT control the visit
- Do not override the rule



## 6) Evaluate add-on codes separately

Do not assume a valid E/M code supports an add-on code.



### G2211 (Medicare complexity add-on)

Requires documentation showing:

- Ongoing, longitudinal care relationship **AND**
- Visit complexity tied to being the focal point for care



#### Not sufficient by itself:

- Provider specialty (e.g., PCP)
- Multiple diagnoses listed
- Routine follow-up visit
- Prescription renewal (including controlled substances)
- Detailed note without clear complexity



#### Practical rule

If the note does not clearly show:
- longitudinal responsibility, OR
- care of a serious/complex condition

→ **G2211 is unsupported**



## 7) Write the audit report

Use this structure:

### 1. Medical Decision Making (MDM) Analysis
- Problems
- Data
- Risk

For each:
- state supported level
- explain why higher level is NOT supported if relevant



### 2. E/M Level Determination
- Apply 2-out-of-3 rule
- State whether billed code is supported
- If not, give correct level



### 3. Add-on Code Compliance
- Evaluate separately
- State clearly: supported or unsupported
- Explain why



### 4. Final Conclusion

- Billed E/M code
- Supported E/M code
- Add-on code status
- One-line basis



## Common mistakes to avoid

### 1) Counting everything as a problem
Narrative ≠ management



### 2) Stacking weak problems
Stable + monitor + history ≠ Moderate



### 3) Letting one element drive the visit
Risk alone does not determine level



### 4) Treating prescription as automatic Moderate overall
It supports **Risk only**



### 5) Treating referrals as data
Planning a referral ≠ reviewing data



### 6) Assuming add-on codes are automatic
They require separate support



### 7) Missing the “active vs passive” distinction
Only active management counts



## Final check before answering

- Did you identify the billed code?
- Did you confirm the date of service matches?
- Did you separate active vs passive problems?
- Did you score Problems, Data, Risk separately?
- Did you apply 2-of-3 rule correctly?
- Did you avoid using time unless supported?
- Did you review add-on code separately?
- Did you explain why higher level is NOT supported?



## Tone

- Write like a medical auditor
- Be direct and practical
- Do not overstate
- Stay grounded in the note



## Default closing

- **Billed E/M code:** [code]
- **Supported E/M code:** [code]
- **Add-on code:** [supported / unsupported]
- **Basis:** [short explanation]