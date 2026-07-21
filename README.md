# Enterprise IT Support & Cloud Identity Management Sandbox

Full-lifecycle IT Service Management (ITSM) sandbox integrating Jira Service Management with Microsoft Entra ID to simulate enterprise Tier 1/2 IT infrastructure support.

---

## 🛠️ Environment Setup
* **ITSM Platform:** Jira Service Management (Cloud)
* **Identity Provider:** Microsoft Entra ID (Azure Portal)
* **Standards Followed:** ITIL Framework (Incident, Service Request, & Problem Management)

---

## Ticket Walkthroughs

### Ticket 1: VPN Connection Timeout (Alex Wilber)
* **Issue Type:** `[System] Incident`
* **Status:** `Resolved / Done`
* **Root Cause Analysis:** User account was missing the required remote access permissions in the cloud directory.
* **Resolution Steps:**
  1. Triaged and assigned the incoming connection timeout incident within Jira Service Management.
  2. Navigated to Microsoft Entra ID and located the user profile for Alex Wilber.
  3. Modified group memberships to assign the user to the `sg-Remote-VPN-Users` security group.
  4. Provided a professional resolution summary directly to the client via the customer portal link.
  5. Satisfied project data integrity constraints by linking the individual incident to the global `[MASTER] Remote Access & VPN Connection Issues` tracking ticket.

### Ticket 2: Urgent Account Deprovisioning & Offboarding (John Doe)
* **Issue Type:** `[System] Service Request`
* **Status:** `Resolved / Done`
* **Root Cause Analysis:** Urgent HR offboarding request requiring immediate revocation of identity credentials, active session termination, and privilege removal.
* **Resolution Steps:**
  1. Triaged and validated the incoming urgent offboarding request within Jira Service Management.
  2. Located John Doe in Microsoft Entra ID and toggled **Account Enabled** to **No** to block future authentication attempts.
  3. Executed a **Password Reset** to scramble account credentials and prevent unauthorized re-entry.
  4. Triggered **Revoke Sessions** token invalidation to immediately terminate all active browser and application sessions.
  5. Stripped all assigned Security and Department group memberships (`sg-Remote-VPN-Users`, `dept-sales`) to eliminate residual privileges.
  6. Documented all technical remediation steps in the ticket resolution log and linked the request to the `[MASTER] Security Deprovisioning & User Lifecycle Tracking` parent ticket for ITIL audit compliance.
