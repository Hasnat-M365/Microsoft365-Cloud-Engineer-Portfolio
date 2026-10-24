# Root Cause Analysis

## Problem

OTP emails stopped reaching Microsoft 365 mailboxes after migration.

---

## Technical Findings

The legacy relay configuration was optimized for Exchange Server mailbox delivery.

Mailbox migration changed the mail flow path and introduced Exchange Online routing requirements.

---

## Root Cause

Relay traffic was not aligned with the updated Exchange Online mail flow design.

As a result, application-generated SMTP traffic did not follow a valid delivery path.

---

## Corrective Actions

- Validated connector configuration
- Updated SMTP relay settings
- Confirmed mail routing
- Performed validation testing

---

## Result

Mail flow restored successfully.
