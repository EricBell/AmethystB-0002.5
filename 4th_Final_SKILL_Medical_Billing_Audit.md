---
name: medical-billing-em-audit-cms-medicare
description: Use this skill when auditing outpatient professional medical billing under CMS/Medicare office and outpatient E/M rules. Review the encounter note and the billing document together, score MDM one element at a time, separate active management from background narrative, and decide whether the billed code and any add-on code are supported.
---

# CMS/Medicare Outpatient E/M Audit Skill

## What this skill is for
Use this skill to perform a coding and compliance review of outpatient professional charges using the encounter note and the billing document.

The job is to decide whether the billed code or codes are supported by the documentation. The output should be an audit findings report, not a patient complaint, appeal letter, casual summary, or medical opinion.

This skill is a good fit when the file set includes:
- a clinic or office note,
- a bill, statement, or charge sheet,
- a question about office or outpatient E/M coding,
- a question about a Medicare add-on code,
- instructions to use CMS or Medicare office visit rules.

## Basic approach
Work from a strict documentation standard.

- A code is supported only when the note supports it.
- Do not assume the billed code is correct.
- Do not stretch the documentation to save a higher code.
- If the note is thin, mixed, or unclear, score conservatively.
- Separate what is simply mentioned from what is actually evaluated or managed.

The main question is: **What level is supported by the written note?**

## Workflow

### 1) Start with the billing question
Pull the billing details from the statement before scoring the note:
- date of service,
- billed line items,
- charge descriptions,
- likely CPT or HCPCS codes,
- dollar amounts if shown.

State plainly which code or codes are being reviewed.

If the bill uses descriptions instead of code numbers, map them carefully. Do not drift into unrelated charges unless the task asks for that.

### 2) Pick the coding framework
For office or outpatient E/M reviews under current CMS rules:
- Use the **2021-2025 office and outpatient E/M framework**.
- For established patients, use the correct established-patient office visit code family.
- If the assignment says to review by **MDM**, use MDM and not time.
- Only mention time if the note itself gives usable total-time language. Do not use wording from the bill alone as time support.

### 3) Build the real problem list
List every issue mentioned in the note, then sort each one into a bucket:
- **Actively addressed and relevant to MDM**
- **Mentioned but not meaningfully managed**
- **History or background only**
- **Resolved or not active**
- **Patient speculation or symptom mention without real coding weight**

This step matters. Weak reviews often go wrong by counting every clinical sentence as if it supports the code.

### 4) Score the MDM elements one by one
For office and outpatient E/M, score these separately:
- Number and Complexity of Problems Addressed
- Amount and/or Complexity of Data to be Reviewed and Analyzed
- Risk of Complications and/or Morbidity or Mortality of Patient Management

Do not blur them together.

### 5) Use the 2-out-of-3 rule
The overall MDM level is the highest level met by **at least two of the three elements**.

One higher-scoring element does not control the whole visit by itself.

### 6) Review add-on codes on their own
Do not assume a valid base E/M code automatically supports an add-on code.

If an add-on code is billed, review it separately under the applicable Medicare standard.

### 7) Write the audit report
Give a structured audit findings report with clear reasoning. Keep the report focused on the billed code review requested in the assignment.

## Output format
Unless the user asks for a different format, write the answer in Markdown as an **Audit Findings Report** with these sections:

### 1. Medical Decision Making (MDM) Analysis
Analyze the three required MDM elements separately:
- **Problems Addressed**
- **Data Reviewed and Analyzed**
- **Risk of Patient Management**

For each element:
- identify the documented facts that count,
- state the supported level,
- explain why a higher level is not supported if relevant.

### 2. E/M Level Determination
State whether the documentation supports the billed E/M code.

If not, state the appropriate supported level based on the MDM analysis.
Apply the 2-out-of-3 rule directly and explain the result in clear audit language.

### 3. Add-on Code Compliance
If an add-on code is under review, evaluate it separately.

State whether the documentation satisfies the reporting requirements for that add-on code and explain why or why not.

### 4. Final Conclusion
End with a brief final conclusion that states:
- whether the billed E/M code is supported,
- the supported E/M code if different,
- whether the add-on code is supported or unsupported.

Do not add extra sections unless the assignment asks for them.

## Scoring guidance

### A. Number and Complexity of Problems Addressed
Count only problems that are actually addressed during the visit in a way that contributes to MDM.

#### Problems that often count
- a stable chronic illness that is evaluated or managed at the visit,
- an acute uncomplicated illness or injury that is evaluated or managed,
- a chronic illness with exacerbation, progression, or treatment side effect when the note really shows that,
- an undiagnosed new problem with uncertain prognosis when the note shows real diagnostic uncertainty and management.

#### Things not to over-count
- diagnoses listed only in history,
- resolved or historical conditions with no active work,
- casual symptom mention with no real management,
- patient guesses unless the clinician actually adopts and works through that uncertainty,
- chronic conditions that only appear on the med list,
- broad lifestyle discussion with no coding consequence.

#### Practical rules
- A resolved issue plus simple observation usually should not be inflated into a significant active problem.
- A stable chronic illness stays stable unless the note shows exacerbation, progression, or treatment side effects.
- A new symptom that is mild, not dangerous, and only monitored is often lower-level rather than moderate.
- History of a condition is not the same as a current exacerbation.
- Letting the patient monitor symptoms, continue the same conservative plan, or seek care later if needed is not automatically moderate problem complexity.

A useful question is: **What real management work happened today for this problem?**

### B. Amount and/or Complexity of Data to be Reviewed and Analyzed
Score data conservatively.

#### Count data only when the note shows it
Examples:
- external note review,
- test review or ordering,
- independent historian,
- independent interpretation,
- discussion with an outside physician or other qualified healthcare professional.

#### Do not count
- general familiarity with the patient,
- mention of prior care without current review,
- a future idea of seeing a specialist,
- medication list or vitals by themselves,
- a problem mention without any qualifying data work.

If the note does not show qualifying data work, this element is **minimal or none**.

### C. Risk of Complications and/or Morbidity or Mortality of Patient Management
This element is about the risk tied to management decisions made at the encounter.

#### Common moderate-risk trigger
- **Prescription drug management** usually supports **moderate risk**.

That can include starting, renewing, adjusting, or actively managing a prescription medication when the note shows that management as part of the visit.

#### Do not over-read risk
- OTC advice alone is not prescription management.
- A medication listed in the chart is weaker than actual visit-level management.
- Historical risk factors do not automatically raise today’s risk element.

If prescription management is clearly documented, moderate risk may be supported for the **risk element** even when the overall MDM remains lower.

## Established patient E/M guardrails
Use the MDM result, not your gut.

A common weak-documentation pattern is when only one of the three MDM elements reaches a higher level. In that situation, the overall MDM does not rise to that higher level because the 2-out-of-3 rule still controls.

Do not let one stronger element outweigh two weaker ones.

## Add-on code guidance
Treat any add-on code as a separate compliance question.

### What to look for
The note should support the specific standard for the add-on code being billed. For Medicare complexity-based add-on codes, look for documentation that actually shows the required ongoing care relationship, longitudinal management, or inherent visit complexity.

### What is not enough by itself
- the provider specialty alone,
- multiple diagnoses listed in the chart,
- a routine follow-up,
- a prescription being renewed,
- a note that feels detailed,
- broad assumptions about the provider-patient relationship.

### Default stance
If the encounter note does not clearly show the required basis for the add-on code, treat the add-on as **unsupported**.

## Bill-versus-note rules
When you have both the note and the bill:
- confirm that the billed lines match the codes being discussed,
- confirm that the **date of service** matches across the documents,
- use the note to decide support,
- use the bill to show what was charged,
- if a charge is tied to an unsupported code, say so plainly if the task is bill-focused.

## Common mistakes to avoid

### 1) Counting narrative clutter as coding support
Examples:
- resolved or historical conditions,
- old history,
- lifestyle talk,
- speculative causes,
- symptom discussion without management value.

### 2) Upgrading a problem because it sounds serious in plain English
Coding categories are narrower than ordinary language. “New” does not automatically mean moderate. “Chronic” does not automatically mean complex. “Pain” does not automatically mean exacerbation.

### 3) Letting one element decide the whole visit
A higher score in one element does not determine the overall MDM. The overall level still depends on the 2-out-of-3 rule.

### 4) Treating a possible referral as data
A referral idea, self-referral discussion, or specialist history is not the same as reviewing outside records or discussing management with an outside clinician.

### 5) Treating an add-on code as automatic
It is not automatic. The note still has to support the specific Medicare or payer standard for the add-on.

### 6) Writing the wrong kind of deliverable
Do not default to a patient letter, insurer appeal, generic summary, SOAP note, or casual opinion unless the user asks for that format. The default product here is an **audit findings report**.

## Final check before you answer
Before finishing, make sure all of these are true:

- Did you identify the billed code or descriptor from the statement?
- Did you confirm the note and bill match the same date of service?
- Did you separate active problems from non-countable note clutter?
- Did you score **Problems**, **Data**, and **Risk** separately?
- Did you apply the **2-of-3** rule directly?
- Did you avoid using time unless the note actually supports it?
- Did you review any add-on code separately from the base E/M code?
- Did you explain not only what is supported, but why the higher billed level is not?
- Did you write an audit findings report instead of a generic answer?

If not, revise before finalizing.

## Tone
- Write like a coding or compliance reviewer, not like a lawyer or marketer.
- Be direct, specific, and grounded in the note.
- Keep the wording clean and practical.
- Do not overstate.
- Do not cite rules you were not asked to use.

## Default closing format
End with a brief summary such as:
- **Billed E/M code:** [billed code or descriptor]
- **Supported E/M code:** [supported code]
- **Add-on code:** [supported / unsupported / not billed]
- **Basis:** [one sentence tying the result to the MDM pattern and any add-on code analysis]
