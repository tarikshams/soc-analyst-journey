# SOC Role in Blue Team — Practical Challenge

**Platform:** TryHackMe
**Room:** [SOC Role in Blue Team](https://tryhackme.com/room/socroleinblueteam)

## Objective

The practical challenge was designed to test whether I could identify which cybersecurity role should handle different security situations.

Instead of treating every security problem as a SOC analyst's responsibility, I had to understand the responsibilities of different Blue Team and security roles.

---

## Role Matching Challenge

The challenge presented seven different situations and required the appropriate role to be selected.

The roles shown in the challenge were:

* SOC L1 Analyst
* SOC L2 Analyst
* Threat Researcher

The wider room also introduced roles such as SOC Engineer, GRC, CIRT, and other specialized defensive positions.

### How I approached the scenarios

| Situation                                                                  | Appropriate role  | Reason                                                         |
| -------------------------------------------------------------------------- | ----------------- | -------------------------------------------------------------- |
| SIEM creates an alert about a firewall brute-force attack                  | SOC L1 Analyst    | Initial alert triage is an L1 responsibility                   |
| HR manager reports a phishing campaign requiring deeper analysis           | SOC L2 Analyst    | More advanced investigation is appropriate                     |
| Office employee is hit by ransomware and immediate response is required    | CIRT              | A serious active incident requires incident-response expertise |
| Servers storing credit-card data require PCI DSS auditing                  | GRC               | Compliance and regulatory requirements fall under GRC          |
| Need to investigate a new framework version for vulnerabilities            | Threat Researcher | Requires research into emerging vulnerabilities and threats    |
| SIEM becomes unavailable because of a storage issue                        | SOC Engineer      | Security-tool infrastructure is an engineering responsibility  |
| FIN7 is actively targeting the company and its tactics need to be analyzed | Threat Researcher | Threat researchers study threat actors and their behavior      |

### Main lesson

The correct response to a security problem depends on **what kind of problem it is**.

For example:

```text
Alert needs initial triage
        ↓
SOC L1

Advanced investigation
        ↓
SOC L2

Security platform problem
        ↓
SOC Engineer

Compliance requirement
        ↓
GRC

Major active incident
        ↓
CIRT

Threat actor / vulnerability research
        ↓
Threat Researcher
```

---

# Final Challenge

The final challenge placed me in the role of a **CISO of TrySecureMe**.

Seven incidents were occurring simultaneously, and I had to assign the appropriate security roles to deal with them.

The challenge tested whether I could distinguish between:

* Alert triage
* Advanced investigation
* Threat research
* Security engineering
* Compliance
* Incident response

## Result

**Flag obtained:**

`[INSERT THE FLAG FROM THE COMPLETED CHALLENGE]`

I am leaving the flag as a placeholder because it was not included in the information documented here.

---

# What I Learned

The most useful part of this room was understanding that cybersecurity is divided into specialized responsibilities.

A SOC analyst should not automatically try to handle every security problem.

For example:

* A suspicious SIEM alert may start with **SOC L1**.
* A complex investigation may move to **SOC L2**.
* A broken SIEM may require a **SOC Engineer**.
* A major breach may require **CIRT**.
* A compliance requirement may involve **GRC**.
* Threat-actor research may involve a **Threat Intelligence / Threat Research** role.

This helped me understand the importance of **knowing when and where to escalate**.

## Career relevance

For someone starting in SOC L1, learning these boundaries is important because real security operations involve collaboration between multiple teams.

The SOC is therefore not an isolated department. It is part of a larger defensive security structure.

## Related Resources

* [TryHackMe — SOC Role in Blue Team](https://tryhackme.com/room/socroleinblueteam)
* [TryHackMe — SOC Fundamentals](https://tryhackme.com/room/socfundamentals)
* [TryHackMe — Junior Security Analyst Intro](https://tryhackme.com/room/jrsecanalystintrouxo)
* [TryHackMe — SOC Level 1 Path](https://tryhackme.com/path/outline/soclevel1)
* [JPCERT/CC](https://www.jpcert.or.jp/english/)
* [Mandiant](https://www.mandiant.com/)
* [AWS Security Incident Response](https://aws.amazon.com/security/incident-response/)

## Final Takeaway

The room showed me where a SOC fits within a larger security organization and how different defensive roles cooperate.

The important progression for me is not simply:

`Learn SOC → Get a job`

but rather:

`SOC L1 → gain broad experience → identify a specialization → develop deeper expertise`
