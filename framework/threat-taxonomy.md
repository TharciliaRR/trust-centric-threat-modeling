# TCTM Threat Taxonomy

## Overview

Traditional threat modeling frameworks such as STRIDE, MITRE ATLAS, and the OWASP Top 10 for LLM Applications provide valuable approaches for identifying security threats in software and AI systems.

However, these frameworks primarily focus on technical compromise, adversarial attacks, and system security.

Autonomous AI systems introduce a broader challenge.

Organizations must not only protect systems from compromise but also preserve trust in:

* identities;
* information sources;
* decisions;
* governance mechanisms;
* operational behavior.

To address this challenge, the Trust-Centric Threat Modeling Framework (TCTM) introduces a trust-oriented threat taxonomy.

The taxonomy categorizes threats based on their impact on organizational trust.

---

# Taxonomy Structure

```text
TCTM Threat Taxonomy

├── TMT - Trust Manipulation Threats
├── DIT - Decision Integrity Threats
├── GFT - Governance Failure Threats
└── OTT - Operational Trust Threats
```

Each category represents a distinct class of threats capable of degrading trust in autonomous AI systems.

---

# TMT – Trust Manipulation Threats

## Definition

Trust Manipulation Threats target the information, context, and interactions used by autonomous agents.

The objective of these attacks is to influence system behavior by manipulating trusted inputs.

---

## Security Objective

Preserve Context Trust.

---

## Core Question

> Can the system trust the information it receives?

---

## TMT-01 Prompt Injection

### Description

Malicious instructions embedded in prompts, documents, emails, or retrieved content designed to influence model behavior.

### Example

An attacker embeds hidden instructions within a document processed by an AI assistant.

### Affected Trust Domains

* Context Trust
* Decision Trust

---

## TMT-02 Context Poisoning

### Description

Manipulation of retrieved information used by RAG systems or knowledge repositories.

### Example

Corrupted policies inserted into an internal knowledge base.

### Affected Trust Domains

* Context Trust
* Governance Trust

---

## TMT-03 Knowledge Base Tampering

### Description

Unauthorized modification of organizational knowledge sources.

### Example

Altering compliance documentation used by AI agents.

### Affected Trust Domains

* Context Trust

---

## TMT-04 Confidence Manipulation

### Description

Attempts to artificially increase confidence in unreliable outputs.

### Example

An attacker causes the model to present uncertain recommendations as highly reliable.

### Affected Trust Domains

* Decision Trust

---

# DIT – Decision Integrity Threats

## Definition

Decision Integrity Threats affect the reliability, consistency, and alignment of autonomous decisions.

These threats do not necessarily compromise infrastructure but compromise trust in outcomes.

---

## Security Objective

Preserve Decision Trust.

---

## Core Question

> Can stakeholders trust the decisions produced by the system?

---

## DIT-01 Hallucinated Actions

### Description

Actions or recommendations based on fabricated information.

### Example

A financial agent generates investment advice using nonexistent market data.

### Affected Trust Domains

* Decision Trust

---

## DIT-02 Decision Drift

### Description

Progressive deviation from intended objectives or organizational policies.

### Example

An AI assistant gradually favors actions inconsistent with business goals.

### Affected Trust Domains

* Decision Trust
* Operational Trust

---

## DIT-03 Misalignment

### Description

Decisions conflict with organizational strategy, ethics, or compliance requirements.

### Example

Cost-saving recommendations that violate regulatory obligations.

### Affected Trust Domains

* Decision Trust
* Governance Trust

---

## DIT-04 Unjustified Confidence

### Description

High-confidence recommendations generated without sufficient evidence.

### Example

An executive recommendation produced without supporting data.

### Affected Trust Domains

* Decision Trust

---

# GFT – Governance Failure Threats

## Definition

Governance Failure Threats undermine accountability, oversight, transparency, and compliance.

These threats reduce organizational ability to explain and govern autonomous systems.

---

## Security Objective

Preserve Governance Trust.

---

## Core Question

> Can the organization effectively govern and audit autonomous decisions?

---

## GFT-01 Missing Accountability

### Description

Inability to identify ownership of autonomous decisions.

### Example

No individual or team is responsible for AI-generated actions.

### Affected Trust Domains

* Governance Trust

---

## GFT-02 Lack of Auditability

### Description

Decisions cannot be reconstructed or explained.

### Example

Missing logs and reasoning traces.

### Affected Trust Domains

* Governance Trust

---

## GFT-03 Governance Bypass

### Description

Circumvention of organizational governance controls.

### Example

Agents execute actions without required approvals.

### Affected Trust Domains

* Governance Trust
* Operational Trust

---

## GFT-04 Regulatory Non-Compliance

### Description

Autonomous behavior violates legal or regulatory requirements.

### Example

Improper processing of personal information.

### Affected Trust Domains

* Governance Trust

---

# OTT – Operational Trust Threats

## Definition

Operational Trust Threats target the reliability, resilience, and operational behavior of autonomous systems.

These threats may disrupt confidence in ongoing operations.

---

## Security Objective

Preserve Operational Trust.

---

## Core Question

> Can the system operate reliably and securely over time?

---

## OTT-01 Agent Hijacking

### Description

Unauthorized manipulation of agent behavior.

### Example

An attacker gains control of autonomous workflows.

### Affected Trust Domains

* Operational Trust

---

## OTT-02 Autonomous Cascade Failure

### Description

Failures propagate across interconnected agents.

### Example

One compromised planning agent impacts multiple downstream systems.

### Affected Trust Domains

* Operational Trust
* Decision Trust

---

## OTT-03 Runtime Manipulation

### Description

Modification of agent behavior during execution.

### Example

Malicious alteration of runtime parameters.

### Affected Trust Domains

* Operational Trust

---

## OTT-04 Trust Degradation Event

### Description

An incident causing measurable reduction in stakeholder confidence.

### Example

Repeated incorrect recommendations reduce executive trust.

### Affected Trust Domains

* Operational Trust
* Governance Trust

---

# Mapping to Existing Frameworks

## TCTM and Existing Models

| TCTM Threat             | STRIDE                 | OWASP LLM Top 10 | MITRE ATLAS         |
| ----------------------- | ---------------------- | ---------------- | ------------------- |
| Prompt Injection        | Tampering              | LLM01            | Prompt Manipulation |
| Context Poisoning       | Tampering              | LLM02            | Data Poisoning      |
| Agent Hijacking         | Elevation of Privilege | LLM08            | Agent Manipulation  |
| Decision Drift          | N/A                    | Partial Coverage | N/A                 |
| Missing Accountability  | N/A                    | N/A              | N/A                 |
| Confidence Manipulation | N/A                    | N/A              | N/A                 |

---

# Research Gap

Existing frameworks provide extensive coverage of technical threats affecting AI systems.

However, they provide limited support for evaluating:

* trust degradation;
* decision integrity;
* accountability failures;
* governance weaknesses;
* confidence manipulation.

The TCTM Threat Taxonomy extends traditional approaches by introducing trust as a primary threat modeling dimension.

---

# Key Takeaway

The TCTM Threat Taxonomy provides a structured methodology for identifying threats that affect trust in autonomous AI systems. By focusing on trust manipulation, decision integrity, governance failures, and operational trust, the framework expands traditional cybersecurity models to address the unique challenges introduced by autonomous decision-making.

