# Lab 06 — Part 1: Troubleshooting Documentation

## Objective
Practice documenting an IT troubleshooting investigation in ServiceNow, recording diagnostic plans and findings in work notes, and routing an incident to the appropriate support group.

## Incident Details
- Incident Number: INC0009009
- Short Description: Unable to access shared folder
- Caller: David Miller
- Initial State: New
- Initial Priority: 4 - Low
- Initial Impact: 3 - Low
- Initial Urgency: 2 - Medium
- Assignment Group: IT Support - Lab Team

## Tasks Completed

### 1. Inspected the Existing Incident
- Opened incident INC0009009.
- Reviewed the short description, caller, priority, impact, and urgency.
- Confirmed the incident was in the New state.
- Confirmed the Assigned to and Assignment group fields were initially empty.
- Checked the activity history and found no prior work notes.

### 2. Documented the Initial Investigation
Recorded a work note identifying the reported shared-folder access issue, the absence of previous troubleshooting notes, and the next diagnostic steps:
- Confirm the shared-folder path.
- Determine whether one user or multiple users are affected.
- Review access permissions.
- Check network connectivity.

### 3. Assigned the Incident to a Support Group
- Set the Assignment group to IT Support - Lab Team.
- Left Assigned to empty.
- Saved and reopened the incident.
- Verified the assignment group was saved and the incident remained New.

### 4. Documented the Troubleshooting Plan
Added a work note identifying the diagnostic checks that would be needed before determining the cause of the access issue.
- Verified the work note was saved.
- Did not claim that the diagnostic checks had already been performed.

### 5. Documented the Investigation Status
Added a final work note explaining that the available information did not establish a confirmed root cause.
- Identified permissions, network connectivity, the shared-folder path, and file-server availability as possible areas for further investigation.
- Confirmed that additional technical validation was required before documenting a resolution.
- Reopened the incident and verified all three work notes were present.

## Troubleshooting Findings
- The incident reported an inability to access a shared folder.
- No previous troubleshooting notes were present at the start of the exercise.
- The incident was routed to IT Support - Lab Team.
- The investigation plan and current findings were documented in ServiceNow work notes.
- No technical root cause was confirmed during this exercise.
- No resolution was applied or verified.
- The incident remained in the New state.

## Security Analysis
- Work notes provide an auditable record of investigation activity.
- Assignment groups support accountability and appropriate incident routing.
- Troubleshooting documentation should distinguish planned checks from tests that have actually been performed.
- Potential causes should not be reported as confirmed findings without supporting evidence.
- An incident should not be marked resolved until an appropriate fix and outcome have been verified.

## Key Takeaways
- Reviewed an existing ServiceNow incident.
- Recorded structured troubleshooting notes.
- Routed an incident to a support group.
- Verified saved assignment and work-note history.
- Practiced evidence-based troubleshooting documentation without inventing a root cause or resolution.

## Evidence
<img width="1512" height="756" alt="Screenshot 2026-10-26 at 10 07 52 AM" src="https://github.com/user-attachments/assets/a946a296-c469-4da9-925e-56b115fbc690" />
<img width="1512" height="489" alt="Screenshot 2026-10-26 at 10 11 22 AM" src="https://github.com/user-attachments/assets/9310d908-dd6d-457e-8c82-35643911c8a6" />
<img width="1512" height="758" alt="Screenshot 2026-10-26 at 10 23 45 AM" src="https://github.com/user-attachments/assets/a00ba6c6-641e-4dc2-9f0d-61b0f855399d" />


## Result
Part 1 is complete. The incident was reviewed, assigned to IT Support - Lab Team, and updated with three verified troubleshooting work notes. The investigation remains open for further technical validation because no root cause or resolution was confirmed.

# Lab 06 — Part 2: Incident Reporting

## Objective
Create and validate a ServiceNow incident report to demonstrate incident reporting and data organization.

## Report Configuration
- **Report name:** ITSM - Homelab - Incident Report
- **Source table:** Incident [incident]
- **Report type:** List
- **Group by:** Priority
- **Displayed columns:**
  - Number
  - Short description
  - Priority
  - State
  - Assignment group
  - Assigned to
  - Created
- **Chart title:** Incident Distribution by Priority

## Tasks Completed
- Created a report using the Incident table.
- Selected incident fields to display in the report.
- Grouped incident records by priority.
- Ran the report and reviewed the resulting incident groups.
- Saved the report.
- Returned to the reports list and confirmed the saved report was visible.

## Results and Validation
The report displayed 69 incident records across five priority groups:

| Priority | Incident Count |
|---|---:|
| 1 - Critical | 28 |
| 2 - High | 4 |
| 3 - Moderate | 12 |
| 4 - Low | 6 |
| 5 - Planning | 19 |
| **Total** | **69** |

The report was saved and was visible when returning to the reports list.

These counts represent the records present in the instance when the report was run. They are not limited to incidents created during this homelab.

## Security and Operational Analysis
Incident reports help support teams:
- Identify the distribution of incident priorities.
- Review ticket ownership and assignment.
- Monitor incident states and descriptions.
- Organize operational data for review and decision-making.

Report results depend on the available records and the user's access permissions. Priority counts alone do not establish incident resolution performance or SLA compliance.

## Key Takeaways
- ServiceNow reports can summarize and organize incident records.
- Grouping by priority makes the distribution of incident records easier to review.
- Saving a report allows it to be accessed again.
- Report data should be interpreted in the context of the underlying records.

## Skills Demonstrated
- ServiceNow report creation
- Incident table selection
- Report column configuration
- Grouping and summarizing records
- Report execution and validation
- ITSM operational reporting

## Evidence
<img width="1512" height="758" alt="Screenshot 2026-10-26 at 10 44 23 AM" src="https://github.com/user-attachments/assets/9c2d600d-982e-42dc-93f2-67387930e246" />
<img width="1512" height="129" alt="Screenshot 2026-10-26 at 10 48 06 AM" src="https://github.com/user-attachments/assets/2582981f-c40c-453d-a1ec-c07e8225e5b7" />

# Lab 06 — Part 3: Validation and Documentation

## Objective
Validate the troubleshooting documentation and incident report created during Lab 06, and prepare the results for a technical portfolio.

## Tasks Completed

### Troubleshooting Documentation Validation
- Reopened incident INC0009009, "Unable to access shared folder."
- Verified the assignment group was IT Support - Lab Team.
- Verified the three troubleshooting work notes were present.
- Confirmed the incident remained in the New state.

### Incident Reporting Validation
- Confirmed the saved report, "ITSM - Homelab - Incident Report," was visible in ServiceNow.
- Configured the report using the Incident [incident] table.
- Displayed incident details in a list.
- Grouped records by Priority.
- Ran the report and reviewed the results.

## Results
The incident report displayed 69 records grouped as follows:

| Priority | Incident Count |
|---|---:|
| 1 - Critical | 28 |
| 2 - High | 4 |
| 3 - Moderate | 12 |
| 4 - Low | 6 |
| 5 - Planning | 19 |
| **Total** | **69** |

The report was saved and its presence was verified. The counts reflect the records available in the instance at the time of reporting.

## Validation Notes
- Troubleshooting notes document the investigation plan, not a confirmed technical root cause.
- No fix was confirmed for INC0009009 during this lab.
- The incident was not closed as part of the validation process.
- The report summarizes incident records but does not independently establish SLA compliance or resolution effectiveness.

## Key Takeaways
- Clear work notes preserve investigation context and support handoffs between technicians.
- Assignment groups help identify the team responsible for an incident.
- Saved reports provide a repeatable way to review and organize incident data.
- Validation helps ensure that documentation reflects the actual system state.

## Skills Demonstrated
- Incident record validation
- Troubleshooting documentation review
- Work note verification
- Assignment group verification
- ServiceNow report validation
- ITSM documentation and portfolio preparation


# Lab 06 — Troubleshooting Documentation and Reporting

## Overview
This lab focused on documenting incident troubleshooting activity, creating an incident report in ServiceNow, and validating that the records and report were saved correctly.

## Objectives
- Document troubleshooting steps using incident work notes.
- Assign an incident to the appropriate support group.
- Create and save an incident report.
- Group incident records by priority.
- Validate the results and prepare evidence for a technical portfolio.

## Lab Parts Completed

### Part 1 — Troubleshooting Documentation
- Worked with incident `INC0009009`: "Unable to access shared folder."
- Assigned the incident to `IT Support - Lab Team`.
- Added three work notes documenting the initial investigation, troubleshooting plan, and review status.
- Verified the assignment group and work notes.
- Kept the incident in the New state because no root cause or resolution had been confirmed.

### Part 2 — Incident Reporting
- Created the report `ITSM - Homelab - Incident Report`.
- Used the `Incident [incident]` table as the data source.
- Configured a list report with incident fields, including number, short description, priority, state, assignment group, assigned to, and created date.
- Grouped records by Priority.
- Ran and saved the report, then confirmed it was visible in ServiceNow.

#### Report Results
The report displayed 69 incident records across five priority groups:

| Priority | Incident Count |
|---|---:|
| 1 - Critical | 28 |
| 2 - High | 4 |
| 3 - Moderate | 12 |
| 4 - Low | 6 |
| 5 - Planning | 19 |
| **Total** | **69** |

These counts reflect the records available in the instance when the report was run, not only incidents created for this lab.

### Part 3 — Validation and Documentation
- Reopened incident `INC0009009`.
- Verified the assignment group and troubleshooting work notes.
- Confirmed the incident remained in the New state.
- Confirmed the saved incident report was visible.
- Prepared documentation and evidence references for the portfolio.

## Security and Operational Analysis
Accurate incident documentation helps preserve investigation history, improve technician handoffs, and support accountability. Assignment groups clarify team responsibility, while reports help support teams organize and review incident records.

Reports must be interpreted in context. Priority counts alone do not establish resolution effectiveness, root cause, or SLA compliance. Troubleshooting notes should distinguish confirmed findings from planned investigative actions.

## Key Takeaways
- Work notes preserve troubleshooting context and the actions planned or performed.
- Assignment groups identify the team responsible for handling an incident.
- ServiceNow reports can organize incident records by priority.
- Saved reports can be reopened for later review.
- Validation ensures documentation reflects the actual state of the system.
- Technical portfolios should clearly distinguish completed tests from unverified results.

## Skills Demonstrated
- ServiceNow incident management
- Troubleshooting documentation
- Incident assignment and ownership
- Work note validation
- Report creation and configuration
- Data grouping and review
- Technical documentation and evidence management

## Conclusion
This lab demonstrated how to document an incident investigation, organize incident ownership, generate a priority-based incident report, and validate saved ServiceNow records. The troubleshooting incident remained open because a technical root cause and resolution were not established during the exercise.
