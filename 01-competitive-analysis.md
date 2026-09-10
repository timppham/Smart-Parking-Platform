# Research: Competitive Analysis

Before Software Corp designs anything new, it's worth looking at who already owns this space. This parking technology market splits into two camps that rarely overlap: apps built for drivers looking for a spot, and platforms built for the operators running the garages. Our system needs to serve both sides at once, which is already a gap most competitors leave open.

## Driver-Facing Reservation and Payment Apps

These products let a driver find, book, and pay for a spot before they arrive. Most work off a marketplace model: they don't own garages, they resell inventory from lot operators and take a cut.

| Product | Model | Strengths | Weaknesses |
|---|---|---|---|
| SpotHero | Marketplace platform for privately-owned parking spaces | Wide-range network in big American cities, reservation guarantee, CarPlay compatibility, business expense management | Does not include street or pay-to-park spots, coverage is sparse in smaller cities, cost is determined solely by partner garages |
| ParkMobile | Zone payment for street meters | Quick access to street parking, quick zone lookup | Not level-based reservation, no real-time occupancy information about a particular space, bad for garages |

## Operator-Facing Management Platforms

On the other side of the transaction, operators need tools to price, monitor, and enforce their own lots. This is a separate market with its own vendors, and drivers never see most of it.

| Product | Model | Strengths | Weaknesses |
|---|---|---|---|
| Metropolis | Vision-based, gate-less entry with automated billing for operators | Large footprint with many locations, license plate recognition to eliminate tickets and kiosks, good for mixed-use and multifamily developments | Highly dependent on infrastructure, system is based on operator hardware and site takeover rather than on booking by the driver |
| Passport | Curb and enforcement management for cities and agencies | Provides enforcement, permitting, and analytics services to city clients, strong benchmarking and reporting tools | Targeted at municipal governments and not private garage operators, not a consumer-facing reservation product |

## Gaps and Differentiation Opportunities

A few patterns show up once you line these products up side by side.

The driver side and the operator side are split across different vendors. A driver books through SpotHero, but the garage behind that booking is likely running on its own separate management system. Nobody in this research owns both ends of that transaction in one product built for a single mid-size garage operator.

Reservation apps rarely show true real-time occupancy. Most marketplace apps sell against an operator's estimated inventory rather than a live sensor or camera feed, so a spot can still show as available after it's taken.

Metered, on-street tools and off-street garage tools don't talk to each other. A driver comparing a garage reservation against nearby street parking has to check two different apps.

That gap is where this project can differentiate. Rather than being another marketplace reselling someone else's garage inventory, the platform being built here can pair a driver-facing app with a genuine operator dashboard on the same backend, so occupancy data shown to a driver comes straight from the same system the operator is using to manage pricing and reporting. That single-source-of-truth approach is the core positioning the Vision and Scope section builds on.
