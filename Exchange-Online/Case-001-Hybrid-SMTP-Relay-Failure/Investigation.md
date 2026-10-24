# Investigation Process

## Objective

Determine why OTP emails stopped delivering after mailbox migration from Exchange Server 2016 Hybrid to Exchange Online.

---

## Initial Assessment

The customer reported:

- OTP emails were previously delivered successfully.
- Issue started after mailbox migration.
- Application functionality depended on successful email delivery.

---

## Investigation Steps

### 1. Message Trace

Performed Exchange Online message tracing.

Findings:

- Messages were not consistently reaching Exchange Online.

---

### 2. Connector Review

Validated:

- Send Connectors
- Receive Connectors
- Hybrid Configuration

Findings:

- Existing configuration was designed for on-premises mail delivery.

---

### 3. SMTP Relay Testing

Reviewed:

- Authentication requirements
- Relay permissions
- TLS configuration
- Smart host settings

---

### 4. Mail Flow Validation

Conducted end-to-end testing from application server to mailbox.

---

## Conclusion

The SMTP relay configuration required adjustment following mailbox migration to Exchange Online.
