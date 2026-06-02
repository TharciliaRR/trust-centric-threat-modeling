# TCTM Canvas

## Trust-Centric Threat Modeling Framework

### Strategic Trust Assessment Canvas for Autonomous AI Systems

---

# Purpose

The TCTM Canvas provides a structured and visual approach for evaluating trust-related risks in autonomous AI systems.

The canvas enables organizations to rapidly identify:

* Trust Dependencies
* Trust Risks
* Threats
* Governance Gaps
* Control Requirements
* Trust Improvement Opportunities

The objective is to support executive discussions, workshops, architecture reviews, and AI governance assessments.

---

# TCTM Canvas Structure

```text
┌─────────────────────────────────────────────────────────┐
│                 SYSTEM OVERVIEW                         │
├─────────────────────────────────────────────────────────┤
│ BUSINESS OBJECTIVE                                      │
├─────────────┬─────────────┬─────────────┬──────────────┤
│ IDENTITY    │ CONTEXT     │ DECISION    │ GOVERNANCE   │
│ TRUST       │ TRUST       │ TRUST       │ TRUST        │
├─────────────┴─────────────┴─────────────┬──────────────┤
│ OPERATIONAL TRUST                       │              │
├─────────────────────────────────────────┴──────────────┤
│ THREATS                                                │
├────────────────────────────────────────────────────────┤
│ TRUST RISKS                                            │
├────────────────────────────────────────────────────────┤
│ TRUST CONTROLS                                         │
├────────────────────────────────────────────────────────┤
│ TRUST METRICS                                          │
├────────────────────────────────────────────────────────┤
│ TARGET MATURITY                                        │
└────────────────────────────────────────────────────────┘
```

---

# 1. System Overview

## Objective

Describe the autonomous AI system being assessed.

### Questions

* What is the system?
* What business problem does it solve?
* What level of autonomy does it possess?

### Example

Enterprise Financial Advisory Agent

Provides financial recommendations to executive leadership.

Autonomy Level: 3 (Conditional Autonomy)

---

# 2. Business Objective

## Objective

Identify the business outcome supported by the AI system.

### Questions

* What decisions are influenced?
* What business processes are affected?
* What is the expected value?

### Example

Support budget planning and investment prioritization.

---

# 3. Identity Trust

## Objective

Assess confidence in identities and access management.

### Evaluation Areas

* Authentication
* Authorization
* Agent Identity
* Privileged Access

### Key Questions

* Are agent identities authenticated?
* Is MFA implemented?
* Are authorization boundaries defined?

### Trust Score

```text
1 – 5
```

---

# 4. Context Trust

## Objective

Assess trust in information sources and contextual knowledge.

### Evaluation Areas

* Data Provenance
* Knowledge Sources
* Context Validation
* Source Reliability

### Key Questions

* Can context be trusted?
* Are sources verified?
* Is context poisoning monitored?

### Trust Score

```text
1 – 5
```

---

# 5. Decision Trust

## Objective

Assess confidence in recommendations and actions.

### Evaluation Areas

* Decision Integrity
* Explainability
* Human Validation
* Hallucination Resistance

### Key Questions

* Can recommendations be trusted?
* Are decisions explainable?
* Is decision quality validated?

### Trust Score

```text
1 – 5
```

---

# 6. Governance Trust

## Objective

Assess accountability and oversight.

### Evaluation Areas

* Accountability
* Auditability
* Governance Processes
* Compliance

### Key Questions

* Who owns the agent?
* Who is accountable?
* Are governance reviews performed?

### Trust Score

```text
1 – 5
```

---

# 7. Operational Trust

## Objective

Assess runtime trustworthiness and resilience.

### Evaluation Areas

* Monitoring
* Incident Response
* Runtime Protection
* Resilience

### Key Questions

* Is behavior observable?
* Are incidents managed effectively?
* Is trust monitored continuously?

### Trust Score

```text
1 – 5
```

---

# 8. Threats

## Objective

Identify trust-related threats.

### Categories

| Category | Description                |
| -------- | -------------------------- |
| TMT      | Trust Manipulation Threats |
| DIT      | Decision Integrity Threats |
| GFT      | Governance Failure Threats |
| OTT      | Operational Trust Threats  |

### Example Threats

* Prompt Injection
* Context Poisoning
* Hallucinated Recommendations
* Decision Drift
* Missing Accountability
* Agent Hijacking

---

# 9. Trust Risks

## Objective

Identify the most significant trust-related risks.

### Example

| Risk                                  | Severity  |
| ------------------------------------- | --------- |
| Hallucinated Executive Recommendation | Critical  |
| Context Poisoning                     | Very High |
| Governance Bypass                     | High      |

---

# 10. Trust Controls

## Objective

Identify mitigation actions.

### Examples

| Domain            | Control                    |
| ----------------- | -------------------------- |
| Identity Trust    | MFA                        |
| Context Trust     | Data Provenance Validation |
| Decision Trust    | Human-in-the-Loop          |
| Governance Trust  | Accountability Mapping     |
| Operational Trust | Runtime Monitoring         |

---

# 11. Trust Metrics

## Objective

Measure trustworthiness.

### Metrics

| Metric                  | Score |
| ----------------------- | ----- |
| Identity Trust Score    |       |
| Context Trust Score     |       |
| Decision Trust Score    |       |
| Governance Trust Score  |       |
| Operational Trust Score |       |

### Overall Trust Score

```text
____ / 5.0
```

---

# 12. Target Maturity

## Objective

Define the desired future state.

### Maturity Levels

| Level   | Description              |
| ------- | ------------------------ |
| Level 1 | Experimental             |
| Level 2 | Controlled               |
| Level 3 | Governed                 |
| Level 4 | Resilient                |
| Level 5 | Trust-Centric Enterprise |

### Current Level

```text
____
```

### Target Level

```text
____
```

---

# Executive Interpretation

The TCTM Canvas provides a one-page strategic view of trust within an autonomous AI system.

It is intended to support:

* Executive Reviews
* AI Governance Workshops
* Threat Modeling Sessions
* Risk Assessments
* Security Architecture Reviews
* AI Assurance Programs

---

# Strategic Principle

> Trust should be assessed with the same rigor that organizations apply to cybersecurity, governance, and risk management.

The TCTM Canvas provides a practical mechanism for making trust visible, measurable, and actionable.

