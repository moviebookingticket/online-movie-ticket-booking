Functional Requirements — Online Movie Ticket Booking System

Functional requirements describe what the system must do — the specific features and behaviors it provides to customers and administrators. They are grouped below by module.


1. Account Management

FR-1 — Registration and Login
Priority: High | User Story: US-01
- The system shall allow customers to register using an email address or phone number.
- The system shall allow registered customers to log in and log out securely.
- The system shall validate credentials and reject weak passwords or invalid email formats.

FR-8 — Booking History
Priority: Medium | User Story: US-06
- The system shall allow customers to view a list of their past and upcoming bookings.
- The system shall show booking status (Confirmed, Cancelled, Completed) for each entry.


2. Movie Browsing

FR-2 — Browse Movies and Showtimes
Priority: High | User Story: US-02
- The system shall display a list of currently playing movies.
- The system shall allow filtering by date, genre, and cinema location.
- The system shall show showtime, language, and rating for each movie.

FR-12 — Ratings and Reviews
Priority: Low | User Story: US-08
- The system shall allow customers to rate a movie from 1 to 5 stars after watching it.
- The system shall allow customers to leave a written review tied to their booking.


3. Seat Selection and Booking

FR-3 — Seat Map Display
Priority: High | User Story: US-03
- The system shall display a real-time visual seat map for the selected showtime.
- The system shall distinguish available, booked, and selected seats.

FR-4 — Seat Selection and Locking
Priority: High | User Story: US-03
- The system shall allow customers to select one or more available seats.
- The system shall temporarily lock selected seats during checkout to prevent double-booking.
- The system shall release locked seats automatically if checkout is not completed within a set time limit.


4. Payment

FR-5 — Payment Processing
Priority: High | User Story: US-04
- The system shall process payments through a third-party payment gateway.
- The system shall support common payment methods, including card and digital wallet.

FR-6 — E-Ticket Generation
Priority: High | User Story: US-04
- The system shall generate an e-ticket upon successful payment.
- The e-ticket shall include a QR code, booking ID, movie name, and seat numbers.

FR-11 — Promo Codes
Priority: Low | User Story: US-07
- The system shall allow customers to enter a promo code at checkout.
- The system shall apply the discount if the code is valid and show an error if it is not.


5. Cancellation and Refunds

FR-7 — Cancel Booking
Priority: Medium | User Story: US-05
- The system shall allow customers to cancel a booking before the showtime.
- The system shall automatically initiate a refund request upon cancellation.


6. Admin Operations

FR-9 — Manage Movies and Showtimes
Priority: High | User Story: US-10
- The system shall allow administrators to add, edit, and remove movies.
- The system shall allow administrators to create and update showtimes.

FR-10 — Sales Reporting
Priority: High | User Story: US-10
- The system shall allow administrators to generate sales reports for a selected date range.
- The report shall include total revenue and number of transactions.


7. Notifications

FR-13 — Booking Notifications
Priority: Medium | User Story: US-09
- The system shall send a confirmation notification immediately after a successful booking.
- The system shall send a reminder notification before the showtime.


In Scope

- Customer registration, login, and profile management
- Browsing movies and showtimes with filters for date, genre, and cinema location
- Real-time seat map display and seat selection with temporary seat locking
- Online payment processing through a third-party payment gateway
- E-ticket generation with QR code
- Booking cancellation and refund initiation
- Customer booking history
- Admin management of movies, showtimes, and cinemas
- Admin sales reporting by date range
- Promo code application at checkout
- Movie ratings and reviews
- Booking confirmation and reminder notifications


Out of Scope

- Physical box-office or in-cinema kiosk booking integration
- Loyalty or rewards program beyond basic point tracking
- Third-party movie content licensing or streaming of movie content
- Multi-currency or multi-country tax handling
- Native mobile applications for iOS/Android — the system is web-based and mobile-responsive only
- Social media login integration, such as Google or Facebook OAuth
- Dynamic or surge pricing based on demand
- Group booking or corporate account management
- Actual coding, deployment, or hosting of the system — this course project covers planning, requirement analysis, design, and test case creation only, not implementation


Traceability Notes

- All requirements are traced to user stories in the Product Backlog (../planning/product-backlog.xlsx).
- FR-1 through FR-8 are targeted for Sprints 1–2, covering the customer-facing core flow.
- FR-9 and FR-10 are targeted for Sprint 3, covering the admin module.
- FR-11 through FR-13 are stretch goals for Sprint 4, pending capacity.
