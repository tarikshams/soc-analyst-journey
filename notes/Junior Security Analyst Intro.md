# Junior Security Analyst Intro

**Platform:** TryHackMe
**Room:** [Junior Security Analyst Intro](https://tryhackme.com/room/jrsecanalystintrouxo)

## What is a Junior Security Analyst?

A Junior Security Analyst, commonly working at **SOC Level 1 (L1)**, is part of the defensive security team responsible for monitoring and investigating security alerts.

The role is often the first point of analysis when a security tool reports suspicious activity. The analyst needs to review the alert, understand what happened, collect relevant information, and decide whether the case can be closed, requires action, or should be escalated.

## What does a SOC L1 analyst do?

During a typical shift, an analyst may:

* Monitor security alerts and tickets.
* Investigate suspicious activity.
* Participate in SOC discussions and security workshops.
* Work with other teams when an incident requires their involvement.
* Keep up with new attacks, vulnerabilities, and defensive techniques.

The work is continuous because new threats and attack techniques appear regularly.

## The SOC environment

A Security Operations Center (SOC) is a team responsible for monitoring and protecting an organization's systems and infrastructure.

A Junior Security Analyst does not work alone. Different roles support different parts of the security operation.

### Junior Security Analyst

Responsible mainly for the **initial investigation of alerts**.

A simplified workflow is:

```text
Security Alert
      ↓
Initial Investigation
      ↓
Collect Evidence
      ↓
Determine Severity / Legitimacy
      ↓
Close / Take Action / Escalate
```

### Senior Analyst

Handles more complicated investigations and provides guidance to Junior Analysts when an alert requires deeper analysis.

### SOC Engineer

Maintains and configures security tools and alerting systems. While the analyst investigates alerts, the SOC Engineer helps make sure the underlying security tooling works properly and generates useful alerts.

### SOC Manager

Oversees the SOC operation, coordinates the team, and reports security-related results to management.

### Incident Responder

Becomes involved when a significant security incident requires dedicated incident-response and containment activities.

## Why alert investigation matters

A SOC analyst may receive a large number of alerts during a shift. Not every alert represents a real attack.

The analyst therefore needs to distinguish between:

* Benign activity
* Suspicious activity
* Confirmed malicious activity

This means the job is not simply:

> "Look at alerts."

It is:

> **Review → investigate → make a decision → respond or escalate.**

## Practical alert investigation

The room includes a simulated SOC environment where I investigate alerts using an alert dashboard.

The investigation involves:

1. Opening the alert dashboard.
2. Reviewing the available alerts.
3. Identifying the malicious IP address.
4. Escalating the alert to the appropriate person.
5. Blocking the malicious IP using the firewall.
6. Checking the response after the blocking action.

This demonstrates a simplified version of the process an analyst may follow when dealing with a malicious network indicator.

## Investigation mindset

One useful way to think about the investigation is:

```text
Alert
  ↓
Indicator
  ↓
Investigation
  ↓
Decision
  ↓
Response
  ↓
Verification
```

For example, an IP address appearing in an alert is only an indicator. The analyst needs to determine whether it is actually malicious and what action should be taken.

## My practical findings

These are the values I obtained from the TryHackMe lab:

| Investigation item | Finding            |
| ------------------ | ------------------ |
| Malicious IP       | `[add my finding]` |
| Escalated to       | `[add my finding]` |
| Firewall response  | `[add my finding]` |

## Key lessons

### 1. SOC L1 is an investigation role

The analyst is not simply watching a dashboard. They need to interpret alerts and determine what they mean.

### 2. Escalation is part of the job

A Junior Analyst does not have to solve every incident alone. Cases that require additional expertise can be escalated to senior analysts or the appropriate response team.

### 3. Indicators need context

An IP address, domain, username, file, or process can be an important indicator, but an analyst should investigate the context around it before deciding what it means.

### 4. Defensive actions should be verified

After taking an action such as blocking an IP, the analyst should check whether the action succeeded and record the result.

### 5. Continuous learning is necessary

The cybersecurity landscape changes constantly. A SOC analyst needs to follow new attacks, vulnerabilities, threat actors, and defensive techniques.

## Useful resources

* [TryHackMe — Junior Security Analyst Intro](https://tryhackme.com/room/jrsecanalystintrouxo) — the room used for this learning.
* [TryHackMe — SOC Fundamentals](https://tryhackme.com/room/socfundamentals) — useful background on SOC roles and processes.
* [The Hacker News](https://thehackernews.com/) — useful for following current cybersecurity incidents and security news.

## Personal takeaway

This room gave me an introduction to what a SOC L1 analyst actually does. The practical exercise was especially useful because it showed that the role involves moving from an alert to investigation and then to an appropriate defensive action.
There are many open-source databases out there, like AbuseIPDB, and Cisco Talos Intelligence, where you can perform a reputation and location check for the IP address. Most security analysts use these tools to aid them with alert investigations. You can also make the Internet safer by reporting the malicious IPs, for example, on AbuseIPDB.
