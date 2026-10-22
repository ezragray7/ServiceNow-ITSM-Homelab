# Lab 04 — Part 1: Knowledge Article Creation

## Objective
Create a ServiceNow knowledge article using the Standard template, assign it to the appropriate knowledge base and category, and observe the initial publication workflow.

## Environment
- Platform: ServiceNow Personal Developer Instance (PDI)
- Module: Self-Service > Knowledge
- Knowledge Base: IT Knowledge Base
- Template: Standard

## Tasks Completed
- [x] Opened the Knowledge module.
- [x] Selected the IT Knowledge Base.
- [x] Selected the Standard article template.
- [x] Entered the article title: Troubleshooting Common Account Login Issues.
- [x] Selected the IT category.
- [x] Left Scheduled Publish Date and Valid To blank.
- [x] Created an article containing troubleshooting steps, security reminders, escalation guidance, and support-request recommendations.
- [x] Saved the article after satisfying the minimum article-length requirement.
- [x] Selected Publish and observed a message indicating that the item was in review.
- [x] Located the saved article under My Knowledge Articles.
- [x] Verified that the article remained in review.

## Article Summary
The article provides general guidance for users experiencing account login problems. It covers credential verification, account lockouts, application access, network connectivity, security precautions, and escalation to IT support.

## Workflow Observations
Selecting Publish did not immediately make the article available as a published knowledge article. ServiceNow displayed an in-review message, and the article remained accessible under My Knowledge Articles with its status still in review.

This exercise demonstrated that saving a knowledge article and initiating publication are separate steps in the observed workflow.

## Security Analysis
The article emphasizes safe account-recovery practices, avoiding password sharing, protecting verification codes, and using approved IT support channels.

No real user credentials or sensitive account information were included in the article.

## Key Takeaways
- Knowledge articles are organized by knowledge base and category.
- ServiceNow provides different article templates for different knowledge-management purposes.
- The Standard template is appropriate for general IT troubleshooting guidance.
- The article editor enforced a minimum content-length requirement.
- Selecting Publish can initiate a review workflow rather than immediate publication.
- My Knowledge Articles provides a way to locate the saved article while it is in review.

## Skills Demonstrated
- ServiceNow Knowledge Management
- Knowledge article creation and organization
- IT documentation and troubleshooting writing
- Knowledge publication workflow validation
- Basic security-awareness documentation

## Evidence
<img width="1512" height="749" alt="Screenshot 2026-10-21 at 2 29 53 PM" src="https://github.com/user-attachments/assets/8df7c4e4-16ca-4234-876d-57ba9c302fce" />

<img width="1512" height="749" alt="Screenshot 2026-10-21 at 2 30 04 PM" src="https://github.com/user-attachments/assets/b98cb63a-17c3-404b-b76f-9716330cbf61" />

<img width="1512" height="258" alt="Screenshot 2026-10-21 at 2 33 11 PM" src="https://github.com/user-attachments/assets/46da7629-3836-4f6c-8737-9f8f31ee40b7" />

# Lab 04 — Part 2: Review Article Workflow

## Objective
Inspect and validate the ServiceNow knowledge article review and approval workflow, approve the training article, and verify that it becomes available through the Knowledge portal.

## Environment
- Platform: ServiceNow Personal Developer Instance (PDI)
- Module: Knowledge Management
- Article: Troubleshooting Common Account Login Issues
- Knowledge Base: IT Knowledge Base

## Tasks Completed
- [x] Located the article under My Knowledge Articles.
- [x] Confirmed the article's Workflow field was set to Review.
- [x] Inspected the Approvals tab.
- [x] Found an approval record with the initial state Requested.
- [x] Identified the approver listed on the record as Bernard Laboy.
- [x] Inspected the Article Versions tab.
- [x] Observed article versions 0.01 and 0.02.
- [x] Confirmed version records displayed version, modified by, and modified on fields.
- [x] Approved the requested approval record.
- [x] Verified that the approval state changed to Approved.
- [x] Returned to the article record and confirmed its Workflow field changed to Published.
- [x] Opened the regular Knowledge portal and verified that the published article was visible.

## Workflow Results
The article initially entered the Review workflow after Publish was selected. Its approval record showed Requested. After the approval was granted, the approval state changed to Approved and the article's Workflow field changed to Published.

The published article was subsequently visible through the regular Knowledge portal.

## Version History Observations
The Article Versions tab contained versions 0.01 and 0.02. The records displayed the version number, the user who modified the version, and the modification date and time.

## Security Analysis
The review and approval process provides a checkpoint before a knowledge article becomes available to readers. In a production environment, approval permissions and reviewer responsibilities should be configured according to organizational policy.

The training article contains general account troubleshooting guidance and does not include real user credentials.

## Key Takeaways
- Saving an article and publishing it are separate actions.
- Selecting Publish can initiate a review workflow.
- Approval records can track the approval state.
- Approving the request advanced this article to Published.
- Published articles can be accessed through the regular Knowledge portal.
- ServiceNow maintains article version history.

## Skills Demonstrated
- ServiceNow Knowledge Management
- Knowledge article lifecycle management
- Approval workflow validation
- Article version history inspection
- Publication verification
- IT documentation and security awareness

## Evidence
<img width="1512" height="750" alt="Screenshot 2026-10-22 at 8 22 28 AM" src="https://github.com/user-attachments/assets/2db8c260-d3c2-4583-9bad-b4e6f4236d46" />

<img width="1512" height="446" alt="Screenshot 2026-10-22 at 8 23 34 AM" src="https://github.com/user-attachments/assets/07c69675-f22e-45d3-8608-e42ac5dd87c2" />

# Lab 04 — Part 3: Validate Knowledge Access

## Objective
Validate that a published ServiceNow knowledge article can be found and opened through the Knowledge portal, and inspect the reader-facing features available for the article.

## Environment
- Platform: ServiceNow Personal Developer Instance (PDI)
- Module: Self-Service > Knowledge
- Knowledge Base: IT Knowledge Base
- Article: Troubleshooting Common Account Login Issues

## Tasks Completed
- [x] Opened the published article through the regular Knowledge portal.
- [x] Verified that the article content was visible.
- [x] Identified reader-facing feedback controls.
- [x] Selected Helpful and received a confirmation message.
- [x] Verified that feedback records appeared in the article's Feedback tab.
- [x] Observed three feedback records created after selecting Helpful three times during screenshot capture.
- [x] Checked the Related Articles section.
- [x] Confirmed that no related articles were displayed.
- [x] Checked for attachments and downloadable links.
- [x] Confirmed that no attachments or links were available.
- [x] Searched the Knowledge portal for the article title.
- [x] Confirmed that the article appeared in search results.

## Access Validation Results

### Article Visibility
The article opened successfully through the regular Knowledge portal after its workflow reached Published.

### Search Discoverability
Searching for "Troubleshooting Common Account Login Issues" returned the article in the Knowledge portal results.

### Reader Feedback
Selecting Helpful displayed a feedback confirmation message. The article's Feedback tab subsequently showed three records, corresponding to the three clicks performed during screenshot capture.

### Related Articles
The Related Articles section was available, but no related articles were displayed.

### Attachments and Links
No attachments or downloadable links were available for the article.

## Security Analysis
The published article provides general account troubleshooting guidance and reminds readers not to share passwords or include them in support tickets.

The exercise validated basic article visibility and feedback behavior. It did not test access using a separate user account or verify role-based access restrictions.

## Key Takeaways
- Published knowledge articles can be opened through the regular Knowledge portal.
- Articles can be discovered through Knowledge search.
- Reader feedback can be submitted and recorded.
- Related articles may be absent when no related content is configured.
- Attachments and links are only available when provided with the article.
- Testing a reader-facing page does not, by itself, prove that role-based access controls are correctly configured.

## Skills Demonstrated
- ServiceNow Knowledge Management
- Knowledge article search and discovery
- Reader-facing article validation
- Feedback feature testing
- Knowledge content verification
- Basic security and access-validation documentation

## Evidence
<img width="1512" height="755" alt="Screenshot 2026-10-22 at 8 28 33 AM" src="https://github.com/user-attachments/assets/45ebd426-3d2f-4d04-8afa-9927696288d5" />

<img width="1512" height="755" alt="Screenshot 2026-10-22 at 8 32 23 AM" src="https://github.com/user-attachments/assets/f4a650b1-9f99-480c-88fd-5cd87ab68151" />

<img width="1512" height="353" alt="Screenshot 2026-10-22 at 8 33 50 AM" src="https://github.com/user-attachments/assets/a1316974-badc-49e5-8a32-c321ee0c0299" />

<img width="1512" height="757" alt="Screenshot 2026-10-22 at 8 39 18 AM" src="https://github.com/user-attachments/assets/ae6a8ee0-0eac-42ee-9c8c-cf8b867666e9" />


# Lab 04 — Knowledge Management

## Overview
This lab explored ServiceNow Knowledge Management by creating a knowledge article, testing its review and approval workflow, and validating reader access through the Knowledge portal.

## Objectives
- Create and organize a knowledge article.
- Understand the article review and approval process.
- Verify article publication and search discoverability.
- Test reader feedback functionality.
- Document knowledge article access and related features.

## Lab Parts Completed
- **Part 1 — Knowledge Article Creation:** Created a Standard knowledge article titled "Troubleshooting Common Account Login Issues" in the IT Knowledge Base and assigned it to the IT category.
- **Part 2 — Review Article Workflow:** Inspected the approval record, approved the article, and verified that its workflow changed from Review to Published.
- **Part 3 — Validate Knowledge Access:** Confirmed the published article was accessible and searchable through the Knowledge portal, tested reader feedback, and inspected related articles and attachment availability.

## Key Findings
- ServiceNow enforced a minimum article length of more than 300 words.
- Selecting Publish initiated a review workflow rather than immediately publishing the article.
- The approval record initially showed Requested and changed to Approved after approval.
- The article workflow subsequently changed to Published.
- Article version history included versions 0.01 and 0.02.
- The published article appeared in Knowledge search results.
- Selecting Helpful displayed a confirmation, and three feedback records appeared after three clicks.
- No related articles, attachments, or downloadable links were displayed for this article.

## Security Analysis
The knowledge article provided general account troubleshooting guidance, including credential verification, account lockout handling, application access checks, and escalation to IT support.

The article emphasized safe account recovery practices and avoiding the disclosure of passwords or verification codes.

This lab validated the basic publication and reader experience. It did not verify role-based access restrictions using a separate user account.

## Skills Demonstrated
- ServiceNow Knowledge Management
- Knowledge article creation and categorization
- Article review and approval workflows
- Article version history inspection
- Knowledge search and publication validation
- Reader feedback testing
- IT documentation and security awareness

## Lab Conclusion
This lab demonstrated the basic lifecycle of a ServiceNow knowledge article, from creation and review through approval, publication, and reader access validation.

The exercise provided practical experience with knowledge content management and the workflow controls used to publish IT support documentation.
