# Unified-Kill-Chain-TryHackMe-Writeup
## Overview

The Unified Kill Chain (UKC) is a comprehensive framework developed to understand and dissect cyber attacks in a structured way. Published by Paul Pols in 2017 and updated in 2022, the UKC complements other models like the Lockheed Martin Kill Chain and MITRE ATT&CK by providing a detailed, realistic 18-phase structure covering the entire lifecycle of an attack.

This write-up summarizes the lessons from the TryHackMe **Unified Kill Chain** room and reflects on its practical value in threat modeling, red/blue team operations, and cybersecurity posture development.

---

## Learning Objectives

- Understand the purpose and benefits of cyber kill chain frameworks.
- Explore the 18 phases of the Unified Kill Chain.
- Analyze attacker behavior and how defensive measures can be mapped accordingly.
- Compare UKC with frameworks like MITRE ATT&CK and Lockheed Martin Kill Chain.
- Apply UKC to real-world threat modeling scenarios.

---

## What Is a Kill Chain?

A Kill Chain is a conceptual model from the military used to describe the stages of an attack. In cybersecurity, it maps out how adversaries gain, expand, and maintain access to systems or networks.

---

## Threat Modeling and UKC

Threat modeling involves:
1. Identifying critical systems and data.
2. Discovering vulnerabilities and weaknesses.
3. Planning mitigations and security controls.
4. Implementing policies for long-term protection.

UKC aids this process by identifying attack surfaces, methodologies, and attacker objectives.

---

## UKC Phases Breakdown

### **Phase: In (Initial Foothold)**

1. **Reconnaissance (TA0043)** – Collect public and private info (infra, emails, credentials).
2. **Weaponization (TA0001)** – Set up payload delivery methods (C2, reverse shells).
3. **Social Engineering (TA0001)** – Phishing, impersonation, and pretexting to gain access.
4. **Exploitation (TA0002)** – Execute code through software vulnerabilities.
5. **Persistence (TA0003)** – Maintain access via services, startup entries, or web shells.
6. **Defense Evasion (TA0005)** – Avoid detection by AVs, firewalls, IDS.
7. **Command & Control (TA0011)** – Establish secure communication back to attacker.
8. **Pivoting (TA0008)** – Move from public-facing systems into internal networks.

---

### **Phase: Through (Network Propagation)**

9. **Discovery (TA0007)** – Internal enumeration: users, processes, configs, shares.
10. **Privilege Escalation (TA0004)** – Abuse misconfigurations to gain admin or root.
11. **Execution (TA0002)** – Run scripts/malware to automate persistence and backdoors.
12. **Credential Access (TA0006)** – Dump creds, keylogging, memory scraping.
13. **Lateral Movement (TA0008)** – Access other systems using stolen creds or tools.

---

### **Phase: Out (Action on Objectives)**

14. **Collection (TA0009)** – Gather sensitive files, emails, logs, media.
15. **Exfiltration (TA0010)** – Encrypt, compress and stealthily extract data.
16. **Impact (TA0040)** – Encrypt, delete, deface, or DoS targets.
17. **Objectives** – Fulfill attacker’s goals (e.g., ransom, espionage, sabotage).
18. **Clean-Up (Implicit)** – Cover tracks or disable monitoring.

---

## Comparison to Other Frameworks

| Feature | Unified Kill Chain | MITRE ATT&CK | Lockheed Martin Kill Chain |
|--------|---------------------|--------------|-----------------------------|
| Release Year | 2017 | 2013 | 2011 |
| Number of Phases | 18 | ~14 (Tactics) | 7 |
| Scope | Full attack lifecycle | Technique-driven | Initial intrusion-focused |
| Recurrence Support | Yes (looping phases) | Partial | No |

---

## Why UKC Matters

- Offers **comprehensive insight** into attacker motives and movements.
- Assists blue teams in **mapping defenses** to every phase.
- Helps red teams simulate **realistic kill chains** during engagements.
- Enables better **threat intelligence correlation**.

---


## Skills Demonstrated

- Kill chain analysis and mapping
- Threat modeling methodology
- MITRE tactic and technique association
- Blue/red team cyber strategy
- Cyber threat intelligence (CTI) enhancement

---

## Use in a Cybersecurity Career

Understanding the Unified Kill Chain is essential for:
- SOC analysts (for detection and triage).
- Threat hunters (to predict attacker movement).
- Red teamers (to simulate adversarial behavior).
- Security architects (to implement layered defense).

This write-up serves as evidence of practical knowledge and application of a critical cybersecurity framework.


