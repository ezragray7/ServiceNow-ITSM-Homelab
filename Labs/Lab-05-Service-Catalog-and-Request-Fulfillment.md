# Lab 05 — Part 1: Service Catalog Exploration

## Objective
Explore the ServiceNow Service Catalog, identify available catalog categories and items, and examine how catalog forms collect information before a service request is submitted.

## Tasks Completed
- Opened the Service Catalog through the Self-Service area.
- Explored catalog categories, including Services, Can We Help You, and Office.
- Identified several available catalog items, including:
  - Change Password
  - Parking Sticker Request
  - Password Reset Enrollment
  - Request Knowledge Base
  - New Hire
  - Password Reset
  - Create Incident
- Identified **New Hire** as an Order Guide.
- Inspected the Parking Sticker Request form and identified its requester, vehicle type, driver's license, and vehicle registration fields.
- Inspected the Password Reset form and identified its questions about the affected user, application, and preferred contact method.
- Inspected the Request Knowledge Base form and identified its two fields:
  - Reason for creating the knowledge base
  - Name of the knowledge base

## Security Analysis
- Service Catalog forms collect information needed to evaluate and process service requests.
- Supporting-document fields may collect sensitive personal information, such as driver's license and vehicle registration documents. Such information should only be submitted when necessary and through authorized channels.
- Password-related requests should be handled through approved identity-verification and password-reset procedures.
- Order Guides can group related catalog items into a coordinated request workflow.
- Catalog items should be reviewed before submission to avoid triggering unnecessary operational work.

## Key Takeaways
- The Service Catalog provides a centralized interface for requesting IT and organizational services.
- Catalog items use structured fields to collect request details.
- Order Guides can coordinate multiple catalog requests.
- Different catalog items collect different information based on their purpose.
- Reviewing a form before submission helps identify required information and potential security considerations.

## Skills Demonstrated
- ServiceNow Service Catalog navigation
- Catalog item identification
- Order Guide identification
- Form-field inspection
- Service request workflow analysis
- Basic data-handling and security awareness

## Evidence
<img width="1512" height="757" alt="Screenshot 2026-10-22 at 8 51 21 AM" src="https://github.com/user-attachments/assets/afb56954-dea7-4872-9e6b-002149015539" />
<img width="1512" height="757" alt="Screenshot 2026-10-22 at 8 58 43 AM" src="https://github.com/user-attachments/assets/a8f724a0-99a3-408d-98bb-a3e5e782abd7" />
<img width="1512" height="432" alt="Screenshot 2026-10-22 at 9 00 52 AM" src="https://github.com/user-attachments/assets/7f0fcd94-8cf8-487e-97d7-b89b6bcb4d3e" />


## Result
Successfully explored the ServiceNow Service Catalog, identified available catalog items and an Order Guide, and reviewed the information collected by several request forms. No service request submission is documented in this part.

# Lab 05 — Part 2: Service Request Submission and Approval

## Objective
Submit a test service request through the ServiceNow Service Catalog, inspect the resulting request record, and validate the approval workflow.

## Tasks Completed
- Submitted a test request using the **Request Knowledge Base** catalog item.
- Entered a training-related reason and a proposed knowledge base name.
- Received a confirmation message stating that the request had been received and that notification would follow after approval.
- Located the request through **Self-Service > My Requests**.
- Identified the request number as `REQ0010001`.
- Inspected the request record and verified the following initial values:
  - Requested for: System Administrator
  - Approval: Requested
  - Request State: Pending Approval
- Opened the associated approval record.
- Identified System Administrator as the approver.
- Approved the request using the available **Approve** action.
- Verified that the approval record's state changed to `Approved`.
- Returned to the main request and verified that both Approval and Request State showed `Approved`.
- Inspected the Requested Items related list and found no records associated with `REQ0010001`.
- Checked the Requested Items list and did not find a requested item linked to this knowledge base request.

## Security Analysis
- Service Catalog requests can require approval before progressing through a workflow.
- Approval records provide visibility into who is responsible for reviewing a request and whether a decision has been made.
- Request approval and fulfillment are separate workflow stages. An approved request does not, by itself, prove that a requested item was generated or fulfilled.
- Requested-item records (RITMs) are used to represent individual catalog items associated with a request.
- Workflow validation should rely on the actual request and related records rather than assuming that approval automatically triggers fulfillment.

## Key Takeaways
- ServiceNow assigns a unique request number when a catalog request is submitted.
- The My Requests page provides access to submitted request records.
- The request initially entered a Pending Approval state.
- The approval record was successfully approved.
- The parent request's Approval and Request State fields both changed to Approved.
- No associated Requested Item record was found for this request during validation.
- Additional investigation would be needed to determine why the requested-item record was not visible or generated.

## Skills Demonstrated
- ServiceNow Service Catalog request submission
- Request record navigation
- Approval workflow inspection
- Approval state validation
- Requested-item record investigation
- ITSM workflow troubleshooting
- Evidence-based technical documentation

## Evidence

<img width="1512" height="432" alt="Screenshot 2026-10-22 at 9 10 00 AM" src="https://github.com/user-attachments/assets/8bde5a2a-04c2-40f5-b81b-01b9eb94bc8c" />
<img width="1512" height="228" alt="Screenshot 2026-10-22 at 9 15 10 AM" src="https://github.com/user-attachments/assets/1bf01f40-97c1-4a5f-8c5f-2c65bc87da12" />
<img width="1512" height="263" alt="Screenshot 2026-10-22 at 9 21 12 AM" src="https://github.com/user-attachments/assets/df1b9839-8105-4284-ae37-df0a186ca823" />
<img width="1512" height="471" alt="Screenshot 2026-10-22 at 9 27 12 AM" src="https://github.com/user-attachments/assets/c2c18b7b-7612-46e6-a601-da54a34f14c3" />
<img width="1512" height="471" alt="Screenshot 2026-10-22 at 9 29 12 AM" src="https://github.com/user-attachments/assets/dd2132de-47a5-496c-9477-43d5f43592ce" />


## Result
Successfully submitted and approved a ServiceNow knowledge base request. The request record reached an Approved state, but no associated Requested Item (RITM) was found during validation. The approval workflow was verified; end-to-end fulfillment was not confirmed.
