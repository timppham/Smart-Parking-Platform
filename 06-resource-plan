# 6. Resource and Cost Management: Smart Parking Platform

An unlimited budget can be set for the project brief. The total cost of this approach will be incurred in any case, so there will be some ground for comparison during the process of project development.

# 6.1 Roles and Resources

Assumption: The duration for the project is 14 weeks (September 1 to December 8, 2026), assuming a working week of 40 hours, one person equals 560 hours. Skills include Junior (0 to 2 years), Mid (3 to 6 years), and Senior (7+ years). The names are placeholders. Allocations are averaged across all 14 weeks. The Gantt chart shows when each person’s work peaks.
# Team
- Product Owner: Anthony Black. Senior, 25% allocation, 140 hours at $70 per hour = $9,800
- Project Manager: Tim Duncan. Senior, 50% allocation, 280 hours at $60 per hour = $16,800
- Solutions Architect: Cam Johnson. Senior, 25% allocation, 140 hours at $100 per hour = $14,000
- UX Designer: Max Christie. Mid, 50% allocation, 280 hours at $60 per hour = $16,800
- Backend/API Developer: Anthony Davis. Senior, 100% allocation, 560 hours at $80 per hour = $44,800
- Backend/API Developer: Jalen Johnson. Mid, 100% allocation, 560 hours at $65 per hour = $36,400
- Payment Integration Developer: Jalen Brunson. Senior, 75% allocation, 420 hours at $80 per hour = $33,600
- Mapping & Location Developer: Alperen Sengun. Mid, 75% allocation, 420 hours at $65 per hour = $27,300
- Web App Developer: Austin Reaves. Mid, 100% allocation, 560 hours at $65 per hour = $36,400
- Mobile App Developer: Amen Thompson. Mid, 100% allocation, 560 hours at $65 per hour = $36,400
- DevOps Engineer: Fred VanVleet. Senior, 50% allocation, 280 hours at $80 per hour = $22,400
- QA Engineer: Donovan Clingan. Mid, 60% allocation, 336 hours at $50 per hour = $16,800
- QA Engineer: Reed Sheppard. Junior, 50% allocation, 280 hours at $40 per hour = $11,200

Total: 4,816 hours, $322,700

# Role Definitions
- Product Owner: Prioritizes the backlog and verifies that features are complete. Operators come first.
- Project Manager: Builds the schedule and manages risks. Reports to the city stakeholders.Also acts as Scrum Master (sprint planning, stand-ups, reviews, retrospectives).
- Solutions Architect: Responsible for the architecture of the system.
- UX Designer: Responsible for designing the driver and operator application screens.
- Backend/API Developer: Implements the back-end services, databases, and related APIs used by the applications.
- Payment Integration Developer: Integrates the payment provider and handles PCI-DSS requirements.
- Mapping & Location Developer: Integrates the mapping service, map searches, and navigation.
- Web App Developer: Builds the web version of the driver application and the operator dashboard.
- Mobile App Developer: Builds the mobile driver application for iOS and Android.
- DevOps Engineer: Maintains the cloud environments, creates the build and deployment pipeline, and releases the software.
- QA Engineer: Prepares test cases, runs tests, and reports bugs.

# 6.2 Cost Plan (Bottom-Up)
- Labor: 4,816 labor hours by 13 people for 14 weeks = $322,700
- Overhead: 25% of labor cost = $80,675.
- Cloud hosting: $2,500 per month for 3.5 months = $8,750. This accounts for both the development and staging environment.
- Licenses & Tools: 13 licenses @ $155 each = $2,015. For Jira, GitHub, Figma & IDE.
- Third-party APIs: $500 per month for 2 months = $1,000. For mapping & payments sandbox services.
- Test devices: $3,000, one-off. iOS and Android test phones.
- Training: $1,500, one-off. PCI-DSS secure coding.
- Legal and compliance: $5,000, one-off. PCI-DSS and city ordinance review.

Subtotal before contingency: $424,640

Contingency: 15% of the subtotal = $63,696

Total cost: $488,336

Contingency is 15%. Contingency typically ranges between 5% and 20%, and our risk register has four High risks (R-01, R-05, R-06, R-12), all associated with external factors or schedule.
# 6.3 Monthly Cashflow

Months are 4-week project months, not calendar months. Month 4 is the last two weeks.

# Month 1 (Sep 1 to Sep 28)

- Labor: $92,200
- Overhead (25%): $23,050
- Infra: $2,500
- Other: $6,515 (licenses $2,015, test devices $3,000, training $1,500)
- Contingency (15%): $18,640
- Month total: $142,905

# Month 2 (Sep 29 to Oct 26)

- Labor: $92,200
- Overhead (25%): $23,050
- Infra: $2,500
- Other: $500 (API usage)
- Contingency (15%): $17,738
- Month total: $135,988

# Month 3 (Oct 27 to Nov 23)

- Labor: $92,200
- Overhead (25%): $23,050
- Infra: $2,500
- Other: $5,500 (API usage $500, legal and compliance review $5,000)
- Contingency (15%): $18,487
- Month total: $141,737

# Month 4 (Nov 24 to Dec 8)

- Labor: $46,100
- Overhead (25%): $11,525
- Infra: $1,250
- Other: $0
- Contingency (15%): $8,831
- Month total: $67,706

# Project Total

- Labor: $322,700
- Overhead: $80,675
- Infra: $8,750
- Other: $12,515
- Contingency: $63,696
- Total: $488,336

Contingency is rounded to whole dollars. Month 2 and Month 3 both land on $0.50, so one rounds up and one rounds down to make the months add up to the total cost.
# 6.4 RACI Matrix

R = Responsible, A = Accountable, C = Consulted, I = Informed. One person is accountable for each task. Where a role is listed as Accountable and Responsible, that person does the work and answers for it.
# Requirements and documentation

- Accountable: Product Owner
- Responsible: Project Manager
- Consulted: Solutions Architect, UX Designer, Backend/API, QA
- Informed: Web App, Mobile App, Mapping & Location, Payment Integration, DevOps

# WBS and scheduling

- Accountable and Responsible: Project Manager
- Consulted: Solutions Architect, Backend/API, Web App, Mobile App, Mapping & Location, Payment Integration, QA
- Informed: Product Owner, UX Designer, DevOps

# Architecture and technical design

- Accountable and Responsible: Solutions Architect
- Consulted: Product Owner, UX Designer, Backend/API, Web App, Mobile App, Mapping & Location, Payment Integration, DevOps
- Informed: Project Manager, QA

# UX and UI design

- Accountable and Responsible: UX Designer
- Consulted: Product Owner, Web App, Mobile App, QA
- Informed: Project Manager, Solutions Architect, Backend/API, Mapping & Location, Payment Integration, DevOps

# Backend: authentication and database

- Accountable: Solutions Architect
- Responsible: Backend/API
- Consulted: Web App, Mobile App, DevOps, QA
- Informed: Project Manager, Product Owner, UX Designer, Mapping & Location, Payment Integration

# Frontend: driver app

- Accountable: Product Owner
- Responsible: Web App, Mobile App
- Consulted: Solutions Architect, UX Designer, Backend/API, Mapping & Location, Payment Integration, QA
- Informed: Project Manager, DevOps

# Payment integration

- Accountable: Solutions Architect
- Responsible: Payment Integration
- Consulted: Product Owner, UX Designer, Backend/API, Web App, Mobile App, DevOps, QA
- Informed: Project Manager, Mapping & Location

# Mapping integration

- Accountable: Solutions Architect
- Responsible: Mapping & Location
- Consulted: Product Owner, UX Designer, Backend/API, Web App, Mobile App, QA
- Informed: Project Manager, Payment Integration, DevOps

# Operator dashboard

- Accountable: Product Owner
- Responsible: Backend/API, Web App
- Consulted: Solutions Architect, UX Designer, Payment Integration, QA
- Informed: Project Manager, Mobile App, Mapping & Location, DevOps

# Notifications

- Accountable: Product Owner
- Responsible: Backend/API, Mobile App
- Consulted: Solutions Architect, UX Designer, DevOps, QA
- Informed: Project Manager, Web App, Mapping & Location, Payment Integration

# QA testing

- Accountable and Responsible: QA
- Consulted: Product Owner, Solutions Architect, Backend/API, Web App, Mobile App, Mapping & Location, Payment Integration, DevOps
- Informed: Project Manager, UX Designer

# Deployment and release

- Accountable and Responsible: DevOps
- Consulted: Project Manager, Solutions Architect, Backend/API, QA
- Informed: Product Owner, UX Designer, Web App, Mobile App, Mapping & Location, Payment Integration

# Sprint planning and backlog upkeep
- Accountable: Product Owner
- Responsible: Project Manager
- Consulted: Solutions Architect, UX Designer, Backend/API, Web App, Mobile App, Mapping & Location, Payment Integration, QA
- Informed: DevOps
# Cloud environments and CI/CD setup
- Accountable and Responsible: DevOps
- Consulted: Solutions Architect, Backend/API, QA
- Informed: Project Manager, Product Owner, UX Designer, Web App, Mobile App, Mapping & Location, Payment Integration