# Trust Risk Matrix

## Overview

Traditional cybersecurity risk assessment models typically evaluate risk using two dimensions:

* Impact
* Likelihood

These dimensions are highly effective for evaluating conventional threats such as:

* Data breaches
* Malware infections
* Unauthorized access
* Denial of Service attacks

However, autonomous AI systems introduce a new challenge.

An incident may have limited operational consequences while causing significant degradation of organizational trust.

For example:

| Incident                              | Operational Impact | Trust Impact |
| ------------------------------------- | ------------------ | ------------ |
| Temporary API Failure                 | Moderate           | Low          |
| Hallucinated Executive Recommendation | Moderate           | Critical     |

In both cases, the operational impact may be similar.

The trust consequences are dramatically different.

To address this gap, the Trust-Centric Threat Modeling Framework (TCTM) introduces Trust Impact as an independent risk dimension.



# Traditional Risk Models

Most risk frameworks evaluate risk using:

```text
Risk = Impact × Likelihood
```

While effective for traditional cybersecurity assessments, this approach does not adequately capture the trust implications of autonomous decision-making.


# TCTM Risk Model

The Trust Risk Matrix extends traditional risk calculations.

```text
Risk = Impact × Likelihood × Trust Impact
```

Where:

* Impact = Operational consequence
* Likelihood = Probability of occurrence
* Trust Impact = Degree of trust degradation

This additional dimension enables organizations to evaluate not only technical and operational consequences, but also the effect of incidents on stakeholder confidence and decision reliability.



# Risk Dimensions

## Impact

Measures the operational, financial, legal, or business consequences of an incident.

### Impact Scale

| Score | Description |
| ----- | ----------- |
| 1     | Negligible  |
| 2     | Minor       |
| 3     | Moderate    |
| 4     | Significant |
| 5     | Severe      |



## Likelihood

Measures the probability that a threat will occur.

### Likelihood Scale

| Score | Description    |
| ----- | -------------- |
| 1     | Rare           |
| 2     | Unlikely       |
| 3     | Possible       |
| 4     | Likely         |
| 5     | Almost Certain |



## Trust Impact

Measures the effect of an incident on stakeholder confidence and organizational trust.

### Trust Impact Scale

| Score | Description                  |
| ----- | ---------------------------- |
| 1     | Minimal Trust Degradation    |
| 2     | Limited Confidence Reduction |
| 3     | Noticeable Trust Impact      |
| 4     | Significant Trust Erosion    |
| 5     | Critical Loss of Confidence  |


# Trust Impact Assessment Criteria

Trust Impact should be evaluated using multiple dimensions.

Organizations should consider:

## Decision Reliability

Can stakeholders continue relying on system outputs?



## Governance Confidence

Can leadership continue trusting governance mechanisms?


## Regulatory Confidence

Would regulators question organizational oversight?



## Stakeholder Confidence

Would users lose confidence in the system?


## Organizational Reputation

Could the incident affect public perception?



# Risk Calculation Example

## Threat

Prompt Injection

### Assessment

| Factor       | Score |
| ------------ | ----- |
| Impact       | 5     |
| Likelihood   | 4     |
| Trust Impact | 5     |

### Risk Score

```text
Risk = 5 × 4 × 5

Risk = 100
```

### Classification

Critical



# Risk Classification

After calculating the score, risks are categorized according to the following scale.

| Score Range | Category  |
| ----------- | --------- |
| 1–20        | Low       |
| 21–40       | Moderate  |
| 41–60       | High      |
| 61–80       | Very High |
| 81–125      | Critical  |



# Trust Risk Matrix

The Trust Risk Matrix enables rapid visualization of trust-related risk levels.

| Trust Impact ↓ / Likelihood → | 1 | 2 | 3  | 4  | 5  |
| ----------------------------- | - | - | -- | -- | -- |
| **5**                         | M | H | VH | C  | C  |
| **4**                         | M | M | H  | VH | C  |
| **3**                         | L | M | H  | H  | VH |
| **2**                         | L | L | M  | H  | H  |
| **1**                         | L | L | M  | M  | H  |

### Legend

| Code | Risk Level |
| ---- | ---------- |
| L    | Low        |
| M    | Moderate   |
| H    | High       |
| VH   | Very High  |
| C    | Critical   |



# Mapping Risks to Trust Domains

The Trust Risk Matrix is designed to support all Trust Domains.

| Trust Domain      | Example Threat         |
| ----------------- | ---------------------- |
| Identity Trust    | Privilege Escalation   |
| Context Trust     | Context Poisoning      |
| Decision Trust    | Hallucinated Actions   |
| Governance Trust  | Missing Accountability |
| Operational Trust | Agent Hijacking        |

This mapping enables organizations to identify which dimensions of trust require additional controls.



# Trust Risk Dashboard

Organizations may aggregate scores into a Trust Risk Dashboard.

## Example

| Metric                 | Current Score |
| ---------------------- | ------------- |
| Identity Trust Risk    | 18            |
| Context Trust Risk     | 47            |
| Decision Trust Risk    | 62            |
| Governance Trust Risk  | 31            |
| Operational Trust Risk | 42            |

This approach transforms trust into a measurable and governable risk indicator.


# Why the Trust Risk Matrix Matters

Traditional cybersecurity frameworks focus on protecting systems.

Autonomous AI systems require organizations to protect confidence in decisions.

The Trust Risk Matrix enables organizations to:

* Prioritize trust-related risks
* Quantify trust degradation
* Improve governance decisions
* Support regulatory compliance
* Measure confidence in autonomous systems

Trust becomes a measurable organizational asset rather than a subjective perception.


# Key Takeaway

The Trust Risk Matrix extends traditional cybersecurity risk assessment by introducing Trust Impact as a third dimension of risk. This approach enables organizations to evaluate not only operational consequences, but also the effect of incidents on confidence, governance, and decision integrity. As autonomous systems become increasingly influential, measuring trust becomes as important as measuring security.

