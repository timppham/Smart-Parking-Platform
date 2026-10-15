1. Risks by Category
Technical
- Parking occupancy sensor/camera API from garage partners proves unreliable or inconsistent
- Third-party payment gateway integration has downtime or breaking API changes
- Mapping/navigation service rate limits or deprecates the API being used
- Real-time data sync between driver app and operator dashboard lags or desyncs

Schedule
- Backend authentication takes longer than planned, delaying frontend work that depends on it
- Payment and mapping integrations slip because third-party partner approval/sandbox access is delayed
- QA testing phase gets compressed if earlier development phases run over
- Operator dashboard features depend on reporting requirements that are still being refined

Financial
- Payment gateway transaction fees run higher than budgeted at scale
- Third-party API costs (mapping, sensor data) scale up unexpectedly with usage
- City contract milestone payments are delayed, affecting cash flow for the project
- Scope creep from the city client adding features mid-contract without budget adjustment

People
- A developer on a critical path (e.g., backend/auth) leaves or becomes unavailable
- Miscommunication between the Mobile and Backend/API teams causes integration rework
- Inexperience of a team member regarding payments/PCI-DSS compliance leads to delays
- Lack of responses from operator-side stakeholders prevents dashboards approval

2. Risk Matrix
Impact columns in order: Negligible, Minor, Moderate, Major, Catastrophic

Very High (5): Low, Medium, High, High, Extreme
High (4): Low, Medium, High, High, Extreme
Moderate (3): Low, Medium, Medium, High, High
Low (2): Low, Low, Medium, Medium, High
Very Low (1): Low, Low, Low, Medium, Medium

Risk Level is read straight from this grid. It is not a sum of the two numbers.

3.Risk Register
R-01

Description: Occupancy sensor API unreliable
Category: Technical
Probability: Moderate (3)
Impact: Major (4)
Risk Level: High
Owner: Backend/API Team
Response: Mitigate, add a manual entry fallback (UC-18, FR17)
Status: Open

R-02

Description: Payment gateway downtime
Category: Technical
Probability: Low (2)
Impact: Major (4)
Risk Level: Medium
Owner: Payment Integration Team
Response: Mitigate, add retry logic and status monitoring
Status: Open

R-03

Description: Mapping API rate limits or deprecation
Category: Technical
Probability: Low (2)
Impact: Moderate (3)
Risk Level: Medium
Owner: Mapping & Location Team
Response: Transfer, rely on the vendor SLA
Status: Open

R-04

Description: Backend auth delays frontend start
Category: Schedule
Probability: Moderate (3)
Impact: Moderate (3)
Risk Level: Medium
Owner: Project Manager
Response: Mitigate, build frontend mockups while the backend is built
Status: Open

R-05

Description: Third-party sandbox access delayed
Category: Schedule
Probability: Moderate (3)
Impact: Major (4)
Risk Level: High
Owner: Payment Integration Team
Response: Avoid, request sandbox access early in the contract
Status: Open

R-06

Description: QA phase compressed by upstream delays
Category: Schedule
Probability: High (4)
Impact: Major (4)
Risk Level: High
Owner: QA Team
Response: Mitigate, reserve a buffer week before deployment
Status: Open

R-07

Description: Payment fees exceed budget at scale
Category: Financial
Probability: Low (2)
Impact: Moderate (3)
Risk Level: Medium
Owner: Project Manager
Response: Accept, monitor and reforecast quarterly
Status: Open

R-08

Description: Third-party API costs scale unexpectedly
Category: Financial
Probability: Moderate (3)
Impact: Moderate (3)
Risk Level: Medium
Owner: Project Manager
Response: Mitigate, set usage caps and cost alerts
Status: Open

R-09

Description: Key backend developer becomes unavailable
Category: People
Probability: Low (2)
Impact: Major (4)
Risk Level: Medium
Owner: Project Manager
Response: Mitigate, document code and use pair programming
Status: Open

R-10

Description: Operator stakeholder feedback delays sign-off
Category: People
Probability: Moderate (3)
Impact: Moderate (3)
Risk Level: Medium
Owner: Project Manager
Response: Mitigate, set firm feedback deadlines in the contract
Status: Open

R-11 

Description: Build pipeline and test environments set up late
Category: Technical
Probability: Moderate (3)
Impact: Moderate (3)
Risk Level: Medium
Owner: DevOps Engineer
Response: Mitigate, put environment and CI/CD setup in Sprint 2
Status: Open

R-12 

Description: PCI-DSS problems found after payment integration is built, since the $5,000 legal review is in Month 3
Category: Technical
Probability: Moderate (3)
Impact: Major (4)
Risk Level: High
Owner: Payment Integration Team
Response: Mitigate, run a PCI-DSS design review in Sprint 2
Status: Open

Summary: 4 High risks (R-01, R-05, R-06, R-12), 8 Medium, 0 Low, 0 Extreme.

4. Quality
QA (prevent defect): code reviews on all pull requests, coding standards, design review with the Product Owner
QC (detect defect): unit test, integration test, security test, regression test and user acceptance test
Lesson learned from Knight Capital: releases happen after passing through a staging environment, regression test is done before each release and there is a rollback plan in case of production failure
Defects are tracked using a Kanban board with columns To Do, In Progress, Testing and Done

5. Communication Plan
Meetings

Daily stand-up for each team. Three questions: what I did, what I will do, what is blocking me
Mobile and Web with Backend/API: sync twice a week on API changes
Mapping team: weekly sync with Backend/API
Payment Integration with QA: sync before every test cycle
UX joins the Mobile and Web stand-ups. DevOps joins the Backend stand-up
Sprint planning, sprint review and retrospective every 2 weeks. The Project Manager acts as Scrum Master. The retrospective uses Start, Stop, Continue
Weekly cross-team progress meeting that includes a risk register review
Monthly demo to the city stakeholders

Communication paths

13 people means 13 x 12 / 2 = 78 possible channels. The team structure and the meeting list above keep that manageable, so most talk happens inside a team or in a scheduled meeting.

Reporting by audience

City stakeholders and executives: monthly demo and a short report with milestone status, budget against the $488,336 plan, schedule and cost performance (SPI and CPI), and the High risks. No technical detail
Developers and teams: Jira backlog and sprint board with tasks, progress and blockers
Risk tracking: register reviewed weekly. New High or Extreme risks are escalated right away

Code review workflow

Work happens on a feature branch. The main branch always stays deployable
Small commits with clear messages
Every pull request is named with the Jira issue key and reviewed by at least one other developer
CI builds and tests on each push
The Jira issue moves to Done only after the pull request is merged and tests pass