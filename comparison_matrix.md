# Tenable Identity Exposure Attack Path Coverage Matrix  
**Tenable Identity Exposure vs BloodHound**

**Sources**
- BloodHound documentation: https://bloodhound.specterops.io/get-started/introduction  
- Tenable Identity Exposure public SaaS documentation

---

## Core Data Model & Purpose

| Capability | Tenable Identity Exposure | BloodHound |
|-----------|---------------------------|------------|
| Product Origin | Alsid acquisition | SpecterOps original research |
| Primary Purpose | Identity configuration & exposure analysis | Active Directory attack path analysis |
| Core Data Model | Configuration/state-based | Graph-based (nodes & edges) |
| Underlying Graph Engine | ❌ Not documented | ✔ Neo4j |
| Attack Path Modeling | ❌ Not documented | ✔ Explicitly documented |
| Privilege Escalation Modeling | ❌ Not documented | ✔ Documented |
| Lateral Movement Modeling | ❌ Not documented | ✔ Documented |

---

## Data Collection Architecture

| Capability | Tenable Identity Exposure | BloodHound |
|-----------|---------------------------|------------|
| Collection Method | Dedicated relay / collector | SharpHound collector |
| Agentless Collection | ❌ No | ✔ Yes |
| Requires Domain Admin | Not documented | ❌ No |
| Snapshot-Based Collection | ✔ Yes | ✔ Yes |
| Continuous / Near-Real-Time | Partial | ❌ No |
| Forest & Domain Scope | ✔ Yes | ✔ Yes |

---

## Analysis Capabilities

| Capability | Tenable Identity Exposure | BloodHound |
|-----------|---------------------------|------------|
| Graph Traversal | ❌ Not documented | ✔ Native |
| Shortest Attack Path Analysis | ❌ Not documented | ✔ Documented |
| Multi-Hop Escalation Paths | ❌ Not documented | ✔ Documented |
| Transitive Permission Analysis | ❌ Not documented | ✔ Documented |
| Delegation Abuse Modeling | ❌ Not documented | ✔ Documented |
| Kerberos Attack Modeling | ❌ Not documented | ✔ Documented |

---

## Query & Exploration

| Capability | Tenable Identity Exposure | BloodHound |
|-----------|---------------------------|------------|
| Interactive Graph Exploration | ❌ No | ✔ Yes |
| Custom Query Language | ❌ No | ✔ Cypher |
| Analyst-Driven Exploration | ❌ No | ✔ Yes |
| Ad-Hoc Relationship Queries | ❌ No | ✔ Yes |
| Rule-Based Findings | ✔ Yes | ❌ (analysis-driven) |

---

## Output & Integration

| Capability | Tenable Identity Exposure | BloodHound |
|-----------|---------------------------|------------|
| Native Data Export | Limited (CSV guidance) | ✔ Yes |
| Public API | ❌ Not publicly documented | ❌ Community / ✔ Enterprise |
| Machine-Readable Graph Export | ❌ No | ✔ Yes |
| SIEM Integration | Indirect (CSV → BI tools) | ✔ Direct (JSON / Splunk apps) |
| External Tooling Ecosystem | ❌ Minimal | ✔ Extensive |

---

## User Model & Accessibility

| Capability | Tenable Identity Exposure | BloodHound |
|-----------|---------------------------|------------|
| Requires Admin UI Access | ✔ Yes | ❌ No |
| Security Analyst Friendly | ❌ Limited | ✔ Yes |
| Executive-Ready Views | UI-only | ❌ Not claimed |
| Security Engineer Usability | ❌ Constrained | ✔ Native |
| Non-Admin Data Consumption | ❌ No | ✔ Yes |

---

## Transparency & Trust Model

| Capability | Tenable Identity Exposure | BloodHound |
|-----------|---------------------------|------------|
| Attack Logic Visibility | ❌ Opaque | ✔ Transparent |
| Detection Logic Auditable | ❌ No | ✔ Yes |
| Community Validation | ❌ No | ✔ Extensive |
| Research-Driven Foundation | ❌ Not documented | ✔ Yes |
| Marketing Dependency | High | Low |

---

## Fact-Based Summary

- BloodHound is explicitly documented as a **graph-based Active Directory attack path analysis platform**
- Tenable Identity Exposure is documented as a **configuration and exposure analysis product**, not an attack graph engine
- There is **no documented attack path traversal, shortest-path analysis, or graph query capability** in Tenable Identity Exposure
- Claims that Tenable Identity Exposure replaces BloodHound are **not supported by either product’s documentation**

---
