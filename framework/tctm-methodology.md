# TCTM Assessment Methodology

## Trust-Centric Threat Modeling Framework

### Version 1.0

---

# Executive Summary

The Trust-Centric Threat Modeling Framework (TCTM) provides a structured methodology for evaluating trust-related risks in autonomous AI systems.

Unlike traditional cybersecurity assessments, TCTM expands the scope of analysis beyond infrastructure protection and includes:

* Trust
* Governance
* Decision Integrity
* Accountability
* Operational Resilience

The methodology enables organizations to identify trust-related threats, assess their impact, evaluate organizational maturity, and implement trust-preserving controls.

---

# Methodology Overview

The TCTM assessment process consists of seven phases.

![Flow Across Trust Domains.](https://github.com/TharciliaRR/trust-centric-threat-modeling/blob/main/diagrams/Diagram%20F17.1.png)  

---

# Phase 1 — Define Scope

## Objective

Establish assessment boundaries.

---

## Key Questions

* What system is being evaluated?
* What business function does it support?
* What level of autonomy exists?
* What decisions are influenced?
* What stakeholders are impacted?

---

## Required Outputs

* System Description
* Business Context
* Assessment Scope
* Criticality Classification

---

# Phase 2 — Map Trust Domains

## Objective

Evaluate trust across the five TCTM domains.

---

## Trust Domains

| Domain            | Focus                               |
| ----------------- | ----------------------------------- |
| Identity Trust    | Authentication and authorization    |
| Context Trust     | Information quality and integrity   |
| Decision Trust    | Recommendation and decision quality |
| Governance Trust  | Accountability and oversight        |
| Operational Trust | Runtime behavior and resilience     |

---

## Assessment Approach

Each domain receives a score between:

| Score | Description |
| ----- | ----------- |
| 1     | Very Weak   |
| 2     | Weak        |
| 3     | Moderate    |
| 4     | Strong      |
| 5     | Very Strong |

---

## Output

Trust Domain Profile

Example:

| Domain            | Score |
| ----------------- | ----- |
| Identity Trust    | 4.2   |
| Context Trust     | 3.1   |
| Decision Trust    | 2.8   |
| Governance Trust  | 3.4   |
| Operational Trust | 4.0   |

---

# Phase 3 — Threat Identification

## Objective

Identify threats affecting trustworthiness.

---

## Threat Taxonomy

### TMT

Trust Manipulation Threats

Examples:

* Prompt Injection
* Context Poisoning
* Confidence Manipulation

---

### DIT

Decision Integrity Threats

Examples:

* Hallucinated Actions
* Decision Drift
* Misalignment

---

### GFT

Governance Failure Threats

Examples:

* Missing Accountability
* Governance Bypass
* Audit Deficiencies

---

### OTT

Operational Trust Threats

Examples:

* Agent Hijacking
* Runtime Manipulation
* Resilience Failures

---

## Output

Threat Register

---

# Phase 4 — Trust Risk Assessment

## Objective

Evaluate trust-related risks.

---

## Risk Formula

```text
Risk Score = Impact × Likelihood × Trust Impact
```

---

## Impact Scale

| Score | Description |
| ----- | ----------- |
| 1     | Negligible  |
| 2     | Minor       |
| 3     | Moderate    |
| 4     | Significant |
| 5     | Severe      |

---

## Likelihood Scale

| Score | Description    |
| ----- | -------------- |
| 1     | Rare           |
| 2     | Unlikely       |
| 3     | Possible       |
| 4     | Likely         |
| 5     | Almost Certain |

---

## Trust Impact Scale

| Score | Description                 |
| ----- | --------------------------- |
| 1     | Minimal Trust Impact        |
| 2     | Limited Trust Reduction     |
| 3     | Noticeable Trust Impact     |
| 4     | Significant Trust Erosion   |
| 5     | Critical Loss of Confidence |

---

## Risk Classification

| Score  | Category  |
| ------ | --------- |
| 1–20   | Low       |
| 21–40  | Moderate  |
| 41–60  | High      |
| 61–80  | Very High |
| 81–125 | Critical  |

---

## Output

Trust Risk Register

---

# Phase 5 — Trust Maturity Assessment

## Objective

Evaluate organizational capability.

---

## Assessment Areas

* Governance
* Monitoring
* Accountability
* Trust Metrics

---

## Maturity Levels

| Level   | Description              |
| ------- | ------------------------ |
| Level 1 | Experimental             |
| Level 2 | Controlled               |
| Level 3 | Governed                 |
| Level 4 | Resilient                |
| Level 5 | Trust-Centric Enterprise |

---

## Output

Trust Maturity Score

---

# Phase 6 — Trust Control Selection

## Objective

Define mitigation strategies.

---

## Control Categories

### Identity Trust Controls

Examples:

* MFA
* PAM
* Agent Authentication

---

### Context Trust Controls

Examples:

* Data Provenance Validation
* Context Integrity Monitoring
* Source Verification

---

### Decision Trust Controls

Examples:

* Human-in-the-Loop Approval
* Explainability Requirements
* Decision Validation

---

### Governance Trust Controls

Examples:

* Accountability Mapping
* Audit Trails
* Governance Reviews

---

### Operational Trust Controls

Examples:

* Runtime Monitoring
* Trust Dashboards
* Incident Response

---

## Output

Trust Improvement Plan

---

# Phase 7 — Continuous Monitoring

## Objective

Maintain trust over time.

---

## Trust Monitoring Areas

### Trust Metrics

Measure:

* Trust Scores
* Decision Integrity
* Governance Effectiveness

---

### Trust Observability

Monitor:

* Trust Degradation
* Confidence Trends
* Decision Drift

---

### Trust Assurance

Validate:

* Controls
* Governance
* Operational Effectiveness

---

## Output

Continuous Trust Monitoring Program

---

# Methodology Deliverables

A completed TCTM assessment should produce:

| Deliverable            | Description              |
| ---------------------- | ------------------------ |
| Trust Domain Profile   | Trust assessment results |
| Threat Register        | Identified threats       |
| Trust Risk Register    | Risk assessment          |
| Maturity Assessment    | Capability evaluation    |
| Trust Improvement Plan | Recommended controls     |
| Executive Report       | Strategic findings       |

---

# Assessment Roles

## Executive Sponsor

Provides strategic oversight.

---

## Assessor

Conducts the evaluation.

---

## System Owner

Provides system knowledge.

---

## Governance Lead

Evaluates governance effectiveness.

---

## Security Lead

Evaluates security posture.

---

# Success Criteria

A successful TCTM assessment should:

* Identify trust-related risks
* Quantify trust impact
* Evaluate governance effectiveness
* Assess decision integrity
* Define mitigation controls
* Establish trust monitoring mechanisms

---

# Strategic Observation

Traditional threat modeling evaluates risks to systems.

TCTM evaluates risks to trust.

As organizations increasingly deploy autonomous AI systems, trust becomes a critical organizational asset that must be measured, governed, protected, and continuously monitored.

---

# Methodology Principle

> Trust should be treated as a measurable, governable, and protectable organizational capability.

The TCTM methodology provides a structured process for achieving that objective.  

![Flow Across Trust Domains.](https://github.com/TharciliaRR/trust-centric-threat-modeling/blob/main/diagrams/Diagram%20F17.2.png)  

