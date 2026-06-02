# Comparative Analysis

## Positioning the Trust-Centric Threat Modeling Framework (TCTM) Within Existing Cybersecurity, AI Security, and AI Governance Frameworks

---

# Abstract

The rapid adoption of autonomous AI systems has accelerated the development of frameworks focused on AI security, governance, risk management, and trustworthy AI.

Several frameworks provide valuable mechanisms for identifying threats, assessing risks, and establishing governance practices. However, these frameworks often focus on technical assets, models, infrastructure, or compliance requirements.

This comparative analysis evaluates the Trust-Centric Threat Modeling Framework (TCTM) alongside widely adopted frameworks including STRIDE, PASTA, MITRE ATLAS, OWASP LLM Top 10, NIST AI RMF, and ISO/IEC 42001.

The objective is to identify areas of overlap, complementary capabilities, and research gaps addressed by TCTM.

---

# Introduction

Organizations deploying autonomous AI systems face challenges that extend beyond traditional cybersecurity concerns.

These challenges include:

* Decision Integrity
* Trust Preservation
* Governance Effectiveness
* Accountability
* Autonomous Agent Oversight

Existing frameworks provide important foundations but vary significantly in scope and objectives.

This analysis compares TCTM against representative frameworks across cybersecurity, AI security, and AI governance domains.

---

# Evaluation Criteria

Frameworks are compared using the following dimensions.

| Dimension           | Description                             |
| ------------------- | --------------------------------------- |
| Threat Modeling     | Ability to identify threats             |
| AI Security         | Focus on AI-specific attacks            |
| Governance          | Oversight and accountability mechanisms |
| Risk Assessment     | Structured risk evaluation              |
| Trust Assessment    | Explicit trust evaluation               |
| Decision Integrity  | Protection of decision-making processes |
| Agent Governance    | Governance of autonomous agents         |
| Trust Metrics       | Measurement of trustworthiness          |
| Maturity Assessment | Capability maturity evaluation          |

---

# STRIDE

## Overview

STRIDE is a threat modeling methodology developed by Microsoft.

It classifies threats into six categories:

| Category               | Objective            |
| ---------------------- | -------------------- |
| Spoofing               | Identity Protection  |
| Tampering              | Integrity Protection |
| Repudiation            | Accountability       |
| Information Disclosure | Confidentiality      |
| Denial of Service      | Availability         |
| Elevation of Privilege | Authorization        |

---

## Strengths

* Well-established methodology
* Clear threat categorization
* Widely adopted
* Effective for software systems

---

## Limitations

* Limited AI-specific coverage
* No trust assessment
* No trust metrics
* No autonomous agent governance
* No decision integrity evaluation

---

## Relationship to TCTM

TCTM extends traditional threat modeling concepts by introducing trust-oriented assessment domains and trust-specific threats.

---

# PASTA

## Overview

Process for Attack Simulation and Threat Analysis (PASTA) is a risk-centric threat modeling methodology.

It emphasizes:

* Business impact
* Threat analysis
* Risk assessment

---

## Strengths

* Risk-oriented methodology
* Business alignment
* Structured process

---

## Limitations

* Limited trust assessment
* No autonomous AI focus
* No trust maturity evaluation

---

## Relationship to TCTM

TCTM shares PASTA's emphasis on risk but introduces trust as a distinct assessment dimension.

---

# MITRE ATLAS

## Overview

MITRE ATLAS focuses on adversarial threats against AI systems.

Key areas include:

* Model manipulation
* Data poisoning
* AI exploitation techniques

---

## Strengths

* AI-specific threat intelligence
* Adversary-centric approach
* Extensive attack knowledge base

---

## Limitations

* Limited governance perspective
* No trust measurement
* No maturity model
* Limited focus on decision integrity

---

## Relationship to TCTM

MITRE ATLAS can support TCTM threat identification activities, particularly within Trust Manipulation Threats and Decision Integrity Threats.

---

# OWASP LLM Top 10

## Overview

OWASP LLM Top 10 identifies common risks affecting LLM applications.

Examples include:

* Prompt Injection
* Training Data Poisoning
* Sensitive Information Disclosure
* Excessive Agency

---

## Strengths

* Practical guidance
* Focused on modern AI applications
* Widely recognized

---

## Limitations

* Focused primarily on vulnerabilities
* Limited governance coverage
* No trust measurement model
* No maturity assessment

---

## Relationship to TCTM

OWASP LLM threats can be incorporated into the TCTM Threat Taxonomy.

---

# NIST AI Risk Management Framework

## Overview

The NIST AI RMF provides guidance for managing AI-related risks.

Core functions include:

* Govern
* Map
* Measure
* Manage

---

## Strengths

* Comprehensive risk framework
* Governance-oriented
* Strong trustworthiness principles

---

## Limitations

* High-level guidance
* No operational trust metrics
* Limited threat modeling methodology
* No dedicated agent governance model

---

## Relationship to TCTM

TCTM may serve as an operational assessment methodology supporting implementation of NIST AI RMF objectives.

---

# ISO/IEC 42001

## Overview

ISO/IEC 42001 establishes requirements for AI Management Systems (AIMS).

The standard focuses on:

* Governance
* Oversight
* Risk Management
* Continuous Improvement

---

## Strengths

* International standard
* Governance structure
* Compliance-oriented approach

---

## Limitations

* Limited threat modeling guidance
* No trust metrics
* No trust maturity framework
* Limited operational assessment mechanisms

---

## Relationship to TCTM

TCTM can complement ISO 42001 by providing detailed trust assessment and trust risk evaluation capabilities.

---

# Comparative Framework Matrix

| Capability         | STRIDE  | PASTA   | MITRE ATLAS | OWASP LLM | NIST AI RMF | ISO 42001 | TCTM |
| ------------------ | ------- | ------- | ----------- | --------- | ----------- | --------- | ---- |
| Threat Modeling    | ✓       | ✓       | ✓           | Partial   | Partial     | No        | ✓    |
| AI Security        | No      | Partial | ✓           | ✓         | Partial     | Partial   | ✓    |
| Governance         | Partial | Partial | No          | No        | ✓           | ✓         | ✓    |
| Risk Assessment    | Partial | ✓       | Partial     | Partial   | ✓           | ✓         | ✓    |
| Trust Assessment   | No      | No      | No          | No        | Partial     | Partial   | ✓    |
| Decision Integrity | No      | No      | Partial     | Partial   | Partial     | Partial   | ✓    |
| Agent Governance   | No      | No      | No          | No        | Partial     | Partial   | ✓    |
| Trust Metrics      | No      | No      | No          | No        | No          | No        | ✓    |
| Maturity Model     | No      | No      | No          | No        | Partial     | Partial   | ✓    |

---

# TCTM Differentiators

The analysis identifies several capabilities that are either absent or only partially addressed in existing frameworks.

---

## Trust Domains

TCTM introduces five trust-oriented assessment domains:

* Identity Trust
* Context Trust
* Decision Trust
* Governance Trust
* Operational Trust

---

## Trust Impact

TCTM extends traditional risk calculations by introducing Trust Impact as a risk factor.

```text
Risk = Impact × Likelihood × Trust Impact
```

---

## Decision Security

TCTM treats decisions as assets requiring protection.

This perspective is not explicitly present in existing frameworks.

---

## Trust Observability

TCTM proposes mechanisms for monitoring trust degradation through trust signals, telemetry, and trust metrics.

---

## Agent Governance

TCTM introduces governance concepts specifically designed for autonomous AI agents.

---

## Trust Metrics

TCTM provides quantitative mechanisms for measuring trustworthiness.

---

## Trust Maturity Model

TCTM evaluates organizational trust capabilities through a structured maturity framework.

---

# Research Contribution Analysis

The comparative analysis suggests that TCTM occupies a distinct position at the intersection of:

* Cybersecurity
* AI Security
* AI Governance
* Trustworthy AI
* Digital Trust

Rather than replacing existing frameworks, TCTM complements them by focusing on trust as a measurable and governable capability.

---

# Discussion

Existing frameworks remain highly valuable and should continue to serve as foundational components of AI security and governance programs.

However, autonomous AI systems introduce challenges that extend beyond technical threats and compliance requirements.

Organizations increasingly require mechanisms for evaluating:

* Trust
* Confidence
* Decision Integrity
* Accountability
* Autonomous Governance

These areas represent the primary focus of TCTM.

---

# Conclusion

The comparison demonstrates that existing frameworks provide strong capabilities for threat identification, security management, governance, and compliance.

However, significant gaps remain in areas related to trust measurement, trust monitoring, decision integrity, and autonomous agent governance.

The Trust-Centric Threat Modeling Framework seeks to address these gaps by introducing a trust-oriented perspective for assessing autonomous AI systems.

---

# Research Proposition

> Existing frameworks help organizations secure AI systems. TCTM extends this perspective by helping organizations assess, govern, measure, and preserve trust in autonomous AI systems.

