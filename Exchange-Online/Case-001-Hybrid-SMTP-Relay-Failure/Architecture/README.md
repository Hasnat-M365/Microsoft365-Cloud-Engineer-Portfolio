# Mail Flow Architecture

## Original Environment

Application Server
↓
Exchange Server 2016 Relay
↓
On-Premises Mailbox

---

## After Mailbox Migration

Application Server
↓
Exchange Server 2016 Relay
↓
Exchange Online Connector
↓
Microsoft 365 Mailbox

---

## Objective

Ensure SMTP relay traffic continues to reach Microsoft 365 mailboxes after mailbox migration from Exchange Hybrid to Exchange Online.

## Components

### Application Server

Generates OTP and business notification emails.

### Exchange Server 2016 Relay

Processes and relays SMTP messages.

### Exchange Online

Receives and delivers messages to cloud mailboxes.

### Microsoft 365 Mailbox

Final destination for application-generated emails.
