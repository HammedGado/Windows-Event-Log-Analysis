# Incident Report

## Incident Summary

A Windows user account named **analyst1** was created for auditing practice. The account was granted membership in the **Event Log Readers** group and successfully authenticated to the local Windows system. Windows Security Event Logs were reviewed to verify each administrative action.

---

## Timeline

| Time | Event ID | Description |

|------|----------|-------------|

| 4:10 PM | 4720 | Created local user account **analyst1** |

| 4:18 PM | 4732 | Added **analyst1** to the **Event Log Readers** group |

| 4:27 PM | 4624 | Successful interactive logon by **analyst1** |

---

## Evidence Collected

### Event ID 4720

- Created new local user account

- Account Name: **analyst1**

---

### Event ID 4732

- Added **analyst1** to the **Event Log Readers** local security group

---

### Event ID 4624

- Successful account logon

- User: **analyst1**

- Logon Type: **2 (Interactive Logon)**

---

## Analysis

The Security Event Log confirms the expected sequence of administrative actions:

1. A new local user account was created.

2. The account was granted permission to read Windows Event Logs.

3. The account successfully logged on to the workstation.

The recorded events demonstrate how Windows Security Logs provide an auditable record of user account management and authentication activity.

---

## Conclusion

All administrative actions completed during the lab were successfully recorded in the Windows Security Event Log. The collected evidence confirms account creation, group membership assignment, and successful user authentication.

