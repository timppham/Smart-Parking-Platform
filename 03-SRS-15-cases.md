Software Requirements Specification (SRS)
Project: Smart Parking Platform
Version: 0.1 (Draft)
Date: 09.10.2026

1. Introduction

1.1 Purpose
This SRS outlines the requirements for the Smart Parking Platform, which enables drivers to search, reserve, pay for parking, and navigate to their chosen parking spot. The operator can manage occupancy, price, and listing of his facility.

1.2 Scope
The platform comprises a web application and mobile applications (parking spot search, booking and payment, user profile, notification, and navigation handoff to the third party), an operator's dashboard (price management, occupancy monitoring, report generation, and listing management), and admin tools for account and refund management. It does not include any hardware integration for sensors or cameras to be installed in garages, construction and/or renovation of parking places, or even internal workings of the payment and mapping service providers. Only the integration of the platform with these services falls under the scope.

2. Overall Description

Actors: Car drivers, parking operators, system administrators, the payment provider, and the mapping/navigation service.
Environment: Web application and native mobile application (iOS and Android).
Constraints: Needs to interface with a third-party payment processing tool and a map/navigation API. Needs to be compliant with the city's parking guidelines and the PCI-DSS standards for payment transactions. Delivery must fit within the semester time-frame.
Assumptions: The actors have internet connection either via WiFi or mobile data. The garages will provide an occupation feed to the platform using a sensor, camera, or manual input from the operator.
3. Functional and Nonfunctional Requirement
Functional 
- The system shall let drivers to register and login securely
- The system shall let drivers to reset their passwords
- The system shall let drivers search for parking based on their destination
Non-Functional
- The system shall provide every instructions to get to the parking space ( turn-by-turn navigation)
- The system shall let operators set and adjust pricing 
4. User Case
UC-01: Registration of User Account
Actor: Driver
Preconditions: User has a valid email address
Steps: The user clicks on "Create Account" and enters the details regarding the email address, password and basic profile information. The system validates the above information by sending out an email for validation purposes.
Postconditions: An active account is created.

UC-02: Login
Actor: Driver / Operator / Admin
Preconditions: User has a valid account
Steps: The user enters his email and password. The credentials are verified, and he gets access to his dashboard.
Postconditions: The user is verified and gets access to the homepage.

UC-03: Password Reset
Actor: Driver / Operator / Admin
Preconditions: User forgot his password
Steps: The user clicks on "Forgot Password", enters his email associated with the account, and the link for changing password is sent by the system.
Postconditions: The password gets updated, and he can log in using the password.

UC-04: Search for Parking
Actor: Driver
Preconditions: User is logged in
Steps: Entering the address to the search field leads to the query among the nearest facilities, which results in returning the list.
Postconditions: Driver gets a list of nearby parking spots.

UC-05: See Live Availability
Actor: Driver
Preconditions: Driver has found a destination
Steps: Map shows destination and available facilities with their live availability numbers. Tapping on facility displays details.
Postconditions: Live availability of each nearby facility is shown.

UC-06: Reserve Parking Spot
Actor: Driver
Preconditions: Driver is logged in and has chosen a facility
Steps: Driver chooses a date and time slot; system verifies availability of a space and reserves it after confirmation from user until payment.
Postconditions: Reservation is made.

UC-07: Cancel Parking Spot Reservation
Actor: Driver
Preconditions: Driver has an active reservation within cancellation period
Steps: Driver opens the reservation and taps "Cancel" button. System confirms cancellation and frees the space.
Postconditions: Reservation is cancelled; space is released.

UC-08: Pay for Parking Spot Reservation
Actor: Driver, Payment Provider
Preconditions: Driver has an active parking spot reservation
Steps: Driver selects payment method, whether it's saved in app before or not. Request is sent to payment provider. After confirmation of charge, reservation is confirmed.
Postconditions: Parking spot reservation is paid and confirmed.

UC-09: View Reservation History and Receipts
Actor: Driver
Preconditions: Driver has at least one past reservation
Steps: Driver opens "My Reservations." System lists past bookings. Driver taps one to view or download the receipt.
Postconditions: Driver can view or export a receipt.

UC-10: Receive Notifications and Alerts
Actor: Driver
Preconditions: Driver has notifications enabled
Steps: Triggering event occurs, confirmation, expiration warning, or cancellation. System generates a notification and sends it by push alert or email.
Postconditions: Driver is informed of the relevant event.

UC-11: Get Navigation to Garage
Actor: Driver, Mapping Service
Preconditions: Driver has a confirmed reservation
Steps: Driver taps "Navigate." Facility address is sent to the mapping service, which returns turn-by-turn directions.
Postconditions: Driver is routed to the facility.

UC-12: Manage Parking Rates
Actor: Parking Operator
Preconditions: Operator is logged in and manages a facility
Steps: Operator opens facility settings and updates hourly, daily, or event pricing. System saves the change and applies new rates going forward.
Postconditions: Updated pricing is live for new reservations.

UC-13: Monitor Real-Time Occupancy
Actor: Parking Operator
Preconditions: Facility is reporting live occupancy data
Steps: Operator opens the dashboard. Current occupied and available counts display, with the option to drill into specific zones or levels.
Postconditions: Operator has current visibility into facility occupancy.

UC-14: View Occupancy Reports and Analytics
Actor: Parking Operator
Preconditions: Facility has historical occupancy and reservation data
Steps: Operator selects a date range. System aggregates utilization data into trends and exportable reports.
Postconditions: Operator has a utilization report for the selected period.

UC-15: Manage Facility Listing
Actor: Parking Operator
Preconditions: Operator is signed in
Steps: Operator accesses "My Facility" and makes changes to hours, amenities, or capacity or deactivates the listing.
Postconditions: The listing will be updated to reflect those changes.

UC-16: Initiate Refund
Actor: System Administrator, Payment Provider
Preconditions: There is a disputed or cancelled reservation
Steps: Admin views the reservation and clicks "Issue Refund". The request is then sent to the payment provider. After the payment provider confirms, the driver gets his refund.
Postconditions: Driver is issued the refund; status of reservation is updated.