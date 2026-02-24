# Case Study 1 — Data-Driven Product Decision

## Context

Product: B2B SaaS analytics platform  
Users: Mid-size operations teams  
Business Goal: Improve activation rate and reduce early churn  

The product team observed that a large percentage of new users signed up but did not complete onboarding within the first 7 days.

---

## Problem Statement

Only 38% of users completed onboarding, and those who did not complete onboarding had a 2.4x higher churn rate within the first month.

The decision:  
Should we simplify onboarding or add AI-driven guidance to help users configure the product?

---

## Data Available

- Funnel analytics (Signup → Setup → First Value Action)
- Session recordings
- Customer support tickets
- Drop-off heatmaps
- User interviews (n=12)
- Time-to-first-value metrics

Constraints:
- Limited engineering bandwidth (1 sprint available)
- No ML pipeline in place

---

## Hypotheses

H1: Reducing onboarding steps from 6 to 3 will increase completion rate.

H2: Introducing AI-generated setup recommendations will reduce friction and improve activation.

---

## Metrics

Primary Metric:
- Onboarding completion rate

Secondary Metrics:
- Time to first value
- 30-day retention
- Support ticket volume

Guardrails:
- Setup error rate
- Misconfiguration incidents

---

## Options Considered

### Option A — Simplify Onboarding Flow

Pros:
- Fast to implement
- Low technical risk
- Immediate UX improvement

Cons:
- May reduce configurability
- Does not personalize experience

Risks:
- Oversimplification harms advanced users

---

### Option B — AI-Guided Setup Assistant

Pros:
- Personalized onboarding
- Scalable long-term solution
- Improves perceived product intelligence

Cons:
- Requires model evaluation
- More engineering complexity
- Risk of incorrect recommendations

Risks:
- Poor recommendations reduce trust

---

## Recommendation

Ship Option A first (simplified onboarding) as an MVP improvement.

In parallel, scope Option B as a Phase 2 AI enhancement once baseline friction is reduced and instrumentation is improved.

This minimizes risk while validating whether friction reduction alone improves activation.

---

## Execution Plan

Phase 1 (2 weeks):
- Reduce onboarding steps
- Improve inline guidance
- Add instrumentation to track friction points

Phase 2:
- Introduce AI-generated configuration suggestions
- A/B test assistant vs non-assistant flow

---

## Risks & Mitigations

Risk: Data insufficient to train meaningful assistant  
Mitigation: Use rule-based heuristics initially before ML integration  

Risk: AI recommendations are incorrect  
Mitigation: Display confidence levels and allow user override  

---

## Learnings

Data-driven prioritization reduces solution bias.

The simplest improvement often delivers the highest ROI before adding AI complexity.

AI should enhance a stable baseline, not compensate for broken UX.
