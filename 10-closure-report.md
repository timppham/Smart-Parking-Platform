# Project Closure Report (Draft)

INTERNAL: Software Corp use only. Not for distribution to the city.

Project: Smart Parking Platform
Prepared by: Tim Duncan, Project Manager
Version: 0.9 (draft)
Planned go-live: December 8, 2026

# 1. Executive Summary

The Smart Parking Platform is a cloud-based parking system. It involves development of a driver mobile/web application and operator dashboard. It is planned to run between 1st September 2026 and 8 th December 2026. There are 13 people working on this project and it has an approved budget of $488,336 including 15% contingency ($63,696).

Planning is complete. Requirements have been defined with 18 use cases. A Work Breakdown Structure has also been defined, as well as a Gantt Chart with details of dependencies. 6 Milestone points have been created. A Risk Register has been made with 12 risks, alongside a Communications Plan and Cost Plan. Sprint 1 & 2 have been created in Jira. Schedule and cost will be updated once closed.

There are 4 high risks in the project which are having the greatest effect on the project:

Occupancy Sensor API (R-01)

Payment Sandbox Access (R-05)

Compressed QA window (R-06)

Late discovery of PCI-DSS issues (R-12)

A 12 month maintenance agreement has been proposed (starting from day after deployment) with the city. It costs $197,533. This includes bug fixes, API and platform changes, patches and performance improvements. Response times depend on severity.

# 2. Objectives and Deliverables

Objectives from the Vision and Scope
- Drivers will be able to locate, book, pay for parking in an easy application.
- Operator functionality
- Operators will be able to manage their properties, pricing and real-time space availability.
- Real time data is visible to both parties.
- Project completion date: 8 th December 2026. Within budget of $488,336.

Deliverables
- User account, Search, Real Time Availability, Book, Cancel Booking, Payment, Booking History/Receipts, Notifications and Navigation.
- Operator Dashboard: List Properties, Manage Pricing, Real Time Space Availability, Reports, Manual Space Availability
- Admin Functionality: User Account Management, Refunds.
- Technical Development, API, Mapping Integration, Payment Integration, Testing, Deployment.
- Project documentation: SRS, WBS, Gantt Chart, Risk Register, Communication Plan, Resource & Cost Plan, Stakeholder Analysis, Team Charter, Project Charter.

# 3. Achievements and Shortfalls

Achievements:
- Requirements have been completed. We have a SRS document (version 0.6) containing 18 use cases (UC-01 to UC-18), plus FR16 and FR17.
- The Work Breakdown Structure is complete. It outlines all use cases, UX, DevOps and project management.
- The Gantt chart is complete. There are 13 tasks with finish-to-start and start-to-start relationships. Resources are named. There are 6 milestones (Sep 22, Oct 6, Oct 20, Nov 3, Nov 24, Dec 8).
- The risk register is complete. There are 12 risks, each with their owner, mitigation strategy and risk level taken from the matrix.
- The budget has been worked out. We have labour costs of $322,700, overhead $80,675, plus other costs of $21,265, subtotal $424,640 and contingency $63,696, total $488,336.
- Stakeholder analysis has been carried out. We have a Power Interest grid, team charter and project charter.
- The Jira board has a backlog of approximately 62 items. We have 2 sprints (Sprint 1 & 2) with documented objectives. A retrospective has been created (Start/Stop/Continue).
- A communication plan has been created. This has been tailored to our audience. We have monthly demos for the city, sprint boards for developers and weekly risk review.

Shortfalls
- Inconsistencies in initial plan: Cost Plan includes DevOps tasks which aren’t in schedule. Resource Plan includes a UX Designer, but there are no UX tasks in WBS. 2 use cases missing. Risk Register has no risk levels assigned.
- Inconsistencies in our own documentation: Cost Plan, Gantt Chart and RACI are individually accurate but collectively very inaccurate until cross-referenced.
- In first Gantt file tasks were dependent on each other incorrectly and therefore scheduled to occur in 2027. This was identified.
- PCI-DSS Legal Review is scheduled for Month 3, after payment integration has been created. In order to lower risk exposure, a design review was included in Sprint 2. However, as a complete legal review is still scheduled towards the end, risk still remains late (R-12).
- 4 High Risks remain open. No risks have been closed or fully mitigated.
- Remaining items to be confirmed at project closure: final CPI/SPI, actual costs ($488,336), amount of contingency used, and if all sprint goals were met.

# 4. Final Schedule and Budget Comparison

Timeline Planned:
- From 1st September to 8 th December, 2026.
- Actual: To be filled in on completion.

Costs
- Planned Cost: $488,336 ($424,640 + 15% contingency = $63,696)
- Actual Cost & Contingency Used: To be filled in on completion.

# 5. Lessons Learned

Communication
- With 13 people, there are 78 communication paths. To make this manageable, most communication occurred within each team, or in planned meetings.
- Different stakeholders needed different information: city stakeholders wanted information on milestones, cost, and high risks. Developers wanted information on the board and blockers.
- Most issues were in document discrepancies.

Testing and quality
- Test environments and CI/CD were added in Sprint 2 due to R-11.
- Releases have a regression test and rollback strategy in staging. This is due to the example of Knight Capital in an earlier part of the course.
- QA was done early, with 1 week buffer. This is because QA is often compressed if something happens upstream in the project (R-06).

Planning and management
- Dependencies were checked. If finish-to-start dependencies are placed incorrectly, it alters the timing of the schedule.
- Risk ratings were determined from the risk matrix.
- Early requests for sandbox access and strict deadlines for feedback from the firm had no cost, but helped protect the schedule. (R-05, R-10)
- The stakeholder grid meant that the city, operators and development teams were in ‘manage closely’ meaning they had the most direct reporting.

# 6. Recommendations for Future Projects

- Ensure that compliance is reviewed in time. In payments, perform a design review of PCI-DSS in the first month, and a full review before integration begins.
- Ensure partner and vendor sandbox access is requested as soon as possible (ideally in the contract).
- Set up Environments, CI/CD and Test Data in the first sprint.
- Ensure cost plan, timeline, RACI and backlog are consistent with each other (using the same checklist) at every update.
- Have manual workarounds for any features that require data from partners. As with manual occupancy (UC-18).
- Ensure Risk Register is reviewed weekly. Any new High risks should be escalated on the same day.
- Maintain a single source of lessons learnt. Add to this at the end of every sprint.
- Final Retrospective with the whole team. A brief summary should be published to the city.

# 7. Closure Checklist

- Confirm deliverables match all 18 user stories.
- Receive written sign-off from city and Product Owner.
- Free up resources within the project and close the budget.
- Store documentation, code and Jira boards in the repo.
- Pass architecture diagrams, run books, contact lists, and issues to support.
- Final Retrospective.
- Send closure report to management at Software Corp.
- Say thanks to the team.

# 8. Post-Project Proposal: Maintenance Contract

Software Corp propose to provide maintenance on the system for 12 months from 9 th December 2026 until 8 th December 2027. The values given below are estimates based on the rates from the resource and cost plan. They are subject to agreement.

8.1 Why maintenance and not scaling

As there is only one deployment across one city, and there is no indication that we will be deploying to any more cities or expanding the team in the contract, this maintenance period is most appropriate. The platform relies on external services (payment, maps and garage occupancy data) which may change after deployment. Compliance with PCI-DSS will also continue after deployment. If we do scale the platform in the future, we will have 1 years data on performance, load and support to understand how we should scale.

8.2 What is covered

- Fixing bugs and issues that occur in live.
- Adaptive: Updating platform in response to changes in external systems (iOS/Android updates, mapping/payment API changes).
- Perfective: Improving performance to meet NFR1 (search time < 2s) and NFR5 (availability refresh < 30s) as usage increases.
- Preventive: Refactoring and reducing technical debt to avoid failure.

Not included: New functionality. These will be handled via change control and charged separately. The charge for new functionality is time and materials at the rates given in the cost plan per hour.



8.3 Phases

- Handover (before 8th Dec): Architecture diagrams, run books, contact details and known issues will be transferred to support team.
- Stabilisation (9th Dec – 5th Jan): Daily check-ins. Quick fixes to bugs and hot fixes. Early patches.
- Steady State (6th Jan – 20th Nov 2027): Planned changes made monthly. Patches and improvements.
- Evolution Review (20th Nov 2027): Decision to sustain, refactor, rewrite parts of the system. Decision to renew or scale.

8.4 Support model

- Tier 0: Support within application by drivers/operators.
- Tier 1: Initial support from city helpdesk. Ticket raised in Jira.
- Tier 2: Issue reproduced by Software Corp support (QA and DevOps). If applicable, known fix applied from run books.
- Tier 3: Root cause fixed by developers.
- On-call: Rotation of backend developer, DevOps and web/mobile developer to provide 24/7 support for severity 1 issues. Documented sign off between engineers at change.

8.5 Service levels

Proposed targets, to be agreed with the city:

- Uptime: 99.5% per month, excluding planned maintenance windows
- Severity 1:  1 Hour response time, 4 Hour resolution/around, 24/7. (Platform unavailable, payments not working, reservations not possible)
- Severity 2: 4 Hour response time, 2 working day resolution. (Major functionality failure with workaround)
- Severity 3: 1 working day response time, resolved in next monthly release. (Minor defects)
- Severity 4: Backlog. (Questions or appearance issues)
- Severity 2 to 4 support: Mon-Fri, 8am-6pm.
- 5% credit given on the monthly cost for months where SLA was not met.

Monthly metrics will be reported: Uptime, MTTD, MTTR, MTBF, Error rate, Search latency (NFR1), Availability refresh (NFR5), Customer satisfaction (Driver and Operator).

8.6 Incident management and runbooks

All incidents follow the same process: detection, triage, containment, resolution, post-mortem. Runbooks exist for the following failures which are predicted in our risk register.

- Occupancy feed down (R-01): Switch to manual input for occupancy (UC-18) and inform operator.
- Payment gateway outage (R-02): Retry logic, monitor status, alert drivers.
- Mapping API limit or deprecation (R-03): Use cached results, contact vendor.
- Failed release: Rollback following rollback plan in release process.

For severity 1 and 2 incidents, blameless post-mortems are carried out. The root cause and actions for improvement will be identified. The city is updated during the incident, and a brief summary is given after.

8.7 Change and release management

- All changes have approval, risk analysis and rollback plan.
- Releases are deployed into staging with automated regression testing, and deployed to production with feature toggles or progressive deployment.
- Releases occur once a month on Sundays between 2am and 5am local time. Emergency fixes may be deployed outside of this window with approval from the Product Owner.
- All releases have a verified rollback plan.

8.8 Monitoring and security

- Monitoring dashboards and alerts are in place for known scenarios. In addition, logging, metrics and tracing is in place to investigate unknown issues.
- OS, runtimes & dependencies are patched monthly. Critical security patches are done within 72 hours using an emergency process.
- Dependencies are scanned in every build. Static and dynamic security testing occurs quarterly.
- Compliance: Review for PCI-DSS once per year and compliance with city ordnances. Findings are recorded for audit.

8.9 Technical debt

10% of developer time is spent on preventative work. Technical debt is recorded in Jira, prioritised by risk and scheduled for specific releases. If any shortcuts were taken to meet the deadline of the 8 th of December, they will be added to this list upon handover.

8.10 Continuous improvement

Each quarter the team runs a Plan, Do, Check, Act cycle using the monthly metrics, user feedback, and bug reports. A retrospective follows every major incident and every quarterly review, and its actions go into the backlog.

8.11 Team and cost

Team (2,080 hours per full-time year):

- Backend/API developer: Jalen Johnson, 20%, 416 hours at $65 = $27,040
- DevOps engineer: Fred VanVleet, 20%, 416 hours at $80 = $33,280
- Web and mobile developer: Austin Reaves, 20%, 416 hours at $65 = $27,040
- QA engineer: Donovan Clingan, 10%, 208 hours at $50 = $10,400
- Service manager: Tim Duncan, 10%, 208 hours at $60 = $12,480

Labor: 1,664 hours, $110,240

Annual cost:

- Labor: $110,240
- Overhead (25%): $27,560
- Production hosting: $2,500 per month for 12 months = $30,000
- Third-party APIs: $500 per month for 12 months = $6,000, based on the sandbox rate. Higher production usage is billed at cost, and R-08 usage caps and cost alerts stay in place
- Licenses: 5 at $155 = $775
- Annual PCI-DSS and compliance review: $5,000
- Subtotal: $179,575
- Contingency (10%): $17,958
- Total: $197,533, about $16,461 per month

Total cost of ownership for the first year: $488,336 to build plus $197,533 to maintain = $685,869.

Contract type: a fixed monthly fee for the covered work above, and time-and-materials for any enhancement the city asks for.

8.12 Risks to the maintenance contract

- Key resource missing in development team R-09 Documented, working in pairs, role duplication
- Changes to API by partner with short notice R-03 Adaptive maintenance, SLA with vendor
- Costs from 3rd party increase with usage R-08 (Limits and warnings)
- Additional functionality requested by city within maintenance All enhancements will need to go through change control, and incur an additional charge
- Slow city feedback/approvals Support timelines from city defined in contract R-10

8.13 What the city provides

- Single point of decision making/ prioritisation
- Tier 1 support team.
- Feedback on release notes and change requests within timescales
- Access to partners in garage for occupancy data

8.14 How success is measured

- Uptime is at least 99.5% monthly
- All Sev 1/2 issues resolved within SLA.
- NFR1 and NFR5 achieved in all monthly reports.
- No outstanding high security issues older than 72hrs.
- Quarterly review with city. Decision on renewal made in November 2027.

# 9. Acknowledgments and Sign-off

Many thanks to the team of 13 people. Many thanks to the Product Owner for clear priorities, and to city stakeholders for feedback.