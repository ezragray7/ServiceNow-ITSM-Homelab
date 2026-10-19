
# Lab 02: Users and Assignment Groups

## Objective
Practice core ServiceNow IT Service Management (ITSM) administration tasks by reviewing user records, creating a test user, creating an assignment group, configuring group membership, assigning an incident to the group, and reviewing user roles and group access.

## Environment
- **Platform:** ServiceNow Personal Developer Instance (PDI)
- **Interface:** Service Desk / User Administration
- **Lab Type:** ITSM administration and access control
- **Test User:** `lab.test.user`
- **Assignment Group:** `IT Support - Lab Team`
- **Incident:** `INC0010002`

## Security Focus
This lab demonstrates the importance of accurate user administration, support-team organization, incident ownership, and access control review. It also highlights the distinction between group membership and directly assigned roles.

---

## Part 1: User Records

### Objective
Review existing ServiceNow user records and create a dedicated test user for ITSM administration exercises.

### Tasks Completed
- Navigated to the Users list.
- Reviewed an existing user record.
- Identified user account fields, including User ID, name, email, and Active status.
- Verified that the reviewed existing account was active.
- Created a dedicated test user:
  - First Name: `Lab`
  - Last Name: `Test User`
  - User ID: `lab.test.user`
  - Email: `lab.test.user@example.com`
  - Active: Enabled
- Saved the new user and verified that the record was created successfully.
- Reviewed the user's Roles and Groups related lists.

### Security Analysis
User records identify individuals who interact with the ServiceNow platform. The Active field helps administrators manage whether an account is enabled. Dedicated test accounts also help separate training activities from normal user administration.

The test account was created specifically for this lab. Its example.com email address identifies it as a training record rather than a production contact.

### Key Takeaways
- User records contain identity and account-status information.
- Test accounts can support repeatable administration exercises.
- Account status should be reviewed during access audits.
- An empty Roles related list does not necessarily prove that an account has no effective permissions.

### Skills Demonstrated
- ServiceNow user administration
- User record inspection
- Test account creation
- Account-status verification
- Basic access review

---

## Part 2: Assignment Groups

### Objective
Create a support assignment group and configure group membership for incident-management exercises.

### Tasks Completed
- Located and inspected the existing Service Desk group.
- Reviewed group fields such as Name, Manager, Group email, Active, and Group Members.
- Left the existing Service Desk group unchanged.
- Created a new group named `IT Support - Lab Team`.
- Added the following description:

  `Training group for the ServiceNow ITSM homelab. Used to practice incident assignment, support team organization, and access management.`

- Left the Manager, Group email, and Parent fields blank.
- Saved the group successfully.
- Added `lab.test.user` to the group.
- Verified that the test user appeared in the Group Members list.

### Security Analysis
Assignment groups organize users into teams that can own and manage work. Creating a dedicated lab group makes it possible to practice incident routing without modifying an existing support group.

Group membership can influence work assignment and may contribute to access granted through roles or other platform configuration. Membership should therefore be intentional and periodically reviewed.

### Key Takeaways
- Assignment groups organize support personnel.
- Group membership can be managed through the group's member list.
- Existing groups should not be modified unnecessarily during isolated lab exercises.
- Successful membership updates should be verified in the saved record.

### Skills Demonstrated
- Assignment group administration
- Group record creation
- Group membership management
- Verification of saved configuration

---

## Part 3: Incident Assignment

### Objective
Assign an existing incident to a custom support group and verify that the assignment persists after saving.

### Tasks Completed
- Opened incident `INC0010002`.
- Reviewed the Assignment group and Assigned to fields.
- Set the Assignment group to `IT Support - Lab Team`.
- Saved the incident.
- Reopened the incident and verified that the Assignment group value persisted.
- Left Assigned to blank because `lab.test.user` was not available in the selection list.

### Security Analysis
Incident assignment establishes responsibility for investigating and resolving reported issues. Group-level assignment provides a clear team owner even when a specific individual has not yet been selected.

The inability to select the test user individually was not treated as proof of a permissions failure. Possible causes require further investigation. The incident was successfully assigned at the group level, and the individual assignment field was left unchanged.

### Key Takeaways
- Assignment group and Assigned to serve different purposes.
- Group assignment can establish ownership without selecting an individual.
- Saved changes should be verified by reopening the record.
- User-selection behavior may depend on platform configuration and eligibility rules.

### Skills Demonstrated
- Incident record navigation
- Incident assignment
- Group-based work routing
- Saved-record verification
- Basic troubleshooting of assignment behavior

---

## Part 4: User and Group Access Control Review

### Objective
Review the test user's directly listed roles and group memberships without making unnecessary permission changes.

### Tasks Completed
- Opened the `lab.test.user` record.
- Inspected the Roles related list.
- Confirmed that no roles were directly listed in that related list.
- Inspected the Groups related list.
- Confirmed that `IT Support - Lab Team` appeared in the user's group memberships.
- Made no role or group changes during the access review.

### Security Analysis
Access reviews help administrators understand how users are organized and where access-related configuration may be assigned. In this lab, the test user had no entries in the directly listed Roles related list and was a member of the custom IT support group.

An empty direct Roles list does not establish that the user has no effective permissions. ServiceNow access can also be influenced by inherited roles, group-related role assignments, access control lists (ACLs), and other platform configuration. A full effective-access audit would require examining those mechanisms separately.

### Key Takeaways
- Direct role assignments and group memberships are distinct.
- Group membership should be verified after changes.
- Permissions should not be added merely to make a lab record appear more complete.
- Effective access cannot be determined from the direct Roles list alone.

### Skills Demonstrated
- User access review
- Role and group inspection
- Least-privilege awareness
- Basic access-control analysis
- Documentation of access-review findings

---

## Final Lab Summary

This lab provided hands-on experience with foundational ServiceNow ITSM administration. A dedicated test user and custom support group were created, group membership was verified, an incident was assigned to the new group, and the user's directly listed roles and group memberships were reviewed.

The lab reinforced the relationship between user administration, group-based work ownership, and access control. It also demonstrated the importance of validating saved changes and distinguishing observed configuration from assumptions about effective permissions.

## Skills Demonstrated
- ServiceNow ITSM navigation
- User and group administration
- Incident management and assignment
- Group membership verification
- Basic access-control review
- Security-focused documentation
- Evidence collection for a technical portfolio

---

## Evidence Screenshots

<img width="1512" height="756" alt="Screenshot 2026-10-19 at 5 52 13 PM" src="https://github.com/user-attachments/assets/0780748f-c0b3-401c-8e50-5851975506c5" />

<img width="1512" height="565" alt="Screenshot 2026-10-19 at 5 55 54 PM" src="https://github.com/user-attachments/assets/84ebd3c9-7f4e-4f9e-9627-747319621f48" />

<img width="1512" height="755" alt="Screenshot 2026-10-19 at 5 58 15 PM" src="https://github.com/user-attachments/assets/13a3b3ca-be10-4f67-9d66-5f591735475c" />

<img width="1512" height="755" alt="Screenshot 2026-10-19 at 6 09 20 PM" src="https://github.com/user-attachments/assets/b5888fcf-d937-4b5c-8591-95dc3fada3f0" />

<img width="1512" height="755" alt="Screenshot 2026-10-19 at 6 15 00 PM" src="https://github.com/user-attachments/assets/edbc6c8b-ea24-4040-a35d-d5455fd791b0" />

<img width="1512" height="210" alt="Screenshot 2026-10-19 at 6 43 22 PM" src="https://github.com/user-attachments/assets/8c7844e7-d2fe-40df-8503-ff1b9ba8bf96" />

---

## Evidence Checklist
- [x] Existing user record reviewed
- [x] Test user created and verified
- [x] Custom assignment group created
- [x] Group membership verified
- [x] Incident assignment saved and verified
- [x] User Roles and Groups related lists reviewed
- [x] Evidence screenshot references added to the Markdown file
