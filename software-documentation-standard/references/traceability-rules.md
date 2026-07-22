# Traceability Rules

Every major requirement must be traceable to ensure that what is built is exactly what the business requested, no more and no less.

## The Traceability Chain
The standard progression is:
`Business Requirement (BRD) -> Product Feature (PRD) -> Software Requirement (SRS) -> Functional Specification (FSD) -> Technical Design (TD) -> Test Case (TC)`

### Example Trace:
1. **BR-001**: "Increase booking conversions by 20% by offering a seamless mobile booking experience."
2. **FEAT-001**: "Mobile-Responsive Booking Engine." (Maps to BR-001)
3. **FR-001**: "The system shall allow guests to select room types on a mobile view." (Maps to FEAT-001)
4. **FSD-001**: "Mobile Room Selection Screen and API Integration." (Maps to FR-001)
5. **TD-001**: "GraphQL query for room availability optimized for mobile payload." (Maps to FSD-001)
6. **TC-001**: "Verify room selection works on 320px viewport." (Maps to FR-001, FSD-001)

## Identifying Orphans
An AI must identify and flag **orphan requirements**:
- A requirement with no business justification.
- A feature with no originating business requirement.
- A functional requirement with no product feature mapping.
- A technical decision with no requirement or rationale.
- A test case with no requirement coverage.
