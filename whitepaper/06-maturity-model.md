# 6. TCTM Threat Taxonomy

## 6.1 Introduction

Autonomous AI Agents introduce a new class of risks that cannot be fully represented through traditional cybersecurity taxonomies.

While existing frameworks effectively categorize attacks against infrastructure, applications, networks, and machine learning models, they provide limited visibility into threats that undermine trust, governance, and decision integrity.

The TCTM Threat Taxonomy was developed to address this gap.

Rather than focusing exclusively on technical compromise, the taxonomy classifies threats according to their ability to degrade organizational trust in autonomous systems.

The taxonomy serves four primary objectives:

- Standardize threat identification;
- Support trust-oriented risk assessment;
- Improve governance visibility;
- Enable trust-centric security controls.
  
The taxonomy is organized into five major threat families.

Each family corresponds to one or more Trust Domains and represents a distinct mechanism through which trust can be compromised.

## 6.2 Taxonomy Structure
Each threat is identified using the following format:
```
<Category>-<Threat ID>  
```

**Example:**  
TMT-01  

**Where:**  
TMT = Trust Manipulation Threat
01 = Unique threat identifier

### Threat Classification Model
Each threat contains:
| Attribute | Description |
|-----------|-----------|
| Threat ID | Unique Identifier |
| Threat Name | Threat Description |
| Trust Domain Impacted | Associated Trust Domain |
| Attack Vector | Method of Execution |
| Organizational Impact | Business Consequence |
| Trust Impact Level | 1–5 |


## 6.3 Category A — Trust Manipulation Threats (TMT)
**Definition**  
Threats that manipulate the information environment used by autonomous agents.

These attacks seek to influence how the agent perceives reality.

Rather than directly attacking infrastructure, attackers manipulate context.


**Why This Matters**  
Autonomous agents depend heavily on contextual information.

If context becomes compromised, trustworthy decisions become impossible.

### TMT-01 — Prompt Injection  

**Description**  
Malicious instructions embedded within user input, documents, emails, websites, or data sources designed to alter agent behavior.

**Example**  
An invoice contains hidden instructions directing an AI financial agent to ignore validation procedures.

- Impacted Domains
- Context Trust
- Decision Trust
**Trust Impact**
5 (Critical)

### TMT-02 — Context Poisoning  

**Description**  
Manipulation of knowledge sources used by Retrieval-Augmented Generation systems.  

**Example**  
An attacker inserts false policy documents into a corporate knowledge repository.

**Impacted Domains**
- Context Trust
- Governance Trust
  
**Trust Impact**
5 (Critical)

### TMT-03 — Memory Corruption  

**Description**  
Modification of stored memory used by the agent.  

**Example**  
An attacker influences long-term memory so that future recommendations become biased.

**Impacted Domains**  
- Context Trust
- Decision Trust
  
**Trust Impact**
4 (High)

### TMT-04 — Knowledge Manipulation  

**Description**  
Corruption of external information sources used during reasoning.  

**Example**  
Compromised third-party API providing inaccurate data.  
**Trust Impact**  
4 (High)

## 6.4 Category B — Decision Integrity Threats (DIT)  

**Definition**  
Threats that affect the quality, reliability, consistency, and alignment of decisions.  

Unlike traditional attacks, these threats may occur without malicious actors.  

**Why This Matters**  
The primary value of autonomous agents lies in their decisions.   
If decision integrity deteriorates, organizational trust collapses.  

### DIT-01 — Goal Misalignment  

**Description**  
The agent optimizes behavior that diverges from intended organizational objectives.    

**Example**  
A customer service agent prioritizes rapid ticket closure rather than customer satisfaction.  

**Impacted Domains**  
Decision Trust  

**Trust Impact**  
5 (Critical)

### DIT-02 — Decision Drift  

**Description**  
Progressive deviation in decision-making patterns over time.  

**Example**  
An HR agent gradually develops hiring preferences inconsistent with organizational policies.

**Impacted Domains**  
- Decision Trust  
- Operational Trust
  
**Trust Impact**  
4 (High)  

### DIT-03 — Hallucinated Actions   

**Description**  
Actions based on inaccurate or fabricated information.  

**Example**  
An AI legal assistant references nonexistent regulations.  

**Impacted Domains**  
- Decision Trust
- 
**Trust Impact**  
5 (Critical)  

### DIT-04 — Risk Amplification  

**Description**  
Autonomous behavior unintentionally magnifies existing organizational risks.  

**Example**  
An agent repeatedly recommends increasingly aggressive financial strategies. 

**Trust Impact**  
4 (High)

## 6.5 Category C — Governance Failure Threats (GFT)  

**Definition**  

Threats resulting from insufficient oversight, accountability, or policy enforcement.

These threats originate primarily from organizational weaknesses rather than technical vulnerabilities.

**Why This Matters**  
Many AI incidents occur because organizations fail to govern autonomous behavior appropriately.

### GFT-01 — Lack of Human Oversight
**Description**
Autonomous actions occur without meaningful human review.
**Trust Impact**
5 (Critical)  

### GFT-02 — Missing Accountability  
**Description**  
No clear ownership exists for agent decisions.  
**Example** 
Multiple departments use an AI agent, but none assume responsibility for outcomes. 
**Trust Impact** 
4 (High)

### GFT-03 — Untraceable Decisions  
**Description** 
Decisions cannot be reconstructed or audited.  
**Example**  
An executive recommendation is generated without supporting evidence.
**Trust Impact**  
5 (Critical)  

### GFT-04 — Policy Bypass  
**Description**  
Agent behavior circumvents established governance controls. 
**Trust Impact**  
4 (High)

## 6.6 Category D — Operational Trust Threats (OTT)  
**Definition**  
Threats affecting the reliability and resilience of autonomous operations.  

### OTT-01 — Agent Hijacking  
**Description**  
An attacker gains influence over agent behavior.  
**Trust Impact**  
5 (Critical)

### OTT-02 — Tool Abuse  
**Description**  
Misuse of integrated tools or APIs.  
**Example**  
An agent performs unauthorized actions through connected enterprise systems.  
**Trust Impact**  
5 (Critical)

### OTT-03 — Privilege Escalation  
**Description**  
An agent obtains permissions beyond its intended scope.  
**Trust Impact**  
5 (Critical)

### OTT-04 — Autonomous Cascade Failure  
**Description**  
Failure of one agent propagates through multiple connected agents.  
**Example**  
A compromised planning agent influences downstream execution agents.  
**Trust Impact**
5 (Critical)  

## 6.7 Category E — Trust Erosion Threats (TET)  
**Definition**  
Threats that gradually reduce confidence in autonomous systems.  

These threats may not generate immediate security incidents but can significantly impact adoption and business value.  

**Why This Matters**  
Trust is difficult to build and easy to lose.  

### TET-01 — Inconsistent Decisions  
**Description**  
Similar situations produce materially different outcomes.  
**Trust Impact**  
4 (High)

### TET-02 — Opaque Reasoning  
**Description**  
Decision logic cannot be explained.  
**Trust Impact**  
4 (High)

### TET-03 — Loss of Predictability  
**Description**  
Stakeholders become unable to anticipate behavior.  
**Trust Impact**  
5 (Critical)

### TET-04 — Confidence Inflation  
**Description**  
The agent appears more reliable than it actually is.  
**Example**  
Users place excessive confidence in recommendations without verification.
**Trust Impact**  
5 (Critical)  

## 6.8 Trust Impact Classification
The TCTM framework introduces a dedicated Trust Impact metric.
| Level | Description |
|-----------|-----------|
| 1 | Negligible |
| 2 | Minor |
| 3 | Moderate |
| 4 | Significant |
| 5 | Critical|

Unlike traditional impact metrics, Trust Impact evaluates the degree to which confidence in the autonomous system is affected.

## 6.9 Cross-Mapping to Existing Frameworks  

TCTM complements—not replaces—existing methodologies.  

| TCTM Threat | STRIDE | OWASP LLM Top 10 | MITRE ATLAS |
|------------|---------|------------------|-------------|
| Prompt Injection | Tampering | LLM01: Prompt Injection | Prompt Manipulation |
| Context Poisoning | Tampering | LLM02: Insecure Output Handling / Data Poisoning | Data Poisoning |
| Agent Hijacking | Elevation of Privilege | LLM08: Excessive Agency | Agent Manipulation |
| Decision Drift | N/A | Partial Coverage | N/A |
| Missing Accountability | N/A | N/A | N/A |
| Confidence Inflation | N/A | N/A | N/A |

Notably, several TCTM threats have no direct representation in traditional frameworks.

This highlights the importance of trust-oriented analysis.

## 6.10 Taxonomy Application Workflow 

Organizations should apply the taxonomy through the following process:  
```text
Identify Agent
       ↓
Identify Trust Domains
       ↓
Map Threat Categories
       ↓
Assess Trust Impact
       ↓
Calculate Risk
       ↓
Apply Controls
       ↓
Monitor Continuously
```
This workflow creates a repeatable methodology for trust-centric threat assessments.

## 6.11 Chapter Conclusion  

The TCTM Threat Taxonomy expands traditional cybersecurity thinking by introducing a structured classification of threats that undermine trust in autonomous AI systems.

Rather than focusing exclusively on technical compromise, the taxonomy addresses threats affecting context, decisions, governance, operations, and organizational confidence.

By organizing threats into five categories—Trust Manipulation, Decision Integrity, Governance Failure, Operational Trust, and Trust Erosion—the framework provides organizations with a practical mechanism for identifying and managing risks unique to autonomous agents.

This taxonomy forms the analytical foundation for the next component of the framework: the Trust Risk Matrix, which introduces a methodology for quantifying trust-related risk and prioritizing mitigation efforts.

## Key Takeaway
Not all threats compromise systems. Some compromise trust. The TCTM Threat Taxonomy recognizes that in autonomous AI environments, attacks against context, decisions, governance, and confidence can be as damaging as traditional cybersecurity incidents.


