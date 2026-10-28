---
title: "User Stories and Tasks"
permalink: /prp370/user-stories/
---

# 2. User Stories and Tasks

A user story describes a feature from the perspective of the person who
needs it. The FUNDI board contains story cards for customer, fundi,
administrator, and developer needs. The examples below preserve the
meaning of the board's stories and decompose them into tasks and
acceptance criteria.

## 2.1 Example story breakdowns

### US-01 --- Homeowner registration and login

**Story:** As a homeowner, I want to register and log in, so that I can
browse and book fundis.

**Acceptance criteria** - A new user can submit valid registration
details. - Invalid or duplicate details produce a clear error. - A
registered user can log in with valid credentials. - Invalid credentials
do not grant access. - Authenticated routes require a valid
session/token. - Passwords are never displayed or returned as plain
text.

**Tasks** 1. Define the user fields and validation rules. 2. Implement
registration and login endpoints. 3. Hash passwords securely and
configure authentication. 4. Connect the React forms to the API. 5.
Display validation and server errors. 6. Protect routes and test
successful and unsuccessful login cases.

### US-02 --- Fundi trade account

**Story:** As a fundi, I want to register for a trade account, so that I
can set up my storefront.

**Acceptance criteria** - A user can choose/register as a fundi where
permitted. - Required profile fields are validated. - The fundi account
is linked to the correct user. - The account cannot falsely claim
verified status before approval. - The fundi can reach the appropriate
dashboard after login.

**Tasks** 1. Define the fundi profile fields and relationship to the
user. 2. Implement the backend registration/profile workflow. 3. Add the
frontend registration fields. 4. Apply role checks to fundi-only routes.
5. Test valid, invalid, and duplicate account scenarios.

### US-03 --- Verification review and trust badge

**Story:** As an administrator, I want to review submitted ID and
qualification documents, so that I can approve or reject fundis.

**Acceptance criteria** - Verification documents are associated with the
correct fundi. - Only authorized administrators can review
submissions. - An administrator can approve or reject a submission. -
The status and review outcome are persisted. - The verified badge
appears only after approval. - Sensitive verification documents are not
publicly accessible.

**Tasks** 1. Define verification statuses and data model. 2. Configure
private document storage and access rules. 3. Build the fundi
document-submission flow. 4. Build the administrator review workflow. 5.
Enforce backend authorization. 6. Test approved, rejected, pending, and
unauthorized access cases.

### US-04 --- Product and material listings

**Story:** As a fundi, I want to add products/materials to my
storefront, so that customers can purchase them.

**Acceptance criteria** - A fundi can create a listing with required
details. - Price, description, category, and image requirements are
validated. - A fundi can edit or remove their own listings. - Customers
can view listing details and photos. - A fundi cannot edit another
fundi's listings.

**Tasks** 1. Define product fields and persistence. 2. Implement
create/read/update/delete endpoints. 3. Add listing forms and product
cards. 4. Validate price, category, and image inputs. 5. Apply ownership
and role checks. 6. Test listing creation, editing, removal, and
display.

### US-05 --- Transparent labour and callout rates

**Story:** As a fundi, I want to set my callout fee and hourly/job rate,
so that customers see transparent pricing upfront.

**Acceptance criteria** - The fundi can save supported rate types. -
Values are validated and displayed consistently. - Customers can see
applicable labour/callout pricing before booking. - Missing or
negotiable prices are clearly identified rather than misleadingly shown
as zero.

**Tasks** 1. Agree the supported rate model and currency format. 2. Add
persistence and API operations for rates. 3. Build fundi rate-management
UI. 4. Display pricing on fundi profiles and booking pages. 5. Test
valid values, invalid values, and missing prices.

### US-06 --- Search and discovery

**Story:** As a customer, I want to search for verified fundis by trade
category and location, so that I find someone nearby.

**Acceptance criteria** - Search results match the selected
trade/category. - Location criteria are applied when provided. -
Verification status is represented accurately. - Empty results produce a
helpful message. - Search inputs do not cause application errors.

**Tasks** 1. Define searchable fields and filters. 2. Implement backend
query/filter logic. 3. Add search and filter controls. 4. Display result
cards and empty states. 5. Test category, location, and no-result cases.

### US-07 --- Booking management

**Story:** As a fundi, I want to accept, reschedule, or decline
bookings, so that I control my job calendar.

**Acceptance criteria** - A fundi can view only bookings associated with
their profile. - Valid requested bookings can be accepted or declined. -
Rescheduling requires a valid future date/time. - Status changes are
persisted and visible to the customer. - Unauthorized users cannot
change another fundi's booking.

**Tasks** 1. Define the booking status lifecycle and transition rules.
2. Implement booking queries and status-update endpoints. 3. Build the
fundi bookings interface. 4. Add date/time validation and error
messages. 5. Ensure ownership and role checks. 6. Test each permitted
transition and forbidden transition.

### US-08 --- Reviews after completed work

**Story:** As a customer, I want to rate and review a fundi after a
completed job, so that other customers can trust the storefront.

**Acceptance criteria** - Only an eligible customer can review their
booking. - The rating is within the allowed range. - The review is
associated with the correct booking and fundi. - Duplicate reviews for
the same booking are prevented if the product rule is one review per
booking. - Reviews are displayed on the appropriate storefront.

**Tasks** 1. Define review fields and constraints. 2. Implement
create/read review endpoints. 3. Validate rating and comment length. 4.
Link the review to booking, customer, and fundi. 5. Add review form and
display components. 6. Test permissions, invalid ratings, and duplicate
submissions.

### US-09 --- Secure checkout and payment

**Story:** As a customer, I want a secure one-step checkout, so that I
can pay for my order confidently.

**Acceptance criteria** - The customer sees a clear order summary before
confirming. - The server calculates authoritative totals. - Payment
status is recorded and can be reconciled. - Sensitive payment data is
not stored unnecessarily. - Failed or cancelled payment attempts are
handled safely.

**Tasks** 1. Define checkout and order states. 2. Integrate the selected
payment provider in a test environment. 3. Implement server-side total
calculation. 4. Persist order and payment references. 5. Build checkout
confirmation/error screens. 6. Test success, failure, cancellation, and
duplicate-callback scenarios.

**Scope note:** The Trello board contains a payment/escrow story. Do not
claim escrow or live payment processing is complete without working
integration and test evidence.

### US-10 --- Booking-status notifications

**Story:** As a user, I want email/in-app notifications for booking
status changes, so that I stay informed.

**Acceptance criteria** - A notification is triggered for agreed
booking-status changes. - The recipient is the correct customer or
fundi. - Notification failure does not corrupt the booking state. - The
notification content does not expose another user's private information.

**Tasks** 1. Identify the events that trigger notifications. 2. Define
notification storage or delivery mechanism. 3. Implement event handling
and message templates. 4. Connect email/in-app delivery where
configured. 5. Test delivery, failure handling, and recipient selection.

## 2.2 Additional stories in the product scope

The board also includes stories for: - managing a user profile; -
administrator role-based access control; - fundi verification status and
storefront customization; - editing/removing and categorizing product
listings; - filtering/sorting results by rating, price, or distance; -
adding materials to a cart; - combining materials and labour in
checkout; - buying materials without booking a job; - marking a job
completed; - payment protection, commission, subscriptions, and booking
fees; - reading reviews and responding to reviews; - administrator
dashboards, fraud management, and revenue reports; - fundi notifications
for new orders/bookings; - frontend, backend, database, and hosting
foundations.

## 2.3 Reflection --- User Stories and Tasks

**Draft reflection --- personalize this to match your real experience:**

Breaking broad themes into user stories makes the work easier to
discuss, estimate, assign, and test. For example, "booking management"
is not one task: it includes status rules, ownership checks, date
validation, API operations, interface feedback, and tests. Writing
acceptance criteria also helps expose edge cases before implementation.
For FundiShop, security-related acceptance criteria are especially
important because the application handles accounts, bookings, reviews,
and proposed verification documents. A practical improvement is to add
explicit acceptance criteria and subtasks to the Trello cards, then link
each completed story to a commit, test result, or demonstration.

**Evidence to attach:** screenshots of selected Trello story cards with
acceptance criteria/checklists, plus test evidence for at least one
story you personally implemented.

------------------------------------------------------------------------

---
**FundiShop PRP370 Portfolio:** [Overview](../) · [Team Charter](team-charter/) · [User Stories](user-stories/) · [Product Backlog](product-backlog/) · [Sprint Backlog](sprint-backlog/) · [Agile Logbook](agile-logbook/) · [Reflection & Evidence](reflection-evidence/)
---
