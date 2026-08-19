# Validation Brief

**Scenario:** Scenario 1-Retention Engine

## 1 · Hypothesis
I'm testing whether Helping customers approve their first merchant within 14 days will improve 90-day retention.

## 2 · Risk type & kill switch
- **Risk type:** Feasibility
- **Build to test it:** Functional app
- **Kill switch:** Stop if fewer than 70% of eligible treatment accounts can complete the applicable rescue actions before day 14. The intervention would not be operationally feasible enough to test at scale.

## 3 · Success criteria
Pass only if, after every enrolled account has reached day 90:

At least 70% of eligible treatment accounts receive the intervention by day 14.
Median time to first merchant approval is 14 days or less.
The treatment cohort improves first-merchant approval by at least 8 percentage points versus control.
Observed 90-day retention improves by at least 5 percentage points versus control.
Statistical confidence reaches at least 95%.
No compliance, fraud, or operational guardrail materially worsens.

Otherwise, fail or redesign the intervention before rollout.

## 4 · Problem Framework
1. **Goal**, Reduce 90-day customer churn from approximately 30% to 25% or less by accelerating the first meaningful customer outcome.
2. **Problem**, The prototype identifies “no successful merchant approval by day 14” as the strongest churn signal. These accounts show a 31.4-point increase in churn and represent 38% of the new-account cohort.
3. **Context**, New payments-compliance customers can stall because of incomplete KYB, failed API integrations, slow merchant reviews, missing evidence, or limited team adoption. The treatment combines guided approval workshops, same-day reviews, pre-filled risk profiles, provisional approval paths, integration support, and sponsor escalation.
4. **Constraints**, Retention takes 90 days to observe; randomization must occur at the account level; compliance controls cannot be weakened; the intervention requires customer-success and engineering capacity; segment differences may affect results; and the current prototype uses fictional, modelled data rather than production evidence.
5. **Success**, Customers reach their first approved merchant within 14 days, the process is operationally deliverable, and treatment produces at least a 5-point statistically significant improvement in observed 90-day retention without harming compliance or unit economics.
6. **Explore**, Test which intervention components create the most lift, whether day 14 is the true causal threshold, which customer segments respond best, and whether a lower-touch version can preserve the benefit at a sustainable cost.

---
_Module 2 · Vibe Coding Certification · frame before you build._
