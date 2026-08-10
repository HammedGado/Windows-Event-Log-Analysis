# # Findings

## Overview

This lab demonstrates how Windows Security Event Logs record administrative actions involving user account creation, security group membership changes, and successful user authentication.

---

## Key Findings

### Event ID 4720 – User Account Created

- A new local user account named **analyst1** was successfully created.

- The Security Event Log recorded the account creation along with the administrator responsible for the action.

---

### Event ID 4732 – User Added to Security Group

- The **analyst1** account was added to the **Event Log Readers** local security group.

- This granted the account permission to read Windows Event Logs without administrative privileges.

---

### Event ID 4624 – Successful Logon

- The **analyst1** account successfully logged into the local workstation.

- The event recorded an **Interactive Logon (Type 2)**, confirming the user authenticated directly at the computer.

---

## Security Impact

Windows Security Event Logs provide a reliable audit trail for:

- User account creation

- Group membership changes

- User authentication

- Administrative activity

These logs help security analysts verify administrative actions, investigate suspicious account activity, and maintain accountability within Windows environments.

---

## Conclusion

The Security Event Log accurately recorded each administrative action performed during the lab. Reviewing Event IDs 4720, 4732, and 4624 demonstrates how Windows auditing supports system monitoring and forensic investigations.