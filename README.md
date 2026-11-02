# secbyte-email-security-authentication-forensics-digital-evidence-ctf-labs
A practical collection of cybersecurity CTF labs covering email security protocols (SPF, DKIM, DMARC, SMTP flow), email header forensics &amp; inbox spoofing triage, Business Email Compromise (BEC) wire fraud analysis, and digital forensics case documentation (chain of custody, evidence timelines, expert testimony prep).
# Email Authentication, Header Forensics, BEC Triage & Digital Evidence Courtroom CTF Labs

Welcome to the **Email Authentication, Header Forensics, BEC Triage & Digital Evidence Courtroom CTF Lab Collection**. This repository serves as an organized, searchable catalog of practical cybersecurity labs hosted on Learn SecByte.

This collection focuses on technical mail routing protocols, deep header forensic analysis, account takeover triage, and legal evidence handling—spanning **Email Security Architecture & Authentication Defense (SPF alignment, DKIM cryptographic validation, DMARC policy enforcement, SMTP flow analysis)**, **Email Header Forensics & BEC Triage (Inbox forensics, spoofing triage, silent invoice wire fraud)**, and **Digital Evidence Handling, Case Documentation & Courtroom Preparation (Courier incident, chain of custody, evidence timeline construction, expert testimony)**.

---

## Lab Collection Index

### 1. Email Security Architecture, Authentication & Protocol Defense
* **Email Security Fundamentals**  
  *Lab Link:* [https://learn.secbyte.org/ctf/email-security-fundamentals](https://learn.secbyte.org/ctf/email-security-fundamentals)  
  *Focus:* Core principles of enterprise mail security, evaluating transport-layer security (STARTTLS), understanding hop-by-hop trust, and preventing open relay abuses.

* **SPF Configuration: Mail Sender Trust Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/spf-configuration-mail-sender-trust-lab](https://learn.secbyte.org/ctf/spf-configuration-mail-sender-trust-lab)  
  *Focus:* Authoring and auditing Sender Policy Framework (SPF) DNS records, resolving IP include limits (`10-lookup` ceiling), configuring softfail (`~all`) vs. hardfail (`-all`), and validating `Return-Path` headers.

* **DKIM Validation: Mail Authentication Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/dkim-validation-mail-authentication-lab](https://learn.secbyte.org/ctf/dkim-validation-mail-authentication-lab)  
  *Focus:* Validating DomainKeys Identified Mail (DKIM) RSA/Ed25519 signatures, auditing canonicalization modes (`relaxed/simple`), tracking selector DNS records, and detecting body hash tampered messages.

* **DMARC Policy Defense Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/dmarc-policy-defense-lab](https://learn.secbyte.org/ctf/dmarc-policy-defense-lab)  
  *Focus:* Deploying Domain-based Message Authentication, Reporting, and Conformance (DMARC) policies, enforcing SPF/DKIM domain alignment, parsing aggregate RUA/RUF XML reports, and transitioning to `p=reject`.

* **SMTP Sleuth: Mail Flow and Misconfigurations**  
  *Lab Link:* [https://learn.secbyte.org/ctf/smtp-sleuth-mail-flow-and-misconfigurations](https://learn.secbyte.org/ctf/smtp-sleuth-mail-flow-and-misconfigurations)  
  *Focus:* Analyzing raw Simple Mail Transfer Protocol (SMTP) command sequences (`HELO`/`EHLO`, `MAIL FROM`, `RCPT TO`), detecting relay misconfigurations, and debugging delivery failures.

<Image src="image_agent_tag_14930242868309732452" alt="Diagram showing email MUA, MTA, and MDA components during message transmission" caption="Mail Transfer Agent (MTA) & Hop-by-Hop Routing Architecture" />

---

### 2. Email Forensics, Spoofing Triage & Business Email Compromise
* **Email Forensics: The Inbox Incident**  
  *Lab Link:* [https://learn.secbyte.org/ctf/email-forensics-the-inbox-incident](https://learn.secbyte.org/ctf/email-forensics-the-inbox-incident)  
  *Focus:* Extracting raw RFC 5322 message files (`.eml`), parsing MIME multipart structures, recovering deleted mailbox artifacts, and validating message integrity hashes.

* **Email Header Forensics Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/email-header-forensics-lab](https://learn.secbyte.org/ctf/email-header-forensics-lab)  
  *Focus:* Trace hop-by-hop `Received:` timestamps, analyze `Authentication-Results` headers, detect spoofed `From:` display names against actual `X-Originating-IP` addresses.

* **Phishing Detection Lab: Inbox Forensics and Spoofing Triage**  
  *Lab Link:* [https://learn.secbyte.org/ctf/phishing-detection-lab-inbox-forensics-and-spoofing-triage](https://learn.secbyte.org/ctf/phishing-detection-lab-inbox-forensics-and-spoofing-triage)  
  *Focus:* Triaging domain spoofing techniques (Cousin domains, IDN homograph attacks), evaluating lookalike header anomalies, and building automated inbox quarantine rules.

* **Silent Invoice: Business Email Compromise**  
  *Lab Link:* [https://learn.secbyte.org/ctf/silent-invoice-business-email-compromise](https://learn.secbyte.org/ctf/silent-invoice-business-email-compromise)  
  *Focus:* Investigating executive/vendor financial wire fraud campaigns, detecting malicious inbox forwarders and hidden reply-to rules, and auditing compromised Exchange/Microsoft 365 accounts.

### 3. Digital Evidence Handling, Case Documentation & Court Prep
* **Digital Evidence Investigation: The Courier Incident**  
  *Lab Link:* [https://learn.secbyte.org/ctf/digital-evidence-investigation-the-courier-incident](https://learn.secbyte.org/ctf/digital-evidence-investigation-the-courier-incident)  
  *Focus:* Executing digital evidence acquisition procedures, maintaining strict Chain of Custody forms, verifying SHA-256 evidence container hashes, and preserving volatile physical/virtual evidence.

<Image src="image_agent_tag_14930242868309730145" alt="Infographic detailing the 8 steps in a digital forensic chain of custody workflow" caption="Digital Forensics Chain of Custody Workflow & Evidence Handling" />

---

* **Case Documentation Fundamentals**  
  *Lab Link:* [https://learn.secbyte.org/ctf/case-documentation-fundamentals](https://learn.secbyte.org/ctf/case-documentation-fundamentals)  
  *Focus:* Authoring forensic investigation reports, structuring technical findings for executive and legal review, documenting tool verification steps, and maintaining objective audit trails.

* **Court Preparation: Evidence Timelines and Testimony**  
  *Lab Link:* [https://learn.secbyte.org/ctf/court-preparation-evidence-timelines-testimony](https://learn.secbyte.org/ctf/court-preparation-evidence-timelines-testimony)  
  *Focus:* Constructing master forensic timelines from cross-system logs (SIEM, M365, host OS), preparing expert witness disclosures, defending evidence integrity against cross-examination, and presenting findings in legal proceedings.

---

## Learning Path

### Path A: Email Security & Authentication Engineer
1. **Security & Protocol Basics:** Start with [Email Security Fundamentals](https://learn.secbyte.org/ctf/email-security-fundamentals) and [SMTP Sleuth](https://learn.secbyte.org/ctf/smtp-sleuth-mail-flow-and-misconfigurations).
2. **Authentication Defense:** Deploy domain defenses via [SPF Configuration](https://learn.secbyte.org/ctf/spf-configuration-mail-sender-trust-lab), [DKIM Validation](https://learn.secbyte.org/ctf/dkim-validation-mail-authentication-lab), and [DMARC Policy Defense](https://learn.secbyte.org/ctf/dmarc-policy-defense-lab).

### Path B: Email Forensic Analyst & BEC Responder
1. **Header Analysis & Forensics:** Investigate emails via [Email Forensics: The Inbox Incident](https://learn.secbyte.org/ctf/email-forensics-the-inbox-incident), [Email Header Forensics](https://learn.secbyte.org/ctf/email-header-forensics-lab), and [Phishing Detection: Spoofing Triage](https://learn.secbyte.org/ctf/phishing-detection-lab-inbox-forensics-and-spoofing-triage).
2. **BEC & Financial Triage:** Triage account compromise in [Silent Invoice: Business Email Compromise](https://learn.secbyte.org/ctf/silent-invoice-business-email-compromise).

### Path C: Digital Forensic Examiner & Legal Investigator
1. **Evidence Acquisition:** Preserve digital proof using [Digital Evidence Investigation: The Courier Incident](https://learn.secbyte.org/ctf/digital-evidence-investigation-the-courier-incident).
2. **Documentation & Court Testimony:** Prepare legal cases via [Case Documentation Fundamentals](https://learn.secbyte.org/ctf/case-documentation-fundamentals) and [Court Preparation: Evidence Timelines](https://learn.secbyte.org/ctf/court-preparation-evidence-timelines-testimony).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the corresponding direct link to launch the exercise environment hosted on Learn SecByte.
3. Review scenario directives, raw RFC 5322 headers, DNS TXT records, E01/DD disk images, or chain of custody logs.
4. Validate DKIM RSA signatures, trace spoofed originating IPs across `Received:` headers, audit compromised M365 inbox rules, verify forensic hashes, or construct court-admissible evidence timelines to capture flags.

---

## Target Audience

* **Email Security Engineers & Mail Gateway Administrators:** Configure SPF/DKIM/DMARC records, enforce domain alignment, audit SMTP relay configurations, and analyze delivery telemetry.
* **SOC Analysts & Incident Response Teams:** Parse email headers, investigate Business Email Compromise (BEC) wire fraud, detect domain spoofing, and purge malicious messages.
* **Digital Forensic Investigators & Law Enforcement:** Maintain chain of custody controls, acquire digital evidence containers, write forensic reports, and construct timelines for courtroom presentation.
* **Cybersecurity Students:** Acquire practical expertise in mail transfer protocols, cryptographic email verification, forensic artifact analysis, and legal evidence standards.

---

## Disclaimer

All lab links provided in this repository direct to official training environments hosted on Learn SecByte. All materials and exercises are provided strictly for educational purposes, defensive skill building, and authorized security research. Unauthorized scanning, email spoofing, or unauthorized forensic extraction against external production systems is strictly prohibited.
