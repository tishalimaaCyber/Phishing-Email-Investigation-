# Indicators of Compromise (IOCs)

## Phishing Email Investigation

### Email Indicators

| Indicator | Observation |
|---|---|
| Subject | Important Notice: Action Required to Reclaim Your Funds |
| Threat Type | Phishing / Advance-Fee Fraud |
| Risk Level | High |
| Social Engineering Method | Financial reward, urgency, authority impersonation |
| Sensitive Data Requested | Full name, address, phone number, occupation, government ID document |

### Sender Indicators

| Indicator | Observation |
|---|---|
| Display Name | Named individual, presented as CEO/Chairman of an impersonated institution (redacted for privacy) |
| Claimed Institution | AEK Bank 1826 (real institution, impersonated) |
| Sending Domain | nifty.com |
| Reply-To Mismatch | Yes |
| Sender Identity Concern | Display name does not match sending domain; display name closely mirrored the recipient's own name |

### Authentication Results

| Security Control | Result |
|---|---|
| SPF | PASS |
| DKIM | PASS |
| DMARC | PASS |

Note: Authentication confirms the sending domain but does not prove the email content is legitimate.

### Referenced Institutions
The email referenced several unrelated, legitimate institutions to build false credibility. None were actually connected to the scam:
- International Monetary Fund (IMF)
- World Bank
- Bank of America
- Royal Bank of Canada
- HDFC Bank

### Key Findings
- Unexpected financial reward claim
- Impersonation of a real financial institution (AEK Bank 1826) and a named individual in an executive role (redacted for privacy)
- Sender display name closely mirrored the recipient's own name
- Request for government identification and other sensitive personal data
- Urgent response request
- Name-dropping of trusted financial organizations unrelated to the scam
- Sender identity inconsistencies and Reply-To mismatch
