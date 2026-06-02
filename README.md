# Trust-Centric Threat Modeling (TCTM)

A framework for evaluating security, governance and decision integrity in autonomous AI systems.

## Research Areas

- AI Security
- AI Governance
- Trustworthy AI
- Agentic AI
- Cybersecurity Strategy

## Framework Components

- Trust Domains
- Threat Taxonomy
- Trust Risk Matrix
- Trust Maturity Model

## TCTM Architecture

Estrutura:
```text
+----------------------+
|    Trust Domains     |
+----------------------+
           |
           v
+----------------------+
|   Threat Taxonomy    |
+----------------------+
           |
           v
+----------------------+
|  Trust Risk Matrix   |
+----------------------+
           |
           v
+----------------------+
| Trust Maturity Model |
+----------------------+  
```
O TCTM evolui de identificação de domínios para avaliação de maturidade.  

## Trust Domains
Estrutura:
```text
                    +----------------+
                    |      TCTM      |
                    +----------------+
                             |
    ---------------------------------------------------
    |          |          |          |               |
    v          v          v          v               v

+----------+ +----------+ +----------+ +----------+ +----------+
| Identity | | Context  | | Decision | |Governance| |Operational|
|  Trust   | |  Trust   | |  Trust   | |  Trust   | |  Trust   |
+----------+ +----------+ +----------+ +----------+ +----------+

```

## Threat Taxonomy
Estrutura:
```text
                    +------------------+
                    |   TCTM Threats   |
                    +------------------+
                             |
 ---------------------------------------------------
 |                 |                 |              |
 v                 v                 v              v

+---------+   +---------+     +---------+    +---------+
|   TMT   |   |   DIT   |     |   GFT   |    |   OTT   |
+---------+   +---------+     +---------+    +---------+

Trust        Decision       Governance     Operational
Manipulation Integrity      Failure        Trust
Threats      Threats        Threats        Threats


TMT
 ├─ Prompt Injection
 ├─ Context Poisoning
 └─ Confidence Manipulation

DIT
 ├─ Hallucinated Actions
 ├─ Decision Drift
 └─ Misalignment

```
## Author

Tharcilia Rollemberg
