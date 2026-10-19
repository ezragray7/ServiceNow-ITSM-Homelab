
# Lab 01: Incident Management

## Objective

Create and document a ServiceNow incident to simulate a common IT help desk scenario. Practice basic incident creation, caller selection, customer-visible communication, and incident record verification.

## Environment

- **Platform:** ServiceNow Personal Developer Instance (PDI)
- **Interface:** Incidents – Self Service
- **Operating System:** macOS
- **Documentation:** GitHub Markdown
- **Incident Number:** INC0010002

## Scenario

An employee reports that their work computer cannot connect to the internet, preventing access to online work resources. An incident is created to document the reported issue and begin the incident management process.

## Tasks Completed

- [x] Accessed the ServiceNow incident interface.
- [x] Created a test incident.
- [x] Selected a sample caller from the available caller records.
- [x] Added a short description of the reported technical issue.
- [x] Added a customer-visible comment describing the problem.
- [x] Submitted the incident successfully.
- [x] Located the incident in the incident list.
- [x] Opened the saved incident details.
- [x] Verified the incident number and current state.
- [x] Observed the displayed urgency, impact, and priority values.
- [ ] Practice updating the incident during troubleshooting.
- [ ] Resolve the incident after documenting a simulated resolution.
- [ ] Verify the incident's final state.

## Procedures Used

1. Opened the Incidents – Self Service view in ServiceNow.
2. Selected the option to create a new incident.
3. Selected a sample caller from the available caller records.
4. Entered the following short description:

   `Employee unable to connect to the internet`

5. Entered a description explaining that the employee could not access online work resources.
6. Added a customer-visible comment:

   `I am unable to connect to the internet on my work computer. I cannot access online work resources. Please investigate the issue and let me know when service is restored.`

7. Submitted the incident.
8. Located the newly created incident in the incident list.
9. Opened the saved record and verified incident number `INC0010002`.
10. Reviewed the incident fields and activity history.

## Incident Details

| Field | Observed Value |
|---|---|
| Incident Number | INC0010002 |
| Caller | Abel Tuter |
| Short Description | Employee unable to connect to the internet |
| State | New |
| Impact | 3 - Low |
| Urgency | 2 - Medium |
| Priority | 4 - Low |

**Note:** Priority was displayed as `4 - Low` in the incident details. It was not directly selected during incident creation. ServiceNow may calculate priority using impact and urgency according to configured rules.

## Troubleshooting and Resolution

The incident was created to represent a simulated employee connectivity issue.

No actual network troubleshooting or technical remediation has been performed yet. The incident remains in the `New` state pending further workflow practice.

The next stage of this lab will involve documenting simulated troubleshooting activities, updating the incident, and practicing the resolution workflow.

## Security Analysis

- Used a simulated support scenario rather than documenting a real employee's technical problem.
- Avoided including real credentials, passwords, access tokens, or confidential business information.
- Used a sample caller available in the developer instance.
- Documented the incident for educational and portfolio purposes.
- Before publishing screenshots, review them for personal information, account identifiers, or other sensitive details.

## Key Takeaways

- ServiceNow provides an incident management interface for recording and tracking reported IT issues.
- An incident record can include a caller, short description, state, urgency, impact, priority, and customer-visible comments.
- The incident list can be used to locate records, while the details view provides additional information and activity history.
- Priority may be automatically calculated rather than directly editable in a particular view.
- Accurate incident documentation helps support communication, troubleshooting, and accountability throughout the incident lifecycle.

## Skills Demonstrated

- ServiceNow navigation
- IT service management (ITSM) fundamentals
- Incident creation and record verification
- Help desk ticket documentation
- Customer-visible communication
- Incident priority and urgency awareness
- Basic security-conscious documentation
- Technical portfolio documentation with GitHub and Markdown

## Evidence

<img width="1512" height="751" alt="Screenshot 2026-10-19 at 4 45 40 PM" src="https://github.com/user-attachments/assets/504c35bc-2b9e-4c80-bc80-b06f34778a0e" />

<img width="1512" height="184" alt="Screenshot 2026-10-19 at 4 50 00 PM" src="https://github.com/user-attachments/assets/11d6ed36-a3d1-4e83-b967-bcc9aff2726d" />

<img width="1512" height="752" alt="Screenshot 2026-10-19 at 4 53 19 PM" src="https://github.com/user-attachments/assets/9e72dffb-92a3-48c4-bcf0-74d2b3d9670e" />

## Lab Status

**In Progress**

Incident creation and verification are complete. Updating and resolving the incident remain to be practiced before this lab can be marked complete.


