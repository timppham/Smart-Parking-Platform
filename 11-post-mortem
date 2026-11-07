# Post-Mortem: The HealthCare.gov Launch (October 2013)
Course: CIS 4374


# 1. What It Was

HealthCare.gov is a federally run website that allows people in most states to shop for and compare health insurance through the Affordable Care Act. The project was run by the Centers for Medicare and Medicaid Services (CMS). It was developed by CGI Federal who were the lead developer for the Federally Facilitated Marketplace. QSSI developed the data services hub, identity management and testing and support. The site went live on 1 October 2013.

# 2. What Happened

- The site went live on October 1, 2013 and failed under real use. Visitors hit crashes, long waits, and errors when they tried to create accounts and enroll
- According to the GAO, the site was down an estimated 60% of the time for a few weeks in October 2013
- Contractors told Congress that end-to-end testing lasted only about two weeks before launch
- About two weeks before launch, CMS turned off the anonymous "window shopping" feature, so every visitor had to create an account and get an eligibility result before comparing plans. QSSI said this added load to the identity management tool and may have contributed to early crashes
- Enrollment data sent to insurers (the 834 forms) was often wrong, which caused problems after a person had already enrolled
- On October 23, the White House announced teams of technology experts from insurers and CMS to work on the faulty forms
- The administration set a goal of November 30, 2013 for the site to work for the vast majority of users

# 3. What Went Wrong

Planning and oversight
- The GAO found CMS built the site without effective planning or oversight, which led to cost overruns, schedule errors, and delayed functionality
- CMS did not make sure schedules were well built, effort estimates were accurate, or required milestone reviews happened
- No senior CMS executive was named as the point person for integrating the system's pieces
- The HHS chief information officer said he had limited input and that no one raised functionality concerns at monthly meetings

Requirements
- The GAO reviewed 37 requirements for eligibility and enrollment. Nine were approved before development, eight were approved after they were sent to development, and 20 were never approved
- None of the 67 data services hub requirements the GAO reviewed were approved
- Requirements kept changing and communication was poor. Officials said they were rushing to meet the deadline

Testing
- End-to-end testing was never completed before launch
- Integration testing with insurers was still incomplete two months before launch
- Some defects found in testing were not fixed
- A code assessment ordered by CMS in September 2013 found 45 critical and 324 serious coding flaws in the marketplace system
- Each contractor said its own component did well in individual testing. The full system performed badly once it was put together

Capacity and the launch decision
- CMS underestimated how many users would arrive and planned for fewer than the site needed to handle
- CMS knew about problems before deployment and launched anyway to meet the deadline
- Both contractors said they did not recommend delaying the launch. CMS made the final call

Security
- The GAO also found weak security practices, including no requirement for strong passwords and inconsistent software patching

Contract management
- CMS paid $12.5 million under the contract and withheld $267,000, under 2% of the total fee, so the contractor faced little penalty
- The HHS inspector general reported about 60 contracts with an original lifetime value of $1.7 billion. Twenty had already exceeded their estimates. About $800 million was obligated and $500 million paid to contractors as of February 2014

# 4. What Went Right (Recovery)

- A dedicated fix effort ran daily bug fixes and brought in outside technology experts
- By the November 30 goal, the administration reported the site could handle 50,000 users at once, about 800,000 per day, with uptime above 95%, and that hundreds of software bugs had been fixed. Capacity had doubled
- Some problems remained: back-end functions tied to insurers, including payments to insurers, were still being built or repaired, and enrollment data errors were still being corrected
- HHS agreed with all of the GAO's findings, and CMS began corrective action and reevaluated its development schedules

Note: the recovery figures were reported by the administration itself and I did not find an independent check of them.

# 5. Root Causes

- Schedule was treated as fixed and quality was the thing that gave. The launch date did not move when the testing data said it should
- Nobody owned the whole system. Contractors owned pieces, CMS was the final decision maker, and integration had no named lead
- Requirements were unapproved and unstable, so there was nothing firm to test against
- Testing was left to the end, which is the one place a project has no room to absorb what it finds
- Status reporting did not carry bad news upward. Concerns raised by contractors did not become a decision to delay
- Contract oversight had little leverage when the work was late or defective

# 6. Lessons

- Test early and test the whole system. Component tests passing says little about the integrated product
- Approve requirements in writing before development, and get the business owner, the approval authority, and the contractor to sign, which is what the GAO recommended
- Name one accountable person for integration
- A launch date needs an exit: a go or no-go review based on test results, with the authority to say no
- Plan capacity from realistic demand, and test it with load
- Report honest status, including bad news, to the people who can act on it
- Tie payment to results so a contractor has a reason to fix problems

# 7. How This Applies to the Smart Parking Platform

- Our NFR1 (searches under 2 seconds) and NFR5 (availability refresh within 30 seconds) are performance requirements, and the lesson is to load test them before Nov 24, not on go-live
- QA is planned for Nov 3 to Nov 24 with a buffer week, and the same pressure that cut HealthCare.gov's testing is risk R-06 in our register
- Every use case has a Product Owner acceptance step, so requirements are approved before development
- The weekly risk review and the monthly city report are how bad news travels upward
- The PCI-DSS review is the equivalent of the security gaps the GAO found, and it should come before integration

# Sources

- [What went wrong with HealthCare.gov: 10 things to know (Becker's Hospital Review)](https://www.beckershospitalreview.com/healthcare-information-technology/what-went-wrong-with-healthcare-gov-10-things-to-know.html), summarizing the GAO report released in March 2014
- [Officials Spent Just Two Weeks Testing HealthCare.gov Prior to Launching It (Nextgov)](https://www.nextgov.com/cxo-briefing/2013/10/officials-spent-just-two-weeks-testing-healthcaregov-prior-launching-it/72608)
- [What went wrong with HealthCare.gov? (Nextgov)](https://nextgov.com/people/2013/10/what-went-wrong-with-healthcaregov/211515)
- [$500 million in HealthCare.gov spending explained (Nextgov)](https://www.nextgov.com/acquisition/2014/08/500-million-in-healthcaregov-spending-explained/255610), citing the HHS inspector general
- [White House meets goals for HealthCare.gov but more work ahead (Bangor Daily News)](https://www.bangordailynews.com/2013/12/01/news/white-house-meets-goals-for-healthcare-gov-but-more-work-ahead/)