# AI Use Case Framing Framework

This framework is used to evaluate whether an AI-powered feature is worth building, how it should be designed, and how it should be safely deployed.

It is intended for early-stage AI product discovery and strategic evaluation.

---

## 1. Problem Fit

Before discussing models, define the problem clearly:

- What specific user pain are we solving?
- What measurable business impact does solving this create?
- What happens if the system makes a wrong prediction?
- Is the decision reversible?

AI should only be introduced if it meaningfully improves outcomes.

---

## 2. AI Suitability Assessment

Not every problem requires AI.

Ask:

- Can rules or heuristics solve 80% of the problem?
- Is the input unstructured (text, image, speech)?
- Does the problem require pattern recognition at scale?
- Is personalization or probabilistic reasoning needed?

If deterministic logic is sufficient, AI may introduce unnecessary complexity.

---

## 3. Data Readiness

AI performance is constrained by data quality.

Evaluate:

- Do we have sufficient historical data?
- Is the data representative of the user base?
- Are there data biases?
- What PII or privacy concerns exist?
- How often does data update?

Without strong data foundations, AI reliability will suffer.

---

## 4. Success Metrics

Define success at two levels.

### Model-Level Metrics
- Accuracy / Precision / Recall
- Human evaluation scores
- Hallucination rate (for generative systems)

### Product-Level Metrics
- Task success rate
- Time saved
- Conversion / retention lift
- Deflection rate (support use cases)

### Guardrails
- Bias thresholds
- Error tolerance
- Cost per inference
- Latency constraints

---

## 5. UX & Trust Design

AI systems require thoughtful UX design.

- Is the output explainable?
- Can users override or correct the system?
- Is uncertainty communicated?
- What is the fallback when confidence is low?

Trust is often more important than raw accuracy.

---

## 6. Risk & Safety Evaluation

Assess:

- Bias amplification
- Hallucination risk
- Prompt injection (for LLM-based systems)
- Security vulnerabilities
- Regulatory implications

Mitigation strategies must be defined before launch.

---

## 7. Rollout & Iteration Plan

AI products should not launch fully exposed.

Define:

- MVP scope
- Internal beta testing
- Limited external rollout
- Monitoring dashboards
- Feedback loops
- Iteration cadence

Continuous learning and monitoring are required post-launch.

---

## Core Principle

AI should enhance decision-making, not obscure it.

The goal is measurable user value with controlled risk, not model sophistication.
