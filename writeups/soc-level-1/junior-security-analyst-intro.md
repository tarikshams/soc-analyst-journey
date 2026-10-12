# Junior Security Analyst Intro — Practical Investigation

**Platform:** TryHackMe
**Room:** [Junior Security Analyst Intro](https://tryhackme.com/room/jrsecanalystintrouxo)

## Objective

Practice the basic workflow of a SOC Level 1 analyst by investigating a security alert and responding to a malicious IP address.

## Scenario

The room simulates a SOC environment where a Junior Security Analyst is responsible for reviewing security alerts.

The task provides an alert dashboard containing suspicious activity. My goal was to identify the malicious IP, determine who the alert should be escalated to, block the IP using the firewall, and verify the result.

## Investigation Process

### 1. Review the alerts

I opened the simulated alert dashboard and reviewed the available alerts.

The objective was to identify the alert associated with malicious activity rather than treating every alert as equally important.

### 2. Identify the malicious IP

The suspicious alert contained an IP address associated with the malicious activity.

**Malicious IP:**

`[INSERT THE IP ADDRESS YOU FOUND]`

### 3. Escalate the alert

After identifying the malicious IP, the alert needed to be escalated to the appropriate person in the SOC.

**Escalated to:**

`[INSERT THE PERSON/ROLE SHOWN IN THE LAB]`

### 4. Block the IP

I then used the simulated firewall functionality to block the malicious IP address.

### 5. Verify the result

After blocking the IP, the firewall displayed a response confirming the result.

**Firewall response:**

`[INSERT THE EXACT MESSAGE SHOWN BY THE LAB]`

## Investigation Flow

```text
Alert Dashboard
       ↓
Identify suspicious alert
       ↓
Find malicious IP
       ↓
Escalate alert
       ↓
Block IP on firewall
       ↓
Verify firewall response
```

## What this exercise demonstrated

This exercise showed a simplified SOC investigation workflow:

* Alerts need to be reviewed and investigated.
* Indicators such as IP addresses can be used during an investigation.
* A Junior Analyst may need to escalate an alert instead of handling everything alone.
* Defensive actions can be taken when malicious activity is confirmed.
* The result of a defensive action should be verified.

## Key takeaway

The important part of the exercise was not simply blocking an IP. It demonstrated the sequence an analyst follows:

**Detect → Investigate → Escalate → Respond → Verify**

## Resources

* [TryHackMe — Junior Security Analyst Intro](https://tryhackme.com/room/jrsecanalystintrouxo)
* [TryHackMe — SOC Fundamentals](https://tryhackme.com/room/socfundamentals)
* [The Hacker News](https://thehackernews.com/)

