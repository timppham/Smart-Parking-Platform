# User Stories

Each story maps to the use case with the same number.

US-01 (UC-01)
-  As a driver, I want to create an account using my email and password in order to reserve parking.
- Acceptance criteria:
  - Requirements for registration include a valid e-mail, password, and profile details
  - A verification email is sent after sign-up
  - The account is active only after the email is verified
  - Duplicate emails are rejected with a clear message

US-02 (UC-02)
- As a driver, operator or admin, I want to sign in with my email and password, so that I reach my own dashboard.
- Acceptance criteria:
  - Correct credentials open the right home screen for the role
  - Wrong credentials show an error without saying which field was wrong
  - Suspended accounts cannot sign in
  - Sign-in completes in under 2 seconds (NFR1)

US-03 (UC-03)
- As a user, I want to reset my password by email, so that I can get back into my account.
- Acceptance criteria:
  - A reset link is sent to the account email
  - The link expires after a set time and works once
  - The new password works for the next sign-in

US-04 (UC-04)
- As a driver, I want to search for parking by address, so that I can see garages near my destination.
- Acceptance criteria:
  - Entering an address returns nearby facilities
  - Results load in under 2 seconds (NFR1)
  - A search with no matches shows a clear empty message

US-05 (UC-05)
- As a driver, I want to see live availability on a map, so that I do not drive to a full garage.
- Acceptance criteria:
  - Each facility shows its current available count
  - Counts refresh within 30 seconds (NFR5)
  - Tapping a facility shows its details and rates
  - Manually entered counts are labeled as manual

US-06 (UC-06)
- As a driver, I want to reserve a spot for a date and time, so that a space is held for me.
- Acceptance criteria:
  - The system checks availability before confirming
  - The spot is held until payment is made
  - A spot cannot be booked twice for the same slot

US-07 (UC-07)
- As a driver, I want to cancel a reservation, so that I am not stuck with a booking I cannot use.
- Acceptance criteria:
  - Cancel is available only inside the cancellation period
  - The space is released right after cancelling
  - The driver gets a cancellation confirmation

US-08 (UC-08)
- As a driver, I want to pay for my reservation, so that my spot is confirmed.
- Acceptance criteria:
  - A saved or new payment method can be used
  - The reservation is confirmed only after the provider confirms the charge
  - Card data is handled to PCI-DSS standards
  - A failed payment shows a clear error and keeps the hold for a short time

US-09 (UC-09)
- As a driver, I want to see past reservations and receipts, so that I can track and expense my parking.
- Acceptance criteria:
  - My Reservations lists all past bookings
  - A receipt can be viewed and downloaded
  - Receipts show date, facility, and amount paid

US-10 (UC-10)
- As a driver, I want alerts about my reservation, so that I know when it is confirmed, expiring or cancelled.
- Acceptance criteria:
  - Confirmation, expiration warning and cancellation each send an alert
  - Alerts go by push or email based on my settings
  - Alerts arrive within a minute of the event

US-11 (UC-11)
- As a driver, I want turn-by-turn directions to my garage, so that I can find it easily.
- Acceptance criteria:
  - The Navigate button appears for confirmed reservations
  - The facility address opens in the mapping service
  - Directions are returned for the current location

US-12 (UC-12)
- As an operator, I want to change my hourly, daily and event rates, so that pricing matches demand.
- Acceptance criteria:
  - Rate changes save and apply to new reservations only
  - Existing reservations keep their original price
  - Rate changes are logged with the user and time

US-13 (UC-13)
- As an operator, I want to see live occupancy, so that I know how full my facility is.
- Acceptance criteria:
  - Occupied and available counts are shown for the facility
  - Zones or levels can be opened for detail
  - Counts refresh within 30 seconds (NFR5)

US-14 (UC-14)
- As an operator, I want occupancy reports for a date range, so that I can plan staffing and pricing.
- Acceptance criteria:
  - Any date range can be selected
  - Utilization trends are shown
  - The report can be exported

US-15 (UC-15)
- As an operator, I want to edit my facility listing, so that drivers see correct hours, amenities and capacity.
- Acceptance criteria:
  - Hours, amenities and capacity can be edited
  - A listing can be deactivated
  - Changes appear in driver search right after saving

US-16 (UC-16)
- As an admin, I want to issue a refund for a disputed or cancelled reservation, so that drivers are paid back.
- Acceptance criteria:
  - The refund request goes to the payment provider
  - The driver is refunded only after the provider confirms
  - The reservation status updates after the refund
  - Refunds are logged with the admin who issued them

US-17 (UC-17)
- As an admin, I want to suspend, restore and edit user accounts, so that I can handle misuse and fix mistakes.
- Acceptance criteria:
  - Users can be found by email or name
  - A suspended user cannot sign in until restored
  - Every change records the admin and the time

US-18 (UC-18)
- As an operator, I want to enter occupancy counts by hand when the feed is down, so that drivers still see reasonable availability.
- Acceptance criteria:
  - The dashboard shows a notice when the live feed is down
  - A manual count can be saved for the facility or a zone
  - Manual counts are labeled as manual to operators and drivers
  - Live data replaces the manual count when the feed returns