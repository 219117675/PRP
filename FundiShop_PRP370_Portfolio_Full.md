# FundiShop --- PRP370 Agile Portfolio of Evidence

**Student:** Christian Hakizimana\
**Programme:** Diploma in Information and Communication Technology\
**Subject:** PRP370 --- Project Presentation 3\
**Portfolio purpose:** Evidence of Agile planning, user-story
decomposition, product and sprint planning, and reflective learning.\
**Project management board:** [FUNDI Trello
board](https://trello.com/b/iLYYDYvL/fundi)\
**Portfolio website:** [Christian Hakizimana --- GitHub
Pages](https://219117675.github.io/Christian_Hakizimana.github.io/)

> **Evidence integrity note:** This portfolio distinguishes planned work
> from verified implementation. The connected Trello board currently
> contains 54 cards, all in a single **Backlog** list, with no cards
> marked complete. The sprint dates below come from the project-plan
> document and are planned milestones, not proof that each sprint was
> completed. Replace or supplement this portfolio with screenshots,
> commits, test results, meeting records, and accurate personal
> reflections before submitting.

------------------------------------------------------------------------

## Project overview

### Product vision

FundiShop is planned as a digital marketplace that brings homeowners and
renters together with trade professionals ("fundis") and makes it easier
to find services, compare transparent labour/callout pricing, and source
materials. The business concept emphasizes trust, verified trade
accounts, storefronts, booking workflows, product listings, ratings and
reviews, and an integrated customer journey.

The pitch identifies the core problem as the difficulty of finding
trustworthy tradespeople, fragmented access to labour and materials, and
unclear pricing. Its proposed solution is a platform where customers can
discover reviewed trades, book services with clearer labour pricing,
source materials, and leave feedback.

### Intended users

-   **Homeowners and renters:** find tradespeople, compare options, book
    jobs, purchase materials, and review completed work.
-   **Fundis / trade professionals:** register, complete verification,
    manage a storefront, list services/materials, set rates, and respond
    to bookings.
-   **Administrators:** review verification documents, manage platform
    trust and safety, and monitor users and transactions.
-   **Potential later users:** landlords, property managers, small
    businesses, and facilities teams.

### Proposed technical direction

The architecture presentation describes a web presentation layer, a Java
Spring Boot REST application layer, a relational database (PostgreSQL or
MySQL), and external integrations such as payments, email/SMS, maps, and
cloud storage. The actual implementation should be documented separately
from the proposed architecture. In the current development context,
FundiShop has a React frontend and Spring Boot backend; the precise
deployed database, payment integration, and production hosting should be
confirmed with implementation evidence before claiming they are
complete.

### Current evidence snapshot

  -----------------------------------------------------------------------
  Evidence source         What it supports        What it does not prove
                                                  by itself
  ----------------------- ----------------------- -----------------------
  FundiShop pitch         Problem, proposed       That all proposed
  presentation            solution, target users, features are
                          value proposition,      implemented
                          business model          

  Solution architecture   Proposed modules,       That integrations or
  presentation            technology direction,   production deployment
                          data entities,          are complete
                          integrations, and flow  

  FUNDI Trello board      54 backlog cards        Completion of sprints,
                          grouped around 13 work  delivery of stories, or
                          themes; team assignment meetings not recorded
                          on theme cards; board   in the board
                          activity dates          

  Existing application    Must be added as direct Not included in the
  code and tests          evidence: screenshots,  Trello board snapshot
                          Git commits, test       alone
                          output, or a demo       
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 1. Agile Team Charter

## 1.1 Purpose and shared goal

The team's shared goal is to plan and build a useful FundiShop minimum
viable product (MVP) that helps customers discover trade professionals
and supports a trustworthy service-booking experience. The work is
organized into feature areas covering planning and architecture,
authentication, trade verification, storefronts, product/material
listings, transparent labour pricing, search, checkout, booking,
payments, reviews, administration, notifications, and platform
foundations.

## 1.2 Team members and roles

The Trello planning cards show these four members assigned to the
feature-theme cards:

  -----------------------------------------------------------------------
  Team member             Suggested working       Confirmation needed
                          responsibility          
  ----------------------- ----------------------- -----------------------
  Christian Hakizimana    Coordination,           Confirm the exact role
                          full-stack              agreed by the team
                          implementation          
                          contribution,           
                          integration and         
                          portfolio evidence      

  Kabelo Nimrod Moloko    Feature implementation  Confirm specific
                          and review contribution ownership

  Muhammad Siddeeq Rabin  Feature implementation  Confirm specific
                          and review contribution ownership

  Lisakhanya Mpahla       Feature implementation  Confirm specific
                          and review contribution ownership
  -----------------------------------------------------------------------

**Important:** The board shows membership on theme cards; it does not
establish formal job titles or the exact division of development work.
Replace the suggested responsibilities above with the roles actually
agreed by the team.

## 1.3 Values and working agreements

These are proposed charter agreements to confirm with the team:

1.  **Customer value first:** prioritize work that makes the core
    discovery-to-booking journey useful and understandable.
2.  **Transparency:** keep Trello cards current and clearly distinguish
    To Do, In Progress, Blocked, and Done work.
3.  **Shared ownership:** discuss dependencies and review changes that
    affect another feature or the API contract.
4.  **Small, testable increments:** break large feature themes into user
    stories and actionable development tasks.
5.  **Quality and security:** validate inputs, protect account
    information, enforce role-based access, and test critical workflows.
6.  **Respectful communication:** raise blockers early, listen to
    alternatives, and agree on decisions rather than making assumptions.
7.  **Evidence-based completion:** mark a card Done only when its
    acceptance criteria are met and evidence is available.
8.  **Retrospective improvement:** record what worked, what did not, and
    one practical improvement for the next iteration.

## 1.4 Communication and decision-making

**Proposed working agreement --- confirm before submission:**

-   Use Trello as the shared view of backlog and task status.
-   Use the team's agreed communication channel for questions and
    blockers.
-   At a planning session, agree on a sprint goal, select work according
    to priority and capacity, and identify dependencies.
-   During a sprint, communicate blockers as soon as they appear.
-   Review completed work against acceptance criteria and demonstrate it
    where possible.
-   At the end of the sprint, record the result and a short
    retrospective.
-   Resolve technical disagreements by comparing requirements,
    maintainability, security, and implementation effort.

Do not add a meeting cadence, response-time promise, or decision rule
here unless the team has actually agreed to it.

## 1.5 Definition of Ready

A story is ready to enter a sprint when:

-   it describes a user need and the expected value;
-   acceptance criteria are understandable and testable;
-   major dependencies are identified;
-   the team has a reasonable implementation approach;
-   required data/API/UI changes are understood; and
-   the work is small enough to complete and review within the sprint.

## 1.6 Definition of Done

A story can be considered Done only when:

-   the acceptance criteria pass;
-   the implementation is integrated into the agreed branch;
-   relevant validation and error handling are present;
-   security and role permissions have been considered;
-   tests or a repeatable manual test have been run;
-   no known critical defect prevents the intended workflow;
-   the team can demonstrate the feature; and
-   the Trello card and evidence links are updated.

## 1.7 Reflection --- Agile Team Charter

**Draft reflection --- personalize this to match your real experience:**

Creating a team charter makes the team's expectations visible instead of
leaving them implicit. FundiShop has several connected modules, so
unclear ownership or inconsistent communication can cause integration
problems---for example, when a booking page, backend endpoint, and
database model do not agree. A shared Definition of Ready helps prevent
poorly understood stories from entering a sprint, while a Definition of
Done prevents a feature from being treated as complete merely because
code has been written. The next improvement is to confirm the proposed
working agreements with all team members, record the agreed roles and
communication arrangements, and retain a dated screenshot or meeting
note as evidence.

**Evidence to attach:** a screenshot of the agreed charter, team roles
confirmed by the group, and a Trello board/member view. Do not present
proposed agreements as already agreed until the team confirms them.

------------------------------------------------------------------------

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

# 3. Product Backlog

The product backlog is the ordered list of product work. The FUNDI
Trello board has 13 feature-theme cards and 41 associated user
stories/technical stories, for 54 cards in total. All 54 cards are
currently in the **Backlog** list in the connected board snapshot and
none are marked complete. The priority order below is a recommended MVP
sequence based on dependencies and customer value; it should be
confirmed against the team's agreed MoSCoW priorities.

## 3.1 Recommended prioritized backlog

  -------------------------------------------------------------------------------------------
  Priority       ID / theme     Backlog item     Value / reason    Suggested acceptance
                                                                   evidence
  -------------- -------------- ---------------- ----------------- --------------------------
  P0 --- Must    S1             Planning,        Establishes the   Approved architecture/ERD,
                                architecture,    shared technical  repository, board and
                                backlog, ERD,    and delivery      setup notes
                                GitHub, setup    foundation        

  P0 --- Must    S2             User accounts    Enables protected Registration/login tests
                                and              customer and      and role-protection
                                authentication   fundi workflows   evidence

  P0 --- Must    S3             Trade            Supports trust    Verification states, admin
                                verification and and identity of   review and storefront
                                storefront setup service providers evidence

  P0 --- Must    S4             Product and      Makes the         Create/view/edit listing
                                material         marketplace       test evidence
                                listings         useful beyond a   
                                                 directory         

  P0 --- Must    S5             Labour and       Supports          Rate saved and visible
                                callout rates    transparent job   before booking
                                                 pricing           

  P0 --- Must    S6             Search and       Helps customers   Search/filter tests and
                                discovery        find suitable     result screenshots
                                                 fundis            

  P0 --- Must    S8             Booking and job  Delivers the core Booking lifecycle tests
                                scheduling       service-booking   
                                                 workflow          

  P0 --- Must    S10            Ratings and      Supports customer Review permission and
                                reviews          confidence after  display tests
                                                 a job             

  P1 --- Should  S7             Cart and         Combines          Cart totals and checkout
                                integrated       materials and     flow tests
                                checkout         service selection 

  P1 --- Should  S9             Payments and     Supports          Payment-provider sandbox
                                escrow           transaction       evidence; escrow only if
                                                 completion and    genuinely implemented
                                                 protection        

  P1 --- Should  S12            Notifications    Keeps users       Notification trigger and
                                                 informed about    recipient tests
                                                 booking/order     
                                                 changes           

  P1 --- Should  S11            Admin dashboard  Supports          Admin authorization and
                                and platform     oversight,        dashboard evidence
                                management       safety, and       
                                                 operations        

  P0 --- Must    S13            Non-functional   Security,         Test results, security
                                requirements /   reliability,      checks,
                                platform         persistence,      configuration/deployment
                                foundation       responsiveness,   evidence
                                                 and deployment    
  -------------------------------------------------------------------------------------------

**Ordering note:** S13 is cross-cutting and should not wait until the
end. Security, validation, data integrity, and responsive behavior must
be addressed throughout development. The numbering above follows the
board's theme identifiers; the priority labels are a recommended
planning order, not a statement of the board's current status.

## 3.2 Backlog refinement rules

For each backlog item, record: - story ID and title; - user/business
value; - priority; - acceptance criteria; - estimate or relative size; -
dependencies; - owner(s); - status; - implementation evidence; and - any
deferred scope decision.

Revisit the backlog when new risks, user feedback, or technical
dependencies emerge. If the team defers a feature, record the reason and
the release or sprint in which it may be reconsidered.

## 3.3 Proposed MVP boundary

The project plan prioritizes Must Have stories for the MVP and defers
selected Should Have/Could Have items to a later release. Potential
later-release items identified in the plan include advanced profile
management, featured placement, subscriptions, seasonal pricing, review
replies, and advanced reporting. Confirm the final scope with the team
and lecturer before presenting this as the final agreed MVP boundary.

## 3.4 Reflection --- Product Backlog

**Draft reflection --- personalize this to match your real experience:**

The backlog makes the breadth of FundiShop visible and helps the team
separate the core marketplace journey from business features that can be
delivered later. Authentication, fundi trust, discovery, pricing,
bookings, and reviews form a logical foundation because other features
depend on them. Payments, notifications, and administration also matter,
but they introduce integration and security work that needs explicit
planning. The current Trello snapshot has all cards in one Backlog list,
so it does not communicate priority or progress clearly. The next
improvement is to agree on priority and dependencies, add estimates and
acceptance criteria, and introduce workflow states that show what is
ready, in progress, blocked, and done.

**Evidence to attach:** a screenshot of the full backlog and
priority/labels, plus a short explanation of why the highest-priority
stories were selected.

------------------------------------------------------------------------

# 4. Sprint Backlog

A sprint backlog is the selected set of work and plan for achieving a
sprint goal. The project plan in the available FundiShop planning
document lists the following intended schedule. This section records the
plan, not verified completion. The Trello board currently does not have
separate sprint lists or completed cards, so actual sprint outcomes must
be added from the team's real records.

## 4.1 Planned sprint schedule

  -----------------------------------------------------------------------
  Iteration         Planned dates     Focus in the      Goal / candidate
                                      project plan      outcome
  ----------------- ----------------- ----------------- -----------------
  Sprint 0          23--24 July 2026  Planning,         Agree the project
                                      architecture,     foundation and
                                      backlog, ERD,     prepare work for
                                      GitHub, setup     implementation

  Sprint 1          27 July--7 August Authentication,   Establish secure
                    2026              roles, fundi      accounts and
                                      registration,     role-aware access
                                      verification      

  Sprint 2          10--21 August     Storefronts,      Let fundis
                    2026              verification,     present profiles,
                                      product listings, listings, and
                                      labour pricing    rates

  Sprint 3          24 August--4      Search, cart,     Build the
                    September 2026    checkout          customer
                                                        discovery and
                                                        purchasing flow

  Sprint 4          7--18 September   Booking, payments Support booking
                    2026                                and planned
                                                        transaction
                                                        workflows

  Sprint 5          21 September--2   Reviews, admin    Add trust
                    October 2026      dashboard,        feedback and
                                      notifications     operational
                                                        support

  Sprint 6          5--16 October     Testing,          Stabilize the MVP
                    2026              security, bug     and prepare
                                      fixes,            evidence/demo
                                      documentation,    
                                      deployment        

  Presentation      20 October 2026   Final demo and    Demonstrate the
  milestone                           submission        available product
                                                        and submit
                                                        portfolio
                                                        evidence
  -----------------------------------------------------------------------

## 4.2 Sprint backlog template --- complete using actual records

Use this template for each sprint you can verify. Do not invent sprint
goals, capacity, completed work, blockers, or results.

### Sprint \[number\] --- \[actual dates\]

-   **Sprint goal:** \[the goal actually agreed by the team\]
-   **Selected stories:** \[Trello card titles/IDs\]
-   **Tasks and owners:** \[actual task split\]
-   **Dependencies/risks:** \[known dependencies\]
-   **Planned evidence:** \[commits, test output, screenshots, demo\]
-   **Outcome:** \[completed / partially completed / not completed,
    supported by evidence\]
-   **Scope changes:** \[what changed and why\]
-   **Blockers:** \[actual blockers\]
-   **Next action:** \[what the team agreed to do next\]

  -----------------------------------------------------------------------------------------------------
  Story/task       Owner          Acceptance     Status                    Evidence link
                                  criteria                                 
  ---------------- -------------- -------------- ------------------------- ----------------------------
  \[Story/task\]   \[Name\]       \[Testable     \[To Do/In                \[Commit/test/screenshot\]
                                  result\]       Progress/Blocked/Done\]   

  \[Story/task\]   \[Name\]       \[Testable     \[To Do/In                \[Commit/test/screenshot\]
                                  result\]       Progress/Blocked/Done\]   
  -----------------------------------------------------------------------------------------------------

## 4.3 Sprint selection example --- planning template only

**Example goal:** "Deliver a secure account flow with customer/fundi
role separation."

Potential stories: 1. Homeowner registration and login. 2. Fundi trade
account registration. 3. User profile association. 4. Role-based access
control. 5. Authentication validation and error handling.

Potential tasks include defining user fields, implementing endpoints,
connecting React forms, protecting routes, and testing
authorized/unauthorized access. This is a planning example; use it as an
actual sprint backlog only if the team selected these stories for that
sprint.

## 4.4 Reflection --- Sprint Backlog

**Draft reflection --- personalize this to match your real experience:**

The planned schedule provides a sequence from technical foundations to
authentication, storefronts, search, bookings, and final stabilization.
The schedule also shows why integration and testing need dedicated time
rather than being left until the last day. However, a sprint plan is not
the same as a sprint result. Since the available Trello board snapshot
does not show separate sprint lists or completed cards, the portfolio
needs additional evidence before it can claim delivery against each
milestone. The next improvement is to maintain a sprint-specific
selection, keep status current, and record the sprint review and
retrospective with links to demonstrable results.

**Evidence to attach:** screenshots of each actual sprint board/list,
selected cards and statuses, and a working feature or test result. If
sprint records do not exist, state that honestly and use the template to
improve future tracking rather than backdating records.

------------------------------------------------------------------------

# 5. Agile Logbook

An Agile logbook records planning, progress, blockers, decisions, and
reflection over time. The logbook should use real dates and events. The
entries below are based only on the available project-plan and Trello
evidence; they do not claim that undocumented meetings or sprint reviews
took place.

## 5.1 Evidence-based activity log

  -------------------------------------------------------------------------
  Date              Evidence available  What can safely   Follow-up needed
                                        be recorded       
  ----------------- ------------------- ----------------- -----------------
  23 July 2026      Trello activity     Planning-board    Add meeting notes
                    shows theme cards   setup and team    or decisions if
                    being assigned and  assignment        available
                    created/updated     activity occurred 
                    around this date    in Trello         

  23 July 2026      Trello board shows  Feature areas and Confirm actual
                    theme cards for     team assignments  ownership and
                    notifications,      were represented  work completed
                    admin, platform     on the board      
                    foundation, and                       
                    other features with                   
                    team members                          
                    assigned                              

  24 July 2026      Trello activity     User needs were   Add acceptance
                    shows user-story    recorded for      criteria and
                    cards being         authentication,   evidence links
                    created/updated     verification,     
                    around this date    storefronts, and  
                                        other modules     

  26 July 2026      Trello activity     The               Confirm why it
                    shows a             planning/setup    changed and
                    member-assignment   card assignment   whether it
                    change on the       was changed       affected delivery
                    planning/setup card                   

  23 July--20       Project-plan        A planned         Record actual
  October 2026      document defines    delivery timeline sprint outcomes,
                    Sprint 0--6 and a   was documented    changes, and
                    presentation                          reasons
                    milestone                             

  28 October 2026   Portfolio           The accessible    Update the board
                    preparation review  board snapshot    to reflect real
                    of connected Trello contains 54       current status
                    board               cards, one        and add delivery
                                        Backlog list, and evidence
                                        no cards marked   
                                        complete          
  -------------------------------------------------------------------------

**Logbook limitation:** The connected Trello board's activity history is
partial evidence of planning actions, not a complete record of daily
stand-ups, conversations, coding sessions, or retrospective discussions.
Add the actual notes or records if they exist.

## 5.2 Reusable daily log template

### Date: \[YYYY-MM-DD\]

-   **Sprint / goal:**
-   **Work planned today:**
-   **Work actually completed:**
-   **Evidence:** \[Trello card, commit, pull request, test result,
    screenshot\]
-   **Blockers or risks:**
-   **Decision made and who agreed:**
-   **What I learned:**
-   **Next step:**

## 5.3 Reusable retrospective template

### Sprint \[number\] retrospective

-   **What went well?** \[Specific event and evidence\]
-   **What did not go well?** \[Specific issue, not blame\]
-   **What caused the issue?** \[Root cause\]
-   **What will we change?** \[One measurable action\]
-   **Who owns the action?** \[Name\]
-   **When will we review it?** \[Date\]
-   **Evidence of improvement:** \[Updated board, test, commit, or
    meeting note\]

## 5.4 Reflection --- Agile Logbook

**Draft reflection --- personalize this to match your real experience:**

The logbook is valuable because it connects the plan to the work
actually performed. A dated record makes it easier to explain why
priorities changed, how blockers were handled, and what was learned from
each iteration. The available Trello activity confirms that planning
cards and assignments were created or changed in July 2026, but it does
not provide enough evidence to reconstruct every daily activity or
sprint retrospective. I should therefore avoid filling gaps with
invented events. The improvement is to record a short update after each
work session and include a concrete evidence link, so that the final
portfolio demonstrates both the process and the result.

**Evidence to attach:** dated stand-up notes, retrospective notes,
Trello activity screenshots, commits, tests, and progress screenshots.
Ensure that each entry accurately reflects your own participation.

------------------------------------------------------------------------

# 6. Overall reflection and improvement plan

The FundiShop planning material presents a broad marketplace with
several connected workflows. The most important learning objective is to
use Agile artefacts as working tools, not only as assessment documents.
User stories make customer needs specific; acceptance criteria define
observable outcomes; the product backlog helps prioritize value and
dependencies; sprint backlogs convert priorities into short-term plans;
and the logbook captures progress and learning.

The most visible planning gap in the accessible Trello snapshot is that
all cards remain in one Backlog list and no card is marked complete.
This does not prove that no implementation work has happened outside
Trello, but it means the board alone cannot demonstrate delivery. The
next practical actions are to:

1.  Confirm team roles and working agreements.
2.  Prioritize the backlog and document acceptance criteria.
3.  Create sprint lists or use another clear workflow with status,
    owner, and due dates.
4.  Add task checklists to the larger theme cards.
5.  Link stories to actual code commits, tests, screenshots, and
    demonstrations.
6.  Record genuine sprint reviews and retrospectives.
7.  Distinguish implemented features from planned integrations such as
    escrow, payment processing, notifications, and production
    deployment.
8.  Review the portfolio against the assessment rubric and keep a copy
    of the final submitted version.

## Personal reflection --- final edit required

Complete the following in your own words before submission:

-   **My contribution:** \[Describe the specific features, planning,
    testing, documentation, or coordination you personally performed.\]
-   **A technical challenge I faced:** \[Describe a real challenge and
    the steps you took.\]
-   **How Agile helped:** \[Explain how a story, backlog, task
    breakdown, or review changed the way you worked.\]
-   **What I would improve:** \[Identify one genuine weakness and a
    practical action.\]
-   **Evidence that supports my reflection:** \[Link to a commit, test,
    screenshot, Trello card, or dated note.\]

------------------------------------------------------------------------

# 7. Evidence checklist for the GitHub Pages portfolio

The assessment rubric allocates marks to both **evidence** and
**reflection** for each of five criteria. Each section should therefore
include a visible artefact and a reflection explaining what the artefact
demonstrates.

  ---------------------------------------------------------------------------
  Criterion         Evidence to include   Reflection to     Ready?
                                          include           
  ----------------- --------------------- ----------------- -----------------
  Agile Team        Agreed charter,       How the charter   ☐
  Charter           confirmed team roles, supports          
                    working agreements    collaboration and 
                                          what should       
                                          improve           

  User Stories and  Trello story cards,   What              ☐
  Tasks             acceptance criteria,  decomposition     
                    task breakdown,       revealed and how  
                    implementation/test   stories became    
                    evidence              testable          

  Product Backlog   Prioritized list,     How priorities    ☐
                    rationale,            reflect value and 
                    dependencies, Trello  scope             
                    screenshot                              

  Sprint Backlog    Actual sprint goal,   What was          ☐
                    selected stories,     delivered,        
                    task owners/status,   blocked, changed, 
                    demo/test evidence    and learned       

  Agile Logbook     Dated notes, actual   What progress and ☐
                    Trello activity,      setbacks taught   
                    commits,              you               
                    test/screenshots                        
  ---------------------------------------------------------------------------

## Suggested screenshots and artefacts

Use real, readable screenshots with short captions: 1. Trello board
showing the project's lists and status. 2. A feature-theme card with its
checklist. 3. A user-story card with acceptance criteria and task
breakdown. 4. The product backlog and agreed priority. 5. A sprint
backlog with its goal and current statuses. 6. A genuine logbook entry
or retrospective. 7. The project architecture diagram or ERD. 8. The
running application showing a feature that actually works. 9. Test
output or API test results. 10. Relevant Git commit history.

Avoid screenshots containing secrets, access tokens, passwords, private
identity documents, or sensitive customer data.

------------------------------------------------------------------------

# References

-   FundiShop Pitch Presentation. Project concept, problem statement,
    target users, value proposition, activities, and business model.
    *(Use the exact title/date shown on the presentation if your
    lecturer requires a formal reference.)*
-   FundiShop Solution Architecture Presentation. Proposed application
    modules, architecture, data entities, security, and integrations.
    *(Use the exact title/date shown on the presentation if your
    lecturer requires a formal reference.)*
-   FundiShop PRP3 Restructured Agile Project Plan. Sprint schedule and
    proposed MVP scope, 23 July--20 October 2026.
-   FUNDI Trello board. <https://trello.com/b/iLYYDYvL/fundi>. Accessed
    28 October 2026.
-   PRP370-1-2S Assessment 2, October 2026. Portfolio instructions and
    assessment rubric.

> Before submitting, check the required Harvard referencing format with
> the lecturer and add full reference details for the presentation files
> and project-plan document.
