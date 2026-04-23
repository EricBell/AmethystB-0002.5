---
name: cms-em-audit-established-office-g2211
description: Use this skill when reviewing outpatient professional billing under CMS/Medicare E/M rules, especially established office visits (99212-99215) and HCPCS G2211. Read the note and the bill together, score MDM one element at a time, separate real management from background narrative, and decide whether the billed codes are actually supported.
---

# CMS/Medicare Outpatient E/M Audit Skill

## What this skill is for
Use this skill to do a coding/compliance review of outpatient professional charges using the encounter note and the billing document.

The job is not to write a patient complaint, an appeal letter, or a casual summary. The job is to review the documentation the way a coding or compliance person would and decide whether the billed CPT/HCPCS code is supported.

This skill is a good fit when the file set includes:
- a clinic or office note,
- a bill, statement, or charge sheet,
- a question about office/outpatient E/M coding,
- a question about G2211,
- instructions to use CMS / Medicare / 2021-2025 E/M rules.

---

## Basic approach
Work from a strict documentation standard.

- A code is supported only when the note supports it.
- Do not assume the billed code is correct.
- Do not stretch the documentation to save a higher code.
- If the note is thin, mixed, or unclear, score conservatively.
- Separate what is simply mentioned from what is actually evaluated or managed.

The main question is: **What level is supported by the written note?**

---

## Workflow

### 1) Start with the billing question
Before you score the note, pull the billing details from the statement:
- date of service,
- billed line items,
- charge descriptions,
- likely CPT/HCPCS codes,
- dollar amounts if shown.

Say plainly which code or codes are being reviewed.

If the bill uses descriptions instead of code numbers, map them carefully. Examples:
- “Office/Outpatient Established ... Mod Mdm 30 Min” usually points to **99214**.
- “Complex e/m visit add on” usually points to **G2211**.

Do not drift into other charges unless the prompt asks for that.

### 2) Pick the coding framework
For office/outpatient E/M reviews under current CMS rules:
- Use the **2021-2025 office/outpatient E/M framework**.
- For established patients, the code family is **99212-99215**.
- If the assignment says to review by **MDM**, use MDM and not time.
- Only mention time if the note itself gives usable total-time language. Do not use wording from the bill alone as time support.

### 3) Build the real problem list
List every issue mentioned in the note, then sort each one into a bucket:
- **Actively addressed and relevant to MDM**
- **Mentioned but not meaningfully managed**
- **History/background only**
- **Resolved / not active**
- **Patient speculation or symptom mention without real coding weight**

This step matters. A weak review often goes wrong by counting every clinical sentence as if it supports the code.

### 4) Score the MDM elements one by one
For office/outpatient E/M, score these separately:
- Number and Complexity of Problems Addressed
- Amount and/or Complexity of Data to be Reviewed and Analyzed
- Risk of Complications and/or Morbidity or Mortality of Patient Management

Do not blur them together.

### 5) Use the 2-out-of-3 rule
The overall MDM level is the highest level met by **at least two of the three elements**.

That rule is the center of the review. One moderate element does not make the whole visit moderate.

### 6) Review add-on codes on their own
Do not assume a valid base E/M code automatically supports an add-on code.

For **G2211**, do a separate Medicare review. It has its own support test.

### 7) Write the audit report
Give a structured audit report with clear reasoning. Do not give a vague impressionistic answer.

---

## Output format
Unless the user asks for something else, write the answer in Markdown with these sections in this order:

1. **Audit Header**
   - Date of service
   - Encounter source(s) reviewed
   - Billing source(s) reviewed
   - Codes/charges reviewed

2. **Executive Summary**
   - 2-5 sentences
   - State the E/M level that is supported
   - State whether any add-on code is unsupported

3. **Methodology / Standards Used**
   - Say that the review used the **2021-2025 CMS office/outpatient E/M rules**
   - Say that MDM was reviewed by the three required elements and the 2-of-3 rule
   - If G2211 is involved, say that it was reviewed separately under Medicare guidance

4. **Charge Reconciliation**
   - Briefly map the bill wording to the CPT/HCPCS code and amount

5. **MDM Element Review**
   - Separate subsection for:
     - Problems Addressed
     - Data Reviewed and Analyzed
     - Risk of Patient Management
   - In each subsection:
     - point to the documented facts,
     - state the supported level,
     - explain why the higher level is not supported.

6. **Overall E/M Level**
   - Apply the 2-of-3 rule directly
   - State whether the billed E/M code stands or should change

7. **Clinical-to-Coding Correlation Table**
   - A compact table that links note facts to coding impact

8. **G2211 Review**
   - Keep this separate from the E/M section
   - State whether the note shows the kind of longitudinal or inherently complex care Medicare is looking for

9. **Final Determination / Recommended Adjustment**
   - State the final coding conclusion
   - If the job is bill-focused, state which charge should be challenged or adjusted

---

## Scoring guidance

## A. Number and Complexity of Problems Addressed
Count only problems that are actually addressed during the visit in a way that contributes to MDM.

### Problems that often count
- a stable chronic illness that is evaluated or managed at the visit,
- an acute uncomplicated illness or injury that is evaluated or managed,
- a chronic illness with exacerbation, progression, or treatment side effect when the note really shows that,
- an undiagnosed new problem with uncertain prognosis when the note shows real diagnostic uncertainty and management.

### Things not to over-count
- diagnoses listed only in history,
- resolved issues with no active work,
- casual symptom mention with no real management,
- patient guesses such as “maybe it is a pinched nerve” unless the clinician actually adopts and works through that uncertainty,
- chronic conditions that only appear on the med list,
- broad age-related or lifestyle discussion with no coding consequence.

### Practical rules
- A **resolved problem** plus simple observation usually should not be inflated into a significant active problem.
- A **stable chronic illness** stays stable unless the note shows exacerbation, progression, or treatment side effects.
- A **new symptom** that is mild, not dangerous, and only monitored is often low-level rather than moderate.
- A history of chronic pain is not the same as a currently exacerbated chronic illness.
- Letting the patient watch symptoms, continue the same conservative plan, or self-refer is not automatically moderate problem complexity.

A useful question is: **What real management work happened today for this problem?**

## B. Amount and/or Complexity of Data Reviewed and Analyzed
Score data conservatively.

### Count data only when the note shows it
Examples:
- external note review,
- test review or ordering,
- independent historian,
- independent interpretation,
- discussion with an outside physician or other QHP.

### Do not count
- general familiarity with the patient,
- mention of prior care without current review,
- a future idea of seeing a specialist,
- self-referral talk without documented data review,
- medication list or vitals by themselves,
- a problem mention without any qualifying data work.

If the note does not show qualifying data work, this element is **minimal or none**.

## C. Risk of Complications and/or Morbidity or Mortality of Patient Management
This element is about the risk tied to management decisions made at the encounter.

### Common moderate-risk trigger
- **Prescription drug management** usually supports **moderate risk**.

That can include starting, renewing, adjusting, or actively managing a prescription medication when the note shows that management as part of the visit.

### Do not over-read risk
- OTC advice alone is not prescription management.
- A medication listed in the chart is weaker than actual visit-level management.
- Old scary events or historical risk factors do not automatically raise today’s risk element.

If prescription management is clearly documented, moderate risk may be supported even when the other two elements are lower.

---

## Established patient E/M guardrails
Use the MDM result, not your gut.

A common weak-documentation pattern is:
- Problems = low
- Data = minimal/none
- Risk = moderate

That pattern supports **overall low MDM**, because only one element reaches moderate.

Do not let moderate risk from prescription management pull the whole visit up to 99214 by itself.

If the billed code matches **moderate MDM** but the note only supports **low MDM**, recommend the lower established-patient office code.

---

## G2211 guidance
Treat **G2211** as a separate Medicare question.

### What to look for
The note should support that the visit is part of care where the practitioner is the continuing focal point for the patient’s needed health care services, or for ongoing care tied to a single serious or complex condition, with the kind of **longitudinal or inherent complexity** Medicare is talking about.

### What is not enough by itself
- the provider is primary care,
- the patient has several chronic diagnoses on the chart,
- the visit is a routine follow-up,
- a prescription gets renewed,
- a few chronic issues are mentioned,
- the note feels thorough.

### Default stance
If the encounter note does not clearly show that longitudinal or inherent-complexity basis, treat G2211 as **unsupported**.

Do not save G2211 with broad assumptions about the provider-patient relationship if the visit note does not show the needed complexity context.

---

## Bill-versus-note rules
When you have both the note and the bill:
- confirm that the billed lines match the codes being discussed,
- keep the review tied to the correct date of service,
- use the note to decide support,
- use the bill to show what was charged,
- if a charge is tied to an unsupported code, say so plainly if the task is bill-focused.

---

## Common mistakes to avoid

### 1) Counting narrative clutter as coding support
Examples:
- resolved pain,
- old history,
- lifestyle talk,
- speculative causes,
- symptom discussion without management value.

### 2) Upgrading a problem because it sounds serious in plain English
Coding categories are narrower than ordinary language. “New” does not automatically mean moderate. “Chronic” does not automatically mean complex. “Pain” does not automatically mean exacerbation.

### 3) Giving moderate E/M just because prescription management is present
Prescription management often makes **risk** moderate, but the overall visit still depends on **two of the three** MDM elements.

### 4) Treating a possible referral as data
A referral idea, self-referral discussion, or specialist history is not the same as reviewing outside records or discussing management with an outside clinician.

### 5) Treating G2211 as automatic in primary care
It is not automatic. The note still has to support the Medicare-specific complexity idea.

### 6) Writing the wrong kind of deliverable
Do not default to a patient letter, insurer appeal, generic summary, SOAP note, or casual opinion unless the user asks for that format. The default product here is an **audit findings report**.

---

## Final check before you answer
Before finishing, make sure all of these are true:

- Did you identify the billed code or descriptor from the statement?
- Did you separate active problems from non-countable note clutter?
- Did you score **Problems**, **Data**, and **Risk** separately?
- Did you apply the **2-of-3** rule directly?
- Did you avoid using time unless the note actually supports it?
- Did you review **G2211 separately** from the base E/M code?
- Did you explain not only what is supported, but why the higher billed level is not?
- Did you write an audit report instead of a generic answer?

If not, revise before finalizing.

---

## Tone
- Write like a coding/compliance reviewer, not like a lawyer or marketer.
- Be direct, specific, and grounded in the note.
- Keep the wording clean and practical.
- Do not overstate.
- Do not cite rules you were not asked to use.

---

## Default closing format
End with this kind of summary:
- **Supported E/M code:** [code]
- **Billed E/M code:** [code or descriptor]
- **Recommendation:** uphold / downcode / insufficient support
- **G2211:** supported / unsupported
- **Basis:** one sentence tying the result to the MDM pattern and any lack of G2211 support
