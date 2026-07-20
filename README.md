# Phishing-Email-Investigation

A cybersecurity case study analyzing a phishing email through header analysis, social engineering assessment, and threat investigation.

## Phishing Email Investigation and Analysis

### Project Overview
This project documents a cybersecurity investigation of a suspected phishing email. The investigation focuses on identifying social engineering techniques, analyzing email metadata, reviewing authentication results, identifying indicators of compromise (IOCs), and documenting security recommendations.

All sensitive information has been anonymized or removed.

### Investigation Objectives
The objectives of this investigation were:
- Analyze a suspicious phishing email.
- Examine email header information.
- Review SPF, DKIM, and DMARC authentication results.
- Identify phishing indicators and social engineering techniques.
- Document findings using a cybersecurity incident report format.
- Provide mitigation recommendations.

### Investigation Process
The investigation followed these steps:
1. Email collection and preservation.
2. Header and metadata analysis.
3. Authentication review.
4. Content and social engineering analysis.
5. Indicator of Compromise (IOC) identification.
6. Risk assessment.
7. Security recommendations.

### Key Findings

The investigated email contained multiple phishing indicators:
- Unexpected financial reward claim, framed as a large sum of "unclaimed funds" being released.
- Impersonation of a real Swiss financial institution and a named individual presented as its CEO/Chairman (identity redacted for privacy).
- Sender display name closely mirrored the recipient's own name — a technique likely intended to increase perceived familiarity and trust.
- Fabricated bureaucratic obstacles (administrative restrictions, blacklist claims, processing fees) used to add false legitimacy to the review process.
- Name-dropping of unrelated, legitimate financial institutions (e.g. IMF, World Bank, and several major commercial banks) with no actual connection to the email, used as a credibility-building tactic.
- Request for sensitive personal information, including full legal name, residential address, phone number, and a copy of a government-issued ID — a significant escalation beyond typical credential phishing, indicating potential identity theft intent.
- Urgency-based social engineering, prompting immediate reply to complete a "final identity cross-check."
- Sender identity inconsistencies and a Reply-To address mismatch inconsistent with the claimed sender.

### Technical Analysis
The email authentication results were:

| Security Control | Result |
|---|---|
| SPF | PASS |
| DKIM | PASS |
| DMARC | PASS |

Authentication confirmed that the email originated from an authenticated domain, but it did not confirm that the message content was legitimate. This is a key distinction: passing SPF/DKIM/DMARC verifies the sending domain's authorization, not the trustworthiness of the message itself.

### Repository Structure


### Skills Demonstrated
- Phishing Analysis
- Email Header Analysis
- Social Engineering Analysis
- Threat Investigation
- IOC Identification
- Risk Assessment
- Cybersecurity Documentation

### Disclaimer
This project was created for educational and defensive cybersecurity purposes. All sensitive information, including the identities of any real individuals or accounts referenced in the original email has been anonymized. Named financial institutions are referenced factually, as they were impersonated or name-dropped by the sender and are not implicated in the fraudulent activity. No malicious links or attachments were executed during this investigation.
