
# Lab 03 — Part 1: Incident Impact and Urgency

## Objective
Understand how ServiceNow uses incident impact and urgency to calculate priority. Test multiple combinations of impact and urgency, observe the resulting priority values, and document the relationship between incident severity and operational response.

## Environment
- **Platform:** ServiceNow Personal Developer Instance (PDI)
- **Interface:** Service Desk — Incidents
- **Lab:** Lab 03 — Prioritization and SLA Management
- **Test Scenario:** Simulated business-critical application outage
- **Incident:** Lab 03 test incident (record number to be added if needed)

## Security Focus
Accurate incident prioritization helps IT support teams determine which issues require the fastest response. Incorrect priority assignments can delay resolution of critical incidents or cause support resources to be allocated inefficiently.

This exercise used a simulated incident scenario. No actual outage, troubleshooting, or production-system changes occurred.

---

## Tasks Completed

### 1. Created a Test Incident
Created a ServiceNow incident using the following scenario:

**Short description:** `Lab 03 - Multiple employees unable to access a business-critical application`

**Description:** Multiple employees report that they cannot access a business-critical application. This is a simulated training scenario; no actual outage or troubleshooting occurred.

The incident was used to test how changing impact and urgency affected the calculated priority.

### 2. Tested Medium Impact and Medium Urgency
Configured the incident with:

- **Impact:** `2 - Medium`
- **Urgency:** `2 - Medium`
- **Priority:** `3 - Moderate`

The saved incident displayed a priority of 3 - Moderate.

### 3. Increased Urgency to High
Changed the incident's urgency while keeping impact unchanged.

- **Impact:** `2 - Medium`
- **Urgency:** `1 - High`
- **Priority:** `2 - High`

A work note was added to explain the change:

`Lab 03 training exercise: Increased urgency from Medium to High to observe how ServiceNow recalculates incident priority. This is a simulated scenario; no actual outage or troubleshooting occurred.`

After saving the incident, the Priority field displayed 2 - High.

### 4. Increased Impact to High
Changed impact to High while keeping urgency at High.

- **Impact:** `1 - High`
- **Urgency:** `1 - High`
- **Priority:** `1 - Critical`

A work note was added to explain the change:

`Lab 03 training exercise: Increased impact to High to observe the priority calculation. This is a simulated scenario.`

After saving the incident, the Priority field displayed 1 - Critical.

---

## Priority Assessment Results

| Test | Impact | Urgency | Observed Priority |
|---|---|---|---|
| 1 | 2 - Medium | 2 - Medium | 3 - Moderate |
| 2 | 2 - Medium | 1 - High | 2 - High |
| 3 | 1 - High | 1 - High | 1 - Critical |

### Analysis
The tests demonstrated that ServiceNow recalculated the incident's priority when impact and urgency were changed.

- With medium impact and medium urgency, the incident received priority 3 - Moderate.
- Increasing urgency to High while keeping impact at Medium changed the priority to 2 - High.
- Increasing impact to High while keeping urgency at High changed the priority to 1 - Critical.

These results are consistent with the priority behavior observed in this ServiceNow instance. Other instances may use different priority lookup rules or customized configurations.

---

## Security Analysis
Incident prioritization supports effective incident management by helping support teams distinguish routine issues from incidents that may require urgent attention.

High-impact incidents may affect multiple employees or important business services. High urgency indicates that action is needed quickly. Considering both values helps support teams prioritize incidents more consistently.

The simulated scenario and explanatory work notes also demonstrate the importance of maintaining a clear audit trail when changing incident information during training.

## Key Takeaways
- Impact represents the extent of the business or operational effect.
- Urgency represents how quickly the issue requires attention.
- Priority is calculated using the platform's configured priority rules.
- Higher impact and urgency can result in a more critical priority.
- Work notes can document the reason for changes and support traceability.
- Priority behavior should be verified in the actual ServiceNow instance rather than assumed.

## Skills Demonstrated
- ServiceNow incident management
- Incident creation and modification
- Impact and urgency assessment
- Priority verification
- Work note documentation
- Basic ITSM prioritization
- Security-focused operational documentation

---

## Evidence Screenshots

<img width="1512" height="750" alt="Screenshot 2026-10-21 at 12 56 32 PM" src="https://github.com/user-attachments/assets/2b6b6ec3-fdfb-49c2-a6a5-f245d8259771" />

<img width="1512" height="750" alt="Screenshot 2026-10-21 at 1 01 21 PM" src="https://github.com/user-attachments/assets/a46d50b3-0162-499c-8ded-ce1e0f437832" />

<img width="1512" height="750" alt="Screenshot 2026-10-21 at 1 03 54 PM" src="https://github.com/user-attachments/assets/4f24a17a-144d-43e8-82b9-0916aebbaa94" />

---



