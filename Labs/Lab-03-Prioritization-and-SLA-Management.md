
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

# Lab 03 — Part 2: SLA Management

## Objective
Inspect ServiceNow Service Level Agreement (SLA) definitions, review SLA condition rules and timer configurations, and verify SLA tracking on a simulated incident.

## Environment
- Platform: ServiceNow Personal Developer Instance (PDI)
- Module: SLA Definitions
- Module: SLA Condition Rules
- Module: SLA Timer Configuration
- Related list: Task SLAs

## Security Focus
- Understand how SLA configurations support incident response and resolution targets.
- Review existing configuration without modifying system-level settings.
- Observe how ServiceNow tracks SLA progress, elapsed time, and cancellation states.

## Tasks Completed

### 1. Reviewed an Existing SLA Definition
Opened the existing **Priority 1 resolution (1 Hour)** SLA definition and reviewed its configuration.

Observed settings:
- Duration: 1 hour
- Schedule source: No schedule
- Active: Enabled
- Start condition: Condition builder available
- Stop condition: Blank
- Pause condition: Blank

No changes were made to the existing SLA definition.

### 2. Inspected SLA Condition Rules
Reviewed the available records in the SLA Condition Rules module.

| Rule | Class name | Review result |
|---|---|---|
| Default | SLA Condition Base | Active; Application and Class name fields present |
| Issue auto resolution | AutoResolutionSLACondition | Inspected; Application and Class name fields present |
| simple | SLAConditionSimple | Inspected; Application and Class name fields present |

The existing rules were inspected without modification.

### 3. Reviewed SLA Timer Configuration
Opened an existing timer configuration record.

| Field | Observed value |
|---|---|
| Name | Do not show sla timer |
| SLA Timer Source | None |
| Show cancelled | False |
| Show completed | False |

No timer configuration changes were made.

### 4. Verified Task SLA Records on a Training Incident
Opened the simulated incident:

**Lab 03 - Multiple employees unable to access a business-critical application**

Located the Task SLAs related list and confirmed that it contained three records:
- Priority 1 resolution
- Priority 2 resolution
- Priority 3 resolution

The related list exposed SLA definition, type, target, stage, business time remaining, business elapsed time, elapsed percentage, start time, and stop time.

### 5. Recorded SLA Tracking Results

| SLA definition | Type | Target | Stage | Business time left | Business elapsed time | Elapsed percentage |
|---|---|---|---|---|---|---|
| Priority 1 resolution | SLA | Resolution | In Progress | 20 minutes | 39 minutes | 66.39% |
| Priority 2 resolution | SLA | Resolution | Cancelled | 7 hr 52 min | 7 minutes | 1.62% |
| Priority 3 resolution | SLA | Resolution | Cancelled | 23 hr 55 min | 4 minutes | 0.32% |

These values reflect the records observed during the lab. The Priority 2 and Priority 3 records were in the Cancelled stage, while Priority 1 was In Progress.

The precise reasons for cancellation were not established during this exercise.

## Security Analysis
SLA tracking provides visibility into how much time remains before a resolution target is reached and how much time has elapsed. This can help support teams monitor service commitments and prioritize incident handling.

The Task SLAs related list also demonstrates that multiple SLA records can be associated with a single incident. A cancelled SLA record should not automatically be interpreted as a resolved incident; the incident's state and the SLA's lifecycle are separate details that should be reviewed together.

Inspecting the existing rules and timer configuration without modifying them reduced the risk of unintentionally affecting other records or platform behavior.

## Key Takeaways
- ServiceNow provides configurable SLA definitions with duration and lifecycle conditions.
- SLA condition rules and timer configurations are separate configuration areas.
- Task SLAs can be reviewed directly from an incident record.
- SLA records expose timing information such as remaining business time, elapsed business time, and elapsed percentage.
- SLA records can have different lifecycle stages, including In Progress and Cancelled.
- Existing platform configurations should be inspected carefully before making changes.

## Skills Demonstrated
- ServiceNow ITSM navigation
- SLA definition inspection
- SLA condition rule review
- SLA timer configuration review
- Incident SLA tracking and validation
- SLA lifecycle and timing analysis
- Configuration review without unnecessary system changes
- Technical documentation and evidence collection

## Evidence Screenshots

<img width="1512" height="750" alt="Screenshot 2026-10-21 at 1 13 49 PM" src="https://github.com/user-attachments/assets/d36fc3c2-b53d-497a-bb14-780db1bbbd4f" />

<img width="1512" height="696" alt="Screenshot 2026-10-21 at 1 41 18 PM" src="https://github.com/user-attachments/assets/b9cbc488-3f1c-4250-9a34-3575932f1323" />


## Outcome
Successfully reviewed existing SLA configurations and verified three priority-based Task SLA records on a simulated incident. No existing SLA definitions, condition rules, timer configurations, or Task SLA records were modified during this exercise.
