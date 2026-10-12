# SOC Role in Blue Team

**Platform:** TryHackMe
**Room:** [SOC Role in Blue Team](https://tryhackme.com/room/socroleinblueteam)

## Overview

The SOC is part of the **Blue Team**, which is responsible for defending an organization's systems, data, and users against cyber threats.

A SOC L1 analyst is usually one of the entry points into defensive cybersecurity. From there, an analyst can move toward more advanced SOC roles or specialize in areas such as incident response, threat intelligence, digital forensics, security engineering, or application security.

---

## Security Hierarchy

The exact security structure differs between organizations because their security priorities are different.

For example:

* A law firm may prioritize the confidentiality of legal documents.
* A factory may prioritize the availability of production systems.
* A hospital may prioritize patient safety and system availability.

In larger organizations, the **CISO (Chief Information Security Officer)** or a similar senior security leader usually oversees the organization's cybersecurity strategy and departments.

### Simplified hierarchy

```text
                    CEO / Executive Management
                              │
                             CISO
                              │
          ┌───────────────────┼───────────────────┐
          │                   │                   │
       Red Team             GRC Team           Blue Team
    Offensive Security     Governance &        Defensive
                           Compliance           Security
                                                  │
                                    ┌─────────────┼─────────────┐
                                    │             │             │
                                   SOC           CIRT      Specialized
                                                                Roles
```

The exact structure can vary from company to company.

---

# Main Security Teams

## Red Team

The Red Team focuses on **offensive security**.

Typical activities include:

* Penetration testing
* Ethical hacking
* Finding vulnerabilities
* Simulating attacks against an organization

The goal is to discover weaknesses before real attackers can exploit them.

---

## GRC Team

**GRC = Governance, Risk, and Compliance.**

This team focuses on security policies, risk management, and compliance with relevant standards and regulations.

For example, organizations handling payment-card information may need to consider standards such as **PCI DSS**.

The GRC team is therefore concerned not only with technical attacks but also with whether the organization follows appropriate security requirements.

---

## Blue Team

The Blue Team focuses on **defensive security**.

Its purpose is to:

* Monitor for attacks
* Detect suspicious activity
* Investigate security incidents
* Respond to threats
* Improve defensive controls

SOC analysts, SOC engineers, and incident responders are examples of Blue Team roles.

---

# Security Operations Center (SOC)

The **SOC** is a central part of an organization's defensive security operation.

It monitors security events and investigates potential threats.

### Common SOC roles

| Role           | Main responsibility                    |
| -------------- | -------------------------------------- |
| SOC L1 Analyst | Initial alert triage and investigation |
| SOC L2 Analyst | More advanced investigation            |
| SOC Engineer   | Configure and maintain security tools  |
| SOC Manager    | Manage the SOC team and operation      |

### SOC L1

The L1 analyst is generally the first analyst to examine an alert.

Typical responsibilities include:

* Alert triage
* Initial investigation
* Collecting evidence
* Determining whether activity is suspicious
* Escalating complex cases

### SOC L2

The L2 analyst handles more advanced investigations after cases are escalated from L1.

The natural progression from an L1 position is therefore commonly:

```text
SOC L1
  ↓
SOC L2
```

This is a common path, not a requirement. Analysts can eventually specialize in other areas.

### SOC Engineer

SOC engineers focus on the technology supporting the SOC.

For example, they may configure and maintain:

* SIEM platforms
* EDR solutions
* Alerting systems
* Security monitoring infrastructure

If a security monitoring system is malfunctioning or unavailable, the SOC engineer may be the appropriate person to investigate the technical problem.

---

# Cyber Incident Response Team (CIRT)

A **Cyber Incident Response Team (CIRT)**, also known as **CSIRT** or **CERT**, deals with serious or urgent cybersecurity incidents.

Think of CIRT as the organization's specialized emergency response capability.

A CIRT may become involved when:

* A major breach occurs.
* An attack is spreading.
* The SOC cannot contain the incident.
* Immediate incident-response expertise is required.

### Examples

* [JPCERT/CC](https://www.jpcert.or.jp/english/)
* [Mandiant](https://www.mandiant.com/)
* [AWS Security Incident Response](https://aws.amazon.com/security/incident-response/)

A useful distinction is:

```text
SOC
 ↓
Monitor + Detect + Investigate
 ↓
If incident becomes serious / requires deeper response
 ↓
CIRT / Incident Response
```

---

# Specialized Blue Team Roles

Large organizations may have specialists who focus deeply on particular areas.

## Digital Forensics Analyst

Investigates evidence from systems such as:

* Disk storage
* Memory
* Files
* System artifacts

The goal is to determine what happened and uncover evidence that may not be immediately visible.

## Threat Intelligence Analyst

Researches:

* Threat actors
* Campaigns
* Malware
* Indicators of compromise
* Emerging threats

Threat intelligence helps defenders understand who may be attacking them and how those attackers operate.

## Application Security Engineer

Focuses on securing applications and the software development lifecycle.

The goal is to identify and reduce security problems before applications reach production.

## AI Security Researcher

Researches threats involving AI systems and develops ways to defend against them.

---

# SOC Career Path

A SOC L1 position can provide broad exposure to cybersecurity because analysts encounter different types of attacks and security technologies.

A simplified career path is:

```text
SOC L1 Analyst
       ↓
SOC L2 Analyst
       ↓
Senior / Specialized Security Role
       ↓
Security Specialist / Leadership
```

However, the path does not have to remain within the SOC.

An analyst may discover an interest in:

* Security engineering
* Incident response
* Threat intelligence
* Digital forensics
* Application security
* Security management

---

# Building SOC Skills

The room recommends developing core SOC skills while also gaining practical experience.

Useful activities include:

* Practicing through cybersecurity labs
* Participating in CTFs
* Following cybersecurity news
* Learning security tools
* Understanding common attacks
* Developing investigation skills

TryHackMe's [SOC Level 1 path](https://tryhackme.com/path/outline/soclevel1) is one of the resources associated with this learning journey.

The room also introduces the [Security Analyst Level 1 certification](https://tryhackme.com/certification/security-analyst-level-1) as a possible certification path.

---

# Internal SOC vs MSSP

Not every organization operates its own SOC.

Some organizations outsource SOC services to a **Managed Security Services Provider (MSSP)**.

### Internal SOC

An internal SOC works directly for the organization it protects.

Example:

```text
Bank
 ↓
Internal SOC
 ↓
Protects the bank's systems
```

The analysts generally focus on one organization's environment and security tools.

### MSSP

An MSSP provides security services to other organizations.

Example:

```text
MSSP
 ├── Customer A
 ├── Customer B
 ├── Customer C
 └── Customer D
```

An analyst working at an MSSP may investigate incidents across many different customer environments.

### Comparison

|             | Internal SOC                                  | MSSP                                        |
| ----------- | --------------------------------------------- | ------------------------------------------- |
| Environment | One organization                              | Multiple customers                          |
| Tools       | Usually a smaller set of organizational tools | Potentially many different platforms        |
| Work pace   | May have comparatively predictable shifts     | Often more alert-driven and fast-paced      |
| Exposure    | Deep knowledge of one environment             | Exposure to many environments and incidents |
| Learning    | Deep specialization                           | Broad experience across customers           |

Working at an MSSP can therefore provide significant exposure to different technologies and security incidents, although the workload can also be demanding.

---

# Choosing the Right Security Role

The room's final challenge demonstrates that different security problems require different specialists.

A useful mental model is:

```text
Basic alert triage
        ↓
     SOC L1

Advanced investigation
        ↓
     SOC L2

Security tooling problem
        ↓
   SOC Engineer

Major / urgent incident
        ↓
       CIRT

Attacker behaviour / threat research
        ↓
 Threat Researcher

Compliance / regulatory issue
        ↓
       GRC
```

The key lesson is that cybersecurity is a team effort. No single role is expected to handle every type of security problem.

---

# Key Takeaways

1. **Blue Team = defensive security.**
2. **SOC is a major component of the Blue Team.**
3. **SOC L1 analysts perform initial alert triage and investigation.**
4. **SOC L2 analysts handle more advanced investigations.**
5. **SOC Engineers maintain and configure security monitoring tools.**
6. **CIRT handles serious or urgent cyber incidents.**
7. **GRC focuses on governance, risk, and compliance.**
8. **Red Team focuses on offensive security.**
9. **A CISO generally oversees the organization's cybersecurity strategy at a senior level.**
10. **An MSSP provides security services to multiple external customers.**
11. **SOC L2 is a natural next step after SOC L1, but specialization is also possible.**

## Useful Resources

* [TryHackMe — SOC Role in Blue Team](https://tryhackme.com/room/socroleinblueteam)
* [TryHackMe — Junior Security Analyst Intro](https://tryhackme.com/room/jrsecanalystintrouxo)
* [TryHackMe — SOC Fundamentals](https://tryhackme.com/room/socfundamentals)
* [TryHackMe — SOC Level 1 Path](https://tryhackme.com/path/outline/soclevel1)
* [JPCERT/CC](https://www.jpcert.or.jp/english/)
* [Mandiant](https://www.mandiant.com/)
* [AWS Security Incident Response](https://aws.amazon.com/security/incident-response/)
* [Security Analyst Level 1 Certification](https://tryhackme.com/certification/security-analyst-level-1)

## Personal Takeaway

This room helped me understand where a SOC L1 analyst fits within the wider cybersecurity structure. SOC is part of the defensive Blue Team, but it works alongside other functions such as GRC, Red Team, CIRT, and specialized security roles.

The main thing I learned is that progressing in cybersecurity does not mean following only one fixed career path. SOC L1 can provide broad exposure that can later lead toward SOC L2, incident response, security engineering, threat intelligence, forensics, or other specialized areas.
