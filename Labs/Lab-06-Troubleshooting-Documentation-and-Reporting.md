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
