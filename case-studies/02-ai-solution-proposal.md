# Case Study 2 — AI Job Fit Analyzer

## Context

Domain: Career marketplace  
Users: Job seekers and employers  
Business Goal: Improve job application match quality and increase employer satisfaction  

Users often applied to roles that were poorly matched to their profile, leading to low response rates and employer dissatisfaction.

---

## Problem Statement

Low match quality resulted in:
- Reduced employer trust
- Poor candidate experience
- Increased platform churn

We needed a scalable way to assess job-candidate fit beyond keyword matching.

---

## Why AI?

Rule-based filtering (skills overlap) failed to capture:
- Contextual experience
- Transferable skills
- Seniority alignment
- Implicit qualifications

Natural language understanding was required.

---

## Proposed Solution

Input:
- Candidate resume
- Job description

AI Layer:
- LLM-based semantic comparison
- Embedding similarity scoring
- Structured fit explanation generation

Output:
- Fit score (0–100)
- Key match strengths
- Missing qualification signals

Human Oversight:
- Employer feedback loop to refine scoring

---

## Model Options Considered

### Option A — Classic ML Classifier
Pros:
- More predictable
- Easier evaluation

Cons:
- Requires labeled training data
- Limited flexibility

---

### Option B — LLM Prompt-Based Scoring
Pros:
- Rapid deployment
- Handles unstructured text well

Cons:
- Hallucination risk
- Requires guardrails

---

### Option C — RAG + LLM Hybrid
Pros:
- More grounded outputs
- Better explainability

Cons:
- Higher infrastructure complexity

---

## Data Requirements

- Resume text corpus
- Job description corpus
- Historical hiring outcomes (if available)
- Feedback loop signals

Privacy:
- PII handling
- Secure storage
- Data anonymization policies

---

## Evaluation Metrics

Model Metrics:
- Precision / Recall (if labeled data available)
- Human evaluator agreement rate

Product Metrics:
- Employer response rate
- Interview conversion rate
- Candidate application success rate

Guardrails:
- Bias detection (gendered language impact)
- False negative rate for qualified candidates

---

## MVP Scope

Included:
- Resume + JD semantic similarity
- Basic explanation output

Excluded:
- Cultural fit scoring
- Predictive salary estimation
- Automated rejection decisions

---

## Iteration Plan

- Collect employer feedback on match quality
- Fine-tune prompts based on disagreement cases
- Introduce ranking calibration
- Add bias monitoring dashboard

---

## Key Takeaway

AI should assist decision-making, not replace it.

Transparent scoring and explainability are critical for trust in hiring workflows.
