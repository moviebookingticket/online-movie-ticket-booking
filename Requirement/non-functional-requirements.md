Non-Functional Requirements — Online Movie Ticket Booking System

Non-functional requirements describe how well the system must perform, rather than what it does. They cover quality attributes such as performance, security, and usability, organized below by category.


1. Performance

NFR-1 — Seat Map Responsiveness
- The seat map shall refresh to reflect newly booked seats within 5 seconds.
- This ensures customers never attempt to book a seat that was just taken by someone else.


2. Security

NFR-2 — Payment Data Protection
- All payment data shall be transmitted using TLS/SSL encryption.
- The application server shall not store raw payment card data.
- The system shall align with PCI-DSS security standards for handling payment information.


3. Usability

NFR-3 — Ease of Use
- A first-time user shall be able to complete a full booking in 5 minutes or less, without assistance.
- The interface shall use clear labels and guided steps: browse, select seat, pay, confirm.


4. Availability

NFR-4 — System Uptime
- The system shall maintain 99.5% uptime during cinema operating hours.
- Planned maintenance shall be scheduled outside peak booking hours.


5. Scalability

NFR-5 — Concurrent User Support
- The system shall support at least 500 concurrent users during peak periods, such as new movie releases or holiday weekends.
- Performance shall not degrade significantly under this load.


6. Compatibility

NFR-6 — Cross-Platform Access
- The system shall be accessible via modern web browsers, including Chrome, Safari, Firefox, and Edge (last 2 versions).
- The interface shall be responsive and usable on mobile devices without a dedicated app.


7. Data Integrity

NFR-7 — Booking Accuracy
- The system shall prevent double-booking of the same seat under concurrent requests.
- Seat locks shall be enforced consistently across simultaneous sessions.


8. Maintainability

NFR-8 — Code Quality and Testability
- The codebase shall follow a documented coding standard.
- Core booking logic shall be covered by automated tests at 70% coverage or higher, as a target for the future coding phase.


Verification Summary

NFR-1 and NFR-7 are verified by integration test cases covering seat locking and concurrent booking.
NFR-2 is verified by design review, since it is not executable in this documentation-only phase.
NFR-3 is verified by User Acceptance Testing (UAT).
NFR-4 and NFR-5 are out of scope for this course project and remain at the planning level only.
NFR-6 is verified by design review of the responsive mockups.
