# Indicators of Compromise (IOCs)

## Phishing Email Investigation

### Email Indicators

| Indicator | Observation |
|---|---|
| Subject | Important Notice: Action Required to Reclaim Your Funds |
| Threat Type | Phishing / Advance-Fee Fraud |
| Risk Level | High |
| Social Engineering Method | Financial reward, urgency, authority impersonation |
| Sensitive Data Requested | Full name, address, phone number, occupation, ID document |


## Sender Indicators

| Indicator | Observation |
|---|---|
| Display Name  | "Mr. Roger Brechbühler" (claimed identity) |
| Sending Domain | nifty.com |
| Reply-To Mismatch | Yes |
| Sender Identity Concern | Display name does not match email address |


## Authentication Results

| Security Control | Result |
|---|---|
| SPF | PASS |
| DKIM | PASS |
| DMARC | PASS |

Note: Authentication confirms the sending domain but does not prove the email content is legitimate.


## Key Findings

- Unexpected financial reward claim
- Request for government identification
- Urgent response request
- Use of trusted financial organization names
- Sender identity inconsistencies
