# Complete TCTM Assessment Example

## Enterprise Financial Advisory Agent

### Trust-Centric Threat Modeling Framework (TCTM)

---

# Executive Summary

This assessment demonstrates the practical application of the Trust-Centric Threat Modeling Framework (TCTM).

The evaluated system is an autonomous AI agent responsible for generating financial recommendations for executive leadership.

The objective of this assessment is to identify trust-related risks, evaluate organizational trust maturity, and define controls that improve trustworthiness.

---

# Phase 1 — Define Scope

## System Name

Enterprise Financial Advisory Agent (EFAA)

---

## Business Objective

Provide financial recommendations to executives regarding:

* Budget allocation
* Cost optimization
* Investment prioritization
* Financial forecasting

---

## Criticality

Critical

Incorrect recommendations may impact:

* Revenue
* Strategic decisions
* Investor confidence
* Regulatory compliance

---

## Stakeholders

| Stakeholder        | Responsibility           |
| ------------------ | ------------------------ |
| CFO                | Executive decision maker |
| Finance Team       | Financial analysis       |
| AI Governance Team | Oversight                |
| Security Team      | Security monitoring      |
| Internal Audit     | Compliance validation    |

---

## Autonomy Level

Level 3 — Conditional Autonomy

The agent may generate recommendations independently but requires executive approval before execution.

---

# Phase 2 — Trust Domain Assessment

## Identity Trust

### Assessment

* MFA enabled
* PAM implemented
* Agent authentication configured

### Score

| Metric                   | Score |
| ------------------------ | ----- |
| Identity Verification    | 5     |
| MFA Coverage             | 4     |
| Authorization Compliance | 4     |
| Agent Authentication     | 5     |

Identity Trust Score:

```text
4.5
```

---

## Context Trust

### Assessment

The system relies on:

* ERP data
* Financial reports
* External market data

Context validation is partially implemented.

### Score

| Metric             | Score |
| ------------------ | ----- |
| Data Provenance    | 3     |
| Context Integrity  | 3     |
| Source Reliability | 4     |
| Context Validation | 3     |

Context Trust Score:

```text
3.25
```

---

## Decision Trust

### Assessment

The system provides recommendations but lacks comprehensive decision validation.

### Score

| Metric                | Score |
| --------------------- | ----- |
| Decision Integrity    | 3     |
| Explainability        | 2     |
| Hallucination Control | 2     |
| Human Validation      | 3     |

Decision Trust Score:

```text
2.5
```

---

## Governance Trust

### Assessment

Governance processes exist but are not fully formalized.

### Score

| Metric                  | Score |
| ----------------------- | ----- |
| Accountability Coverage | 3     |
| Audit Coverage          | 4     |
| Governance Compliance   | 3     |
| Oversight Effectiveness | 3     |

Governance Trust Score:

```text
3.25
```

---

## Operational Trust

### Assessment

Monitoring and resilience controls are implemented.

### Score

| Metric              | Score |
| ------------------- | ----- |
| Runtime Stability   | 4     |
| Incident Response   | 4     |
| Resilience          | 4     |
| Monitoring Coverage | 4     |

Operational Trust Score:

```text
4.0
```

---

# Phase 3 — Trust Profile

## Current Trust Scores

| Domain            | Score |
| ----------------- | ----- |
| Identity Trust    | 4.5   |
| Context Trust     | 3.25  |
| Decision Trust    | 2.5   |
| Governance Trust  | 3.25  |
| Operational Trust | 4.0   |

---

## Overall Trust Score

Formula:

```text
(4.5 + 3.25 + 2.5 + 3.25 + 4.0) / 5
```

Result:

```text
3.5
```

Trust Rating:

```text
Moderate
```

---

# Phase 4 — Threat Identification

## Threat Register

| Threat ID | Category | Threat                       |
| --------- | -------- | ---------------------------- |
| TMT-01    | TMT      | Context Poisoning            |
| DIT-01    | DIT      | Hallucinated Recommendations |
| DIT-02    | DIT      | Decision Drift               |
| GFT-01    | GFT      | Missing Accountability       |
| OTT-01    | OTT      | Agent Hijacking              |

---

# Phase 5 — Trust Risk Assessment

## Risk Formula

```text
Risk Score = Impact × Likelihood × Trust Impact
```

---

### Threat 1 — Hallucinated Executive Recommendation

| Factor       | Score |
| ------------ | ----- |
| Impact       | 5     |
| Likelihood   | 4     |
| Trust Impact | 5     |

Risk Score:

```text
100
```

Classification:

```text
Critical
```

---

### Threat 2 — Context Poisoning

| Factor       | Score |
| ------------ | ----- |
| Impact       | 4     |
| Likelihood   | 4     |
| Trust Impact | 5     |

Risk Score:

```text
80
```

Classification:

```text
Very High
```

---

### Threat 3 — Missing Accountability

| Factor       | Score |
| ------------ | ----- |
| Impact       | 4     |
| Likelihood   | 3     |
| Trust Impact | 5     |

Risk Score:

```text
60
```

Classification:

```text
High
```

---

# Phase 6 — Maturity Assessment

## Capability Evaluation

| Capability     | Status     |
| -------------- | ---------- |
| Governance     | Formalized |
| Monitoring     | Structured |
| Accountability | Partial    |
| Trust Metrics  | Emerging   |

---

## Maturity Level

```text
Level 3 — Governed
```

---

# Phase 7 — Trust Control Selection

## Recommended Controls

| Domain            | Control                      | Priority |
| ----------------- | ---------------------------- | -------- |
| Decision Trust    | Decision Validation          | P1       |
| Decision Trust    | Explainability Requirements  | P1       |
| Context Trust     | Context Integrity Monitoring | P1       |
| Governance Trust  | Accountability Mapping       | P2       |
| Governance Trust  | Governance Reviews           | P2       |
| Operational Trust | Trust Dashboard              | P3       |

---

# Phase 8 — Post-Mitigation Projection

## Expected Future Scores

| Domain            | Before | After |
| ----------------- | ------ | ----- |
| Identity Trust    | 4.5    | 4.5   |
| Context Trust     | 3.25   | 4.1   |
| Decision Trust    | 2.5    | 4.0   |
| Governance Trust  | 3.25   | 4.3   |
| Operational Trust | 4.0    | 4.4   |

---

## Projected Overall Trust Score

```text
4.26
```

Trust Rating:

```text
Strong
```

---

# Assessment Conclusion

The assessment identified Decision Trust as the most critical weakness within the evaluated system.

Although the organization demonstrates strong Identity Trust and Operational Trust capabilities, deficiencies in decision validation and governance create significant trust-related risks.

The implementation of trust-focused controls is expected to improve the overall Trust Score from 3.5 to 4.26 and increase organizational trust maturity.

---

# Key Findings

### Strengths

* Strong authentication
* Mature operational monitoring
* Stable runtime environment

### Weaknesses

* Low decision explainability
* Hallucination exposure
* Partial accountability structures

### Highest Risk

Hallucinated Executive Recommendations

### Current Trust Rating

Moderate

### Target Trust Rating

Strong

### Current Maturity

Level 3 — Governed

### Target Maturity

Level 4 — Resilient

