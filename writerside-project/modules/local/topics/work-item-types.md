# Work Item Types

<show-structure/>

This document provides a high-level overview of the different types of work items, along with an fictional reference
example.

| **Work Item Type** | **Definition**                                                       | **Purpose**                                                                                                           | **Scope**                                                   |
|--------------------|----------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| **Epic**           | Large-scale initiative spanning multiple releases/sprints            | Provides a long-term vision and big-picture context                                                                   | Typically, 100+ Story Points, or 1-6 months of work         |
| **Feature**        | Mid-level functionality aligned with part of an Epic’s goal          | Groups related User Stories to deliver a tangible portion of the Epic                                                 | Typically, 20-60 Story Points, or 1–4 sprints of work       |
| **User Story**     | The smallest user-centric item that can be completed within a sprint | Written from an end-user’s perspective, focusing on delivering user value with clear acceptance criteria              | Typically, 1–13 Story Points, or less than 1 Sprint of work |
| **Task**           | Technical activities needed to complete a User Story                 | Details how to implement the User Story (design, coding, testing steps)                                               | Typically, hours to a few days of work each                 |
| **Defect**         | Pre-release errors discovered before going live                      | Must be resolved before the User Story is considered “done” or released                                               | Reported during integration testing, UAT, etc.              |
| **Bug**            | Post-release issues discovered after the product/feature is live     | Maintains quality and reliability post-launch; often triaged at the same level as User Stories in the Product Backlog | Reported by end-users or monitoring tools; may need hotfix  |

## Detailed Descriptions

### Epics {collapsible="true"}

- **Definition**: Large-scale initiatives or strategic objectives that represent a long-term vision. Epics often span
  multiple releases or quarters.

- **Scope**:
    - Typically, **multiple months** of work if taken end-to-end (for a single team).
    - Broken down into several **Features**.

- **Sizing Guidelines**:
    - **Effort** can be in the **hundreds of Story Points** or “several sprints” of work.
    - If an Epic seems too large (e.g., more than a quarter), consider splitting it into multiple Epics.

- **When to Create**:
    - When you have **significant business objectives** that go beyond a short timeline.
    - When multiple Features are required to deliver the overarching goal.

- **Additional Tips**:
    - Epics generally **shouldn’t be assigned** to a single sprint; they are high-level containers.
    - Align Epics with **strategic themes** or high-level product goals.

### Features {collapsible="true"}

- **Definition**: Medium-scope chunks of work that directly contribute to achieving an Epic’s goal.

- **Scope**:
    - Typically, **1–4 sprints** for a single team.
    - Usually consists of **multiple User Stories**.

- **Sizing Guidelines**:
    - **Effort** often falls in the **tens of Story Points** (e.g., 20–60 Story Points).
    - If a Feature grows too large (e.g., spanning over 2–3 months), break it down further or re-check if it’s actually
      an Epic.

- **When to Create**:
    - When you need to define a **functional area** (e.g., “Search Feature,” “Catalog Import Mechanism”).
    - When a set of related capabilities is **too large for a single sprint** but clearly belongs to the same outcome.

- **Additional Tips**:
    - A Feature should provide an **end-to-end function** within the overall Epic (e.g., “Import Partner Catalogs”).
    - Use acceptance criteria at a **higher level** than stories, focusing on the overall functional outcome.

### User Stories {collapsible="true"}

- **Definition**: The smallest **user-centric** deliverables that can be completed in a single sprint, written from an *
  *end-user or stakeholder perspective**.

- **Scope**:
    - **One sprint or less** to develop and validate.
    - Each story delivers **tangible value** to an end-user or stakeholder.

- **Sizing Guidelines**:
    - Often sized between **1–13 Story Points**.
    - If a story is **too large** to complete in a single sprint (e.g., >13 points or your typical max), split it.

- **When to Create**:
    - As soon as you can clearly describe **what the user wants** and **why** they need it.
    - When you have enough detail to craft **acceptance criteria** and confirm feasibility.

- **Additional Tips**:
    - Follow the **INVEST** principle (Independent, Negotiable, Valuable, Estimable, Small, Testable).
    - Focus on **user value** (e.g., “As a [user], I want [goal], so that [benefit].”).

### Tasks {collapsible="true"}

- **Definition**: Technical steps or activities (design, coding, testing, research) required to implement a User Story.

- **Scope**:
    - Typically a **few hours to a couple of days** of work.
    - Very granular and team-member focused.

- **Sizing Guidelines**:
    - Often not estimated in Story Points (though some teams do).
    - If a Task is too large (>16 hours or spanning multiple days), **split** it into smaller Tasks.

- **When to Create**:
    - During **Sprint Planning** or **Story Refinement**, once the team understands **how** to build the Story.
    - If you need to track specific implementation steps or technical sub-tasks.

- **Additional Tips**:
    - Tasks are **optional** for teams comfortable planning at the Story level, but can be invaluable for complex work.
    - If the team is new to Agile or a story is complex, break it down into clear tasks to improve visibility.

### Defects (Pre-Release Issues) {collapsible="true"}

- **Definition**: Functional errors, mismatches, or any kind of software issue discovered **before** a feature or
  product is released to production.

- **Scope**:
    - Typically arise during **integration testing, system testing, or UAT**.
    - Must be **resolved before release** (or explicitly deferred).

- **Sizing Guidelines**:
    - Often **not estimated in Story Points**, but if your process requires it, size them similarly to **small tasks**.
    - The focus is on **fixing** before the new functionality goes live.

- **When to Create**:
    - As soon as testers or developers identify an issue in **non-production** environments.
    - If the fix is more involved than a quick adjustment to an existing story.

- **Additional Tips**:
    - **Link Defects** to the related User Story or Feature for traceability.
    - Address them in the **current or next sprint** to avoid carrying them forward indefinitely.

### Bugs (Post-Release Issues) {collapsible="true"}

- **Definition**: Issues or errors identified **after** the product or feature goes live in a production environment.

- **Scope**:
    - Often discovered by **end-users**, monitoring alerts, or customer support.
    - May require **hotfixes** or patch releases, depending on severity.

- **Sizing Guidelines**:
    - Similar to Defects, typically **not story-pointed** unless the fix is substantial.
    - If the Bug fix is large or complex, consider creating a **separate user story** or treat it like a bigger item in
      the backlog.

- **When to Create**:
    - Immediately upon receiving user reports or monitoring alerts in production.
    - If a quick fix is not possible, the bug goes into the **backlog** and is prioritized by the Product Owner.

- **Additional Tips**:
    - Use a **triage process** to classify severity (e.g., P1, P2).
    - Provide **reproduction steps** and **environment details** to streamline debugging.

## Reference Example

This section contains a comprehensive reference example that **incorporates all work item types**—Epics, Features, User
Stories, Tasks, Defects, and Bugs—along with a hierarchy overview reflecting how it might look in 
the **Product Backlog**. 
The scenario focuses on a practical use case: _"importing and exposing external product catalogs"_.

### Visual Hierarchy

```
Epic: Enable External Product Catalog Integration
└── Feature 1: Import Partner Catalogs
    ├── Story 1: Configure External Catalog Endpoints (8 SP)
    │   ├── Task 1: Create admin portal form
    │   ├── Task 2: Implement endpoint auth & scheduling
    │   └── Defect 1 (pre-release): Endpoint config fails with special chars
    ├── Story 2: Validate and Transform Catalog Data (5 SP)
    │   ├── Task 1: Implement transformation logic
    │   ├── Task 2: Write validation tests
    │   └── Bug 1 (post-release): Discount codes cause missing products
    └── Story 3: Store Product Images (8 SP)
        ├── Task 1: Create backend logic for images
        └── Task 2: Implement compression/resizing

└── Feature 2: Expose Partner Products in the Platform
    ├── Story 1: Display Partner Products in Search Results (8 SP)
    │   ├── Task 1: Extend search index for partner data
    │   ├── Task 2: Update UI labeling
    │   └── Defect 2 (pre-release): Partner brand shows as "N/A"
    ├── Story 2: Filter Partner Products by Brand/Category (5 SP)
    │   ├── Task 1: Enhance filter logic for partner fields
    │   └── Task 2: Update front-end filter components
    └── Story 3: Monitor Import Success/Failure Rates (3 SP)
        ├── Task 1: Create partner-facing dashboard
        ├── Task 2: Implement email notifications
        └── Bug 2 (post-release): Dashboard not auto-refreshing
```

### Epic: "Enable External Product Catalog Integration"  {collapsible="true"}

- **Goal**: Expand the product offerings by allowing third-party partners to deliver product catalogs that our platform
  imports, validates, and displays.
- **Business Value**: High — improves variety and revenue potential.
- **Timeline**:
    - **Start Date**: 01/01/2025
    - **Target Date**: 30/06/2025

<br/>

#### Feature 1: "Import Partner Catalogs" {collapsible="true"}

- **Parent**: _Epic: "Enable External Product Catalog Integration"_
- **Description**: Sets up backend pipelines to receive, validate, and store partner catalog data.

<br/>

##### Story 1: "Configure External Catalog Endpoints" {collapsible="true"}

- **Parent**: _Feature: "Import Partner Catalogs"_
- **Description**: As a catalog manager, I can configure external partner endpoints in the admin portal so that the
  system automatically fetches product data.
- **Story Points**: 8
- **Acceptance Criteria**:
    - Admin portal UI for partner URLs/auth credentials.
    - Configurable schedule for data fetch.
    - Logging of fetch attempts, success/failure.
- **Tasks** (technical activities to implement this story):
    - Task 1: _Create admin portal form for endpoint configuration._
    - Task 2: _Implement endpoint authentication and scheduling logic._
- **Defect** (pre-release):
    - Defect 1: _"Endpoint configuration fails to save when URL contains special characters"_
        - **Description**: Found in QA testing. The system rejects valid URLs if they include certain characters
          like ‘%’ or ‘&’.
        - **State**: New (same level as tasks in the backlog, fix before release).

<br/>

##### Story 2: "Validate and Transform Catalog Data" {collapsible="true"}

- **Parent**: _Feature: "Import Partner Catalogs"_
- **Description**: As a catalog manager, I want product data validated and transformed so that only clean, correctly
  formatted items enter our platform.
- **Story Points**: 5
- **Acceptance Criteria**:
    - Schema checks required fields (SKU, name, price).
    - Invalid entries are flagged and reported.
    - Automatic currency/unit conversions.
- **Tasks**:
    - Task 1: _Implement data transformation logic (currency, units)._
    - Task 2: _Write unit tests for validation pipeline._
- **Bug** (post-release):
    - Bug 1: _"Partner products with discount codes aren’t displayed correctly"_
        - **Description**: Discovered by a user in production; discount codes cause an error in the transformation
          pipeline, leading to missing product records.
        - **State**: Active (same level as Stories in the backlog).
        - **Severity**: High (requires a hotfix or next sprint commitment).

<br/>

##### Story 3: "Store Product Images" {collapsible="true"}

- **Parent**: _Feature: "Import Partner Catalogs"_
- **Description**: As an admin, I want product images stored in a central media library so that they can be displayed
  securely and efficiently.
- **Story Points**: 8
- **Acceptance Criteria**:
    - Images uploaded to secure CDN/storage.
    - Automatic compression/resizing for performance.
    - Linked to product records in the database.
- **Tasks**:
    - Task 1: _Create backend logic to store/retrieve images._
    - Task 2: _Implement image compression/resizing._
- (No known defects or bugs yet.)

<br/>

#### Feature 2: "Expose Partner Products in the Platform" {collapsible="true"}

- **Parent**: _Epic: "Enable External Product Catalog Integration"_
- **Description**: Front-end and API enhancements so users can discover and interact with **imported partner products**.

<br/>

##### Story 1: "Display Partner Products in Search Results" {collapsible="true"}

- **Parent**: _Feature 2: "Expose Partner Products in the Platform"_
- **Description**: As a shopper, I want partner products to appear in my search results so I can easily find all
  available items.
- **Story Points**: 8
- **Acceptance Criteria**:
    - Search indexes partner products alongside internal products.
    - Partner items labeled distinctly if needed.
    - Search performance unaffected.
- **Tasks**:
    - Task 1: _Extend search index to handle partner product data._
    - Task 2: _Update UI to label partner items._
- **Defect** (pre-release):
    - Defect 2: _"Partner brand name not displayed correctly in search results"_
        - **Description**: During UAT, brand names for partner products sometimes show up as “N/A.”
        - **State**: New (must be fixed before release).

<br/>

##### Story 2: "Filter Partner Products by Brand/Category" {collapsible="true"}

- **Parent**: _Feature 2: "Expose Partner Products in the Platform"_
- **Description**: As a shopper, I want to filter search results by brand or category so that I can quickly find
  specific products.
- **Story Points**: 5
- **Acceptance Criteria**:
    - Filter logic includes partner brands/categories.
    - UI clearly shows applied filters.
    - No regressions for internal products.
- **Tasks**:
    - Task 1: _Enhance filter logic to include new brand/category fields._
    - Task 2: _Update front-end filter components._
- (No known defects or bugs yet.)

<br/>

##### Story 3: "Monitor Import Success/Failure Rates" {collapsible="true"}

- **Parent**: _Feature 2: "Expose Partner Products in the Platform"_
- **Description**: As a partner admin, I want real-time statistics on product import success/failures so that I can
  address errors promptly.
- **Story Points**: 3
- **Acceptance Criteria**:
    - Dashboard showing import attempts vs. successes/failures.
    - Ability to drill down into error logs.
    - Email notifications for high failure rates.
- **Tasks**:
    - Task 1: _Create partner-facing dashboard for import stats._
    - Task 2: _Implement email notification logic._
- **Bug** (post-release):
    - Bug 2: _"Dashboard does not refresh with new import data"_
        - **Description**: Reported by partner admins; after a new import, the dashboard remains static until a manual
          browser refresh.
        - **State**: Active in backlog; severity is moderate.

<br/>
