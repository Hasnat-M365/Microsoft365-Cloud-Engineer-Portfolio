# Case 001 - Hybrid SMTP Relay Failure

## Business Scenario

A customer migrated mailboxes from Exchange Server 2016 Hybrid to Exchange Online.

Following the migration, an on-premises application responsible for sending One-Time Password (OTP) emails stopped delivering messages to Microsoft 365 mailboxes.

---

## Technologies Used

- Exchange Server 2016
- Exchange Online
- Exchange Hybrid Configuration Wizard (HCW)
- SMTP Relay
- Message Trace
- Exchange Admin Center
- PowerShell

---

## Symptoms

- OTP emails not received
- Application email delivery failures
- Business authentication process impacted
- Users unable to receive verification codes

---

## Investigation Process

### Step 1 - Validate Mail Flow

Performed message tracing to determine whether messages were reaching Exchange Online.

### Step 2 - Review Exchange Hybrid Configuration

Reviewed Hybrid Configuration Wizard settings and mail flow configuration.

### Step 3 - SMTP Relay Validation

Checked:

- Receive Connectors
- Send Connectors
- Relay Permissions
- Anonymous Authentication
- TLS Configuration

### Step 4 - Exchange Online Review

Verified:

- Accepted Domains
- Connectors
- Mail Flow Rules
- Message Tracking

---

## Root Cause

The application relay configuration was designed for legacy on-premises mailbox delivery.

Following mailbox migration, relay traffic was no longer aligned with Exchange Online mail routing requirements.

---

## Resolution

- Updated SMTP relay configuration
- Validated Exchange Online connectors
- Performed end-to-end testing
- Confirmed successful mail delivery

---

## Outcome

✅ OTP emails successfully delivered

✅ Mail flow restored

✅ Application functionality restored

✅ Business operations normalized

---

## Skills Demonstrated

- Exchange Online Administration
- Exchange Hybrid Administration
- SMTP Troubleshooting
- Mail Flow Analysis
- Root Cause Analysis
- Microsoft 365 Support Engineering
