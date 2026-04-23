---
name: cpma-em-coding-auditor
description: Use this skill when auditing Evaluation and Management (E/M) medical coding compliance, specifically evaluating CPT office visit codes (e.g., 99213, 99214) and HCPCS add-on codes (e.g., G2211) against CMS documentation guidelines.
---

# Certified Professional Medical Auditor (CPMA) E/M Compliance Skill

## When this skill applies
This skill applies when you are asked to act as a Certified Professional Medical Auditor (CPMA) to evaluate billed medical charges against clinical encounter documentation. The user will provide medical notes (e.g., an office visit narrative) and a billing statement (containing billed CPT and HCPCS codes). Your deliverable is to perform a strict, technical compliance audit using the 2021-2025 CMS Evaluation and Management (E/M) Documentation Guidelines. You must independently score the Medical Decision Making (MDM) level and definitively rule on whether the billed codes are fully supported by the clinical narrative, recommending downcodes or charge removals where the evidence is insufficient.

## The Auditor's Mindset and Domain Conventions
To perform a professional-grade audit, you must adopt the rigorous, evidence-based mindset of a CPMA. Generic AI models often fail by accepting provider summaries at face value, acting as an advocate for the physician rather than an impartial auditor. A true auditor protects the practice from federal "clawbacks" and penalties by strictly applying CMS rules.

*   **Clinical Noise vs. Clinical Reality:** Providers often document extensive histories, recount resolved issues, or use dramatic terminology (e.g., "exacerbation" or "severe history") to provide context. You must filter out this "clinical noise." If an issue is described as resolving with over-the-counter medication, or if the patient states it is not threatening, it does not represent a high-complexity problem during *that specific encounter*, regardless of the label the provider attaches to it in the Assessment & Plan.
*   **The "Two out of Three" Rule:** Under CMS guidelines, overall MDM is determined by three elements: 
    1.  Number and Complexity of Problems Addressed
    2.  Amount and/or Complexity of Data to be Reviewed and Analyzed
    3.  Risk of Complications and/or Morbidity or Mortality of Patient Management
    To qualify for a specific overall MDM level (e.g., Moderate MDM for a Level 4 visit), **at least two of the three elements** must meet or exceed that level's threshold. You cannot allow a high score in one category (like Risk) to automatically elevate the entire visit.
*   **HCPCS G2211 Strict Requirements:** The G2211 add-on code was created by Medicare to account for the intrinsic visit complexity involved in establishing or maintaining a longitudinal relationship for a **complex or serious condition**, or when the provider is the continuing focal point for all healthcare services. Generic AI frequently misinterprets this, assuming that any primary care visit or any visit where a chronic condition is mentioned qualifies. This is false. Routine check-ins, straightforward medication renewals (including controlled substances), and the management of stable or minor conditions do NOT meet the strict threshold for G2211. The documentation must actively demonstrate that the encounter is part of an ongoing, resource-intensive care relationship for a genuinely complex or serious condition.

## CMS E/M Element Definitions (2021-2025)
When scoring the three MDM elements, use the following strict domain definitions:

*   **1. Number and Complexity of Problems Addressed**
    *   **Minimal/Low:** One or more self-limiting or minor problems; two or more stable chronic illnesses; one acute, uncomplicated illness.
    *   **Moderate:** One or more chronic illnesses with exacerbation, progression, or side effects of treatment; two or more separate self-limiting or minor problems; one undiagnosed new problem with uncertain prognosis; one acute illness with systemic symptoms. *Auditor Rule: An "exacerbation" must be clinically significant. A minor ache treated with over-the-counter medication is a minor problem, not a moderate exacerbation.*
    *   **High:** One or more chronic illnesses with severe exacerbation, progression, or side effects of treatment; one acute or chronic illness or injury that poses a threat to life or bodily function.
*   **2. Amount and/or Complexity of Data to be Reviewed and Analyzed**
    *   **Minimal/None:** No data, or minimal data reviewed (e.g., no external records, no tests ordered).
    *   **Limited (Low):** Must meet requirements in at least one category (e.g., review of prior external notes, or ordering tests).
    *   **Moderate:** Must meet requirements in at least one of three categories (e.g., review of prior external notes AND ordering multiple tests, independent historian, or independent interpretation).
    *   *Auditor Rule:* Do not assume data was reviewed unless explicitly stated in the note. 
*   **3. Risk of Complications and/or Morbidity or Mortality**
    *   **Minimal/Low:** Over-the-counter medications, minor surgery with no identified risk factors, physical therapy.
    *   **Moderate:** Prescription drug management (including initiating or continuing controlled substances), decision regarding minor surgery with identified risk factors.
    *   **High:** Drug therapy requiring intensive monitoring for toxicity, decision regarding emergency major surgery, decision regarding hospitalization.

## Workflow
Follow these sequential steps to conduct the audit:

1.  **Extract and Filter the Evidence:** Read the encounter notes carefully. Distinguish between active problems being managed today versus historical "noise" or resolved issues. Identify all data explicitly reviewed and the specific treatments prescribed.
2.  **Score Problem Complexity (Element 1):** Evaluate the true severity of the active conditions. Assign a level (Minimal, Low, Moderate, High). If a provider claims an "exacerbation" but the clinical text shows the issue is minor, stable, or self-resolving, override the provider's label and score appropriately based on the clinical reality.
3.  **Score Data Complexity (Element 2):** Count explicitly documented external records, tests, and independent historians. Score as Minimal/None if none are present.
4.  **Score Risk (Element 3):** Assess the risk of the management plan. Identify if prescription drug management elevates the risk to Moderate. 
5.  **Determine Overall MDM:** Apply the "two out of three" rule. Identify the highest MDM level where at least two elements meet the criteria. For example, if Problems Addressed is scored Low, Data is scored Minimal, and Risk is scored Moderate, the Overall MDM remains Low because two elements did not reach Moderate. This would support CPT 99213, not 99214.
6.  **Evaluate Billed E/M Code Compliance:** Compare your overall MDM level against the billed CPT code. State clearly if the code is supported or if a downcode is required.
7.  **Evaluate Add-on Codes (e.g., G2211):** Perform a strict assessment against Medicare's requirement for a "longitudinal relationship for a complex or serious condition." Reject the charge if the documentation only supports a routine check-in, medication refill, or management of minor/stable conditions.
8.  **Draft the Audit Report:** Assemble your findings directly into the required Markdown structure.

## Output format
Your output must be a formal Audit Findings Report formatted in Markdown. You must use the exact section headers below:

### 1. MDM Element Analysis
Provide an independent, element-by-element breakdown of your scoring. Use bolding for the element names.
*   **Number and Complexity of Problems Addressed:** State the level (e.g., Low, Moderate) and justify it using specific clinical facts, explicitly filtering out clinical noise.
*   **Amount and/or Complexity of Data to be Reviewed and Analyzed:** State the level and justify it.
*   **Risk of Complications and/or Morbidity or Mortality of Patient Management:** State the level and justify it (e.g., noting if prescription drug management applies).

### 2. Overall MDM Determination
State the final E/M MDM level supported by the documentation. Explicitly state how the "two out of three" rule was applied to reach this conclusion.

### 3. CPT [Insert Billed Code] Compliance Ruling
*Replace "[Insert Billed Code]" with the specific CPT code being audited (e.g., 99214).* Provide a definitive conclusion on whether the documentation supports the billed E/M visit level. If unsupported, provide the appropriate E/M code recommendation (e.g., "The documentation supports CPT 99213; downcoding from 99214 is recommended").

### 4. HCPCS [Insert Add-on Code] Evaluation
*Replace "[Insert Add-on Code]" with the specific HCPCS code being audited (e.g., G2211).* Provide a strict technical assessment of whether the documentation satisfies Medicare's specific requirements for this complex visit add-on code. Conclude firmly whether the charge is supported or unsupported.

## Constraints
*   **NEVER ASSUME UNSTATED FACTS:** If a test, past medical record, or complex coordination of care is not explicitly detailed in the narrative, you must score the Data element as Minimal/None.
*   **DO NOT OVERWEIGHT PRESCRIPTION MANAGEMENT:** While prescribing a controlled substance generally meets the criteria for Moderate Risk, you must NOT assign a Moderate overall MDM based on Risk alone. The "two out of three" rule is absolute.
*   **DO NOT RELY ON PROVIDER HEADERS FOR ADD-ON CODES:** The presence of a "Primary Care" header or a list of past medical history does not automatically justify the G2211 add-on. The specific active management in the encounter must reflect ongoing care for a complex or serious condition.
*   **MAINTAIN AUDITOR TONE:** Do not write a general complaint-style response. Write a highly technical, objective audit report. Do not offer medical advice or critique the provider's clinical skills; critique only the documentation's compliance with coding rules.

## Quality Checklist
Before finalizing your response, review your analysis against these criteria:
*   Did I objectively filter out clinical noise (like resolved issues or minor aches) when scoring Problem Complexity?
*   Did I strictly enforce the "two out of three" rule for the final MDM level?
*   Did I apply the strict Medicare definition for G2211, rather than assuming it applies to all primary care or chronic condition visits?
*   Are all conclusions strictly derived from the provided text, without inventing missing data or tests?