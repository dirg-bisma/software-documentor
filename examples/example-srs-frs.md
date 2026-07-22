# Document Control
[Standard Document Control Table]

---

# 1. Introduction
This document specifies the software requirements for the Centralized Hotel Management Platform MVP.

# 2. User Roles & Permissions
- **Corporate Admin:** Can view all properties and manage global settings.
- **Property Manager:** Can view and manage data only for their assigned property.
- **Front Desk:** Can manage reservations for their assigned property.

# 3. Functional Requirements
- **FR-001 [Property Context Switch]:** The system shall allow a Corporate Admin to select an active property from a dropdown menu. All subsequent data displayed shall be filtered to the selected property.
  - **Traces to:** FEAT-001
  - **Acceptance Criteria:** When "Hotel A" is selected, the dashboard only shows metrics for Hotel A.

- **FR-002 [Create Reservation]:** The system shall allow a Front Desk user to create a reservation by selecting dates, room type, and guest details.
  - **Traces to:** FEAT-002

# 4. Non-Functional Requirements
- **NFR-001 [Performance]:** The system shall load the consolidated corporate dashboard within 3 seconds under normal load.
- **NFR-002 [Data Isolation]:** The system shall guarantee that a Property Manager for Hotel A cannot query or access data for Hotel B via the API or UI.

# 5. Business Rules
- **RULE-001:** A reservation cannot be created in the past.

# 6. Assumptions & Open Questions
- [TBD] The expected normal load is [TBD] concurrent users. (Pending load testing analysis).
