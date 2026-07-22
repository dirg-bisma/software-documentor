# Document Control
[Standard Document Control Table]

---

# 1. Module Overview
This FSD covers the **Reservation Module** for the centralized platform.

# 2. Screen Behavior
## 2.1 Create Reservation Screen (SCR-RES-01)
- **Trigger:** User clicks "New Reservation" on the dashboard.
- **Fields:**
  | Field | Type | Mandatory? | Validation Rule |
  | :--- | :--- | :--- | :--- |
  | Property ID | UUID | Yes | Must be inferred from user's active session context |
  | Check-in Date | Date | Yes | Must be >= Today |
  | Check-out Date | Date | Yes | Must be > Check-in Date |
  | Guest Name | String | Yes | Max 100 characters |
- **Actions/Buttons:**
  - **Check Availability:** Calls `API-RES-01`. If available, enables "Book" button.

# 3. Detailed Validations & Error Handling
- **ERR-RES-001:** If Check-out Date is before Check-in Date, display: "Check-out date must be after check-in date."

# 4. APIs & Integrations
- **API-RES-01 [Check Availability]:** `GET /api/v1/inventory/availability?propertyId={id}&start={date}&end={date}`

# 5. Workflow Behavior
- **State Transition:** When a reservation is successfully created, its state is set to `CONFIRMED`.
