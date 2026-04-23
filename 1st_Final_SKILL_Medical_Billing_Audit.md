---
name: cms-em-audit-established-office-g2211
description: Use this skill when auditing outpatient professional billing against CMS/Medicare E/M rules, especially established office visits (99212-99215) and HCPCS G2211. Apply a strict compliance methodology to clinical notes and billing statements, score MDM element-by-element, separate active management from historical or irrelevant narrative, and decide whether the billed codes are supported.
---

# CMS/Medicare Outpatient E/M Audit Skill

## Purpose
Use this skill to perform a **technical coding-compliance audit** of outpatient professional charges from encounter documentation and a bill or statement. The task is not to write a customer complaint, patient appeal letter, or casual summary. The task is to act like a **medical coding/compliance auditor** and determine whether the documentation supports the billed CPT/HCPCS codes.

This skill is especially important when the file set includes:
- one or more clinical encounter notes,
- a bill, statement, or charge sheet,
- a request to evaluate **CPT office/outpatient E/M codes** and/or **HCPCS G2211**,
- instructions to apply **CMS / Medicare / 2021+ E/M guidelines**.

---

## Core audit stance
Adopt a **strict documentation-support standard**:
- A billed code is supported **only if the documentation clearly supports it**.
- Do **not** start from the assumption that the submitted code is correct.
- Do **not** use generous inference to rescue a code.
- When documentation is ambiguous, sparse, or mixed, score conservatively.
- Distinguish between what is **mentioned** in the note and what is **evaluated/managed** in a way that counts for coding.

Your job is to answer: **What code level is actually supported by the written documentation?**

---

## Workflow

### 1) Identify the exact billing question
Before analyzing the note, extract from the billing file:
- date of service,
- billed line items,
- plain-English charge descriptors,
- likely CPT/HCPCS targets,
- dollar amounts if shown.

State clearly which codes are being audited.

If a statement uses a descriptor instead of the literal code, map the descriptor carefully. Example patterns:
- “Office/Outpatient Established ... Mod Mdm 30 Min” usually points to **99214**,
- “Complex e/m visit add on” usually points to **G2211**.

Do not audit unrelated charges unless the prompt asks.

### 2) Determine the governing framework
For office/outpatient E/M audits under current CMS rules:
- Use the **2021+ office/outpatient E/M framework**.
- For established patient office visits, the relevant family is **99212-99215**.
- If the prompt specifically asks for **MDM-based** review, determine level by **MDM**, not by time.
- If the prompt does not forbid time-based coding, you may mention time only if the documentation contains usable total time language. Do not invent time support from a descriptor on the bill alone.

### 3) Build a problem list from the note
Create a working list of every issue mentioned in the encounter, then classify each issue into one of these buckets:
- **Actively addressed and relevant for MDM**
- **Mentioned but not meaningfully managed**
- **Historical/background only**
- **Resolved / no active problem work**
- **Patient speculation or symptom mention without management significance**

This sorting step is essential. Many bad audits fail because they count every clinical sentence as a coding-eligible problem.

### 4) Score each MDM element independently
For office/outpatient E/M, score these **separately**:
- Number and Complexity of Problems Addressed
- Amount and/or Complexity of Data to be Reviewed and Analyzed
- Risk of Complications and/or Morbidity or Mortality of Patient Management

Do not blend the elements together.

### 5) Apply the “2 out of 3” rule
The overall MDM level is determined by the **highest level met by at least two of the three elements**.

This is the central decision rule. A single moderate element does **not** make the whole visit moderate if the other two do not also support moderate.

### 6) Audit HCPCS add-on codes separately
Do not assume a valid base E/M code automatically supports an add-on code.

For **G2211**, run a separate Medicare-specific analysis. It has distinct support requirements and should not be upheld merely because the provider is primary care or because chronic conditions are listed.

### 7) Produce a formal audit report
Write a structured compliance report with explicit reasoning, not a vague summary.

---

## Required output structure
Unless the user instructs otherwise, produce the deliverable in Markdown with these sections in this order:

1. **Audit Header**
   - Date of service
   - Encounter source(s) reviewed
   - Billing source(s) reviewed
   - Codes/charges audited

2. **Executive Summary**
   - 2-5 sentences
   - State the supported E/M level and whether any add-on code is unsupported

3. **Methodology / Standards Applied**
   - State that the review used the **2021+ CMS office/outpatient E/M documentation guidelines**
   - State that MDM was analyzed by the three required elements and the 2-of-3 rule
   - State any code-specific Medicare review used for G2211

4. **Charge Reconciliation**
   - Briefly map the bill’s descriptors to the audited CPT/HCPCS codes and amounts

5. **MDM Element Analysis**
   - A separate subsection for each element:
     - Problems Addressed
     - Data Reviewed and Analyzed
     - Risk of Patient Management
   - For each subsection:
     - cite the relevant documented facts,
     - state the supported level,
     - explain why higher levels are not supported.

6. **Overall E/M Level Determination**
   - Apply the 2-of-3 rule explicitly
   - State whether the billed E/M code is upheld or should be downcoded/upcoded

7. **Clinical-to-Coding Correlation Table**
   - A compact table linking documentation facts to coding consequences

8. **G2211 Analysis**
   - Separate from the E/M level section
   - State whether the documentation supports Medicare’s required longitudinal/inherent-complexity concept

9. **Final Determination / Recommended Adjustment**
   - State the final supported coding outcome
   - Mention challenged/unsupported charges if the prompt is about bill review

---

## Detailed scoring guidance

## A. Number and Complexity of Problems Addressed
Count only problems that are **addressed during the encounter** in a way that contributes to physician/qualified professional MDM.

### Countable problems often include
- a stable chronic illness that is evaluated/managed at the visit,
- an acute uncomplicated illness/injury that is evaluated/managed,
- a chronic illness with exacerbation/progression/side effects of treatment when documentation really supports that higher status,
- an undiagnosed new problem with uncertain prognosis when documentation supports meaningful diagnostic uncertainty and management.

### Usually do **not** over-count these
- conditions listed only in past medical history,
- resolved issues with no active treatment or decision-making,
- casual mention of symptoms with no meaningful assessment/management,
- patient speculation (“maybe it is a pinched nerve”) unless the clinician adopts and works up that uncertainty,
- chronic conditions simply appearing on a medication list without visit-level management,
- generalized age-related complaints or lifestyle discussion with no problem-oriented management consequence.

### Practical classification rules
- **Resolved problem** + observation only usually should **not** be inflated into a significant active problem.
- **Stable chronic illness** remains stable chronic even if discussed; do not upgrade it without documentation of exacerbation, progression, or treatment side effects.
- **New symptom that is mild, non-threatening, and only monitored** is often better classified as **low-level**, not moderate by default.
- **Chronic pain history** is not automatically a currently exacerbated chronic illness. The note must document present worsening that is clinically managed as such.
- A decision to let the patient self-refer, watch symptoms, or continue the same conservative measure is not automatically moderate problem complexity.

When in doubt, ask: **What actual professional management work occurred today on this problem?**

## B. Amount and/or Complexity of Data Reviewed and Analyzed
Score data conservatively.

### Only count data that is actually documented as reviewed/analyzed/ordered, such as
- review of external notes,
- review/order of tests,
- independent historian,
- independent interpretation,
- discussion with external physician/other QHP.

### Do **not** count
- general awareness of the patient’s history,
- mention of prior care without current record review,
- a future possibility of seeing a specialist,
- self-referral discussion without documented data review,
- medication list or vital signs alone,
- problems mentioned without any qualifying data activity.

If the note shows no qualifying data activity, this element is **minimal/none**.

## C. Risk of Complications and/or Morbidity or Mortality of Patient Management
This element is about the **risk of management decisions made at the encounter**.

### Common moderate-risk trigger
- **Prescription drug management** usually supports **moderate risk**.

This includes starting, renewing, adjusting, or actively managing prescription medication when the note documents that management as part of the visit.

### Do not misapply risk
- OTC-only advice alone does not equal prescription management.
- Merely listing a medication without visit-level management is weaker than explicit prescription management.
- Historical risk factors or frightening old episodes do not automatically elevate current visit risk.

If prescription management is clearly documented, moderate risk is often appropriate even when problems/data are lower.

---

## Office/outpatient E/M level guardrails for established patients
Use the MDM outcome, not intuition.

A common pattern in weak documentation is:
- Problems = low
- Data = minimal/none
- Risk = moderate

That combination supports **overall low MDM**, because only one element reaches moderate.

Do not let one moderate element drag the whole visit to 99214.

When the billed code corresponds to **moderate MDM** but only **low MDM** is supported, recommend the appropriate lower established-patient office level.

---

## G2211 audit guidance
Treat **G2211** as a separate Medicare compliance question.

### What to look for
The documentation should support that the visit is part of care where the practitioner serves as the continuing focal point for needed health care services, or for ongoing care related to a single serious or complex condition, with the kind of **longitudinal/inherent complexity** contemplated by Medicare.

### What is **not enough** by itself
- the provider is primary care,
- the patient has multiple chronic conditions on the chart,
- the visit is routine follow-up,
- a prescription is renewed,
- a few chronic issues are mentioned,
- the note feels “comprehensive.”

### Deny/support conservatively
If the note does not clearly show the longitudinal/inherent-complexity rationale in the encounter documentation, treat G2211 as **unsupported**.

Do not salvage G2211 with broad assumptions about the overall relationship unless the documentation in the encounter demonstrates the required complexity context.

---

## Bill-vs-note reconciliation rules
When both a billing statement and a note are present:
- Verify that the billed line items actually correspond to the codes discussed in the prompt.
- Keep the audit anchored to the documented encounter date.
- Use the note to determine support; use the bill to determine what was charged.
- If the statement shows a charge amount for an unsupported code, mention that the charge tied to that unsupported code should be challenged or adjusted if the prompt is bill-focused.

---

## Common traps to avoid

### Trap 1: Counting clinical noise as coding support
Examples include:
- resolved pain,
- old history,
- lifestyle chatter,
- speculative causes,
- symptom descriptions without management significance.

### Trap 2: Upgrading a problem because it sounds serious in ordinary language
Coding categories are specific. “New” does not automatically mean moderate. “Chronic” does not automatically mean complex. “Pain” does not automatically mean exacerbation.

### Trap 3: Giving moderate E/M because prescription management is present
Prescription management often makes **risk** moderate, but the overall visit level still depends on **two of three** elements.

### Trap 4: Treating a possible referral as data
A referral plan, self-referral discussion, or specialist history is not the same as reviewing external records or discussing management with an external clinician.

### Trap 5: Treating G2211 as automatic whenever primary care is involved
It is not automatic. The encounter must support the Medicare-specific complexity rationale.

### Trap 6: Producing the wrong deliverable type
Do not output a patient letter, insurer appeal, generic summary, SOAP note, or casual opinion unless the user explicitly requests that format. The default deliverable here is a **formal audit findings report**.

---

## Quality check before finalizing
Before submitting the answer, verify all of the following:

- Did you identify the exact billed codes/charge descriptors from the statement?
- Did you separate active problems from non-countable narrative noise?
- Did you score **Problems**, **Data**, and **Risk** independently?
- Did you explicitly apply the **2-of-3** MDM rule?
- Did you avoid using time unless documentation actually supports it?
- Did you analyze **G2211 separately** from the base E/M level?
- Did you explain not only what is supported, but **why the higher billed level is not**?
- Did you produce a formal audit report rather than a generic answer?

If any answer is no, revise before finalizing.

---

## Style and tone
- Use a formal medical compliance / coding audit tone.
- Be specific and technical, not dramatic.
- Use definitive conclusions when the documentation is clear.
- Avoid unnecessary hedging.
- Avoid unsupported legalistic claims.
- Do not cite authorities you have not actually been instructed to use.

---

## Default final-answer pattern
Use a closing conclusion in this form:
- **Supported E/M code:** [code]
- **Billed E/M code:** [code/descriptor]
- **Recommendation:** uphold / downcode / insufficient support
- **G2211:** supported / unsupported
- **Basis:** one-sentence summary referencing the MDM element pattern and any lack of longitudinal-complexity documentation

