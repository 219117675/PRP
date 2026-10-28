---
title: "Product Backlog"
permalink: /prp370/product-backlog/
---

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

---
**FundiShop PRP370 Portfolio:** [Overview](../) · [Team Charter](team-charter/) · [User Stories](user-stories/) · [Product Backlog](product-backlog/) · [Sprint Backlog](sprint-backlog/) · [Agile Logbook](agile-logbook/) · [Reflection & Evidence](reflection-evidence/)
---
