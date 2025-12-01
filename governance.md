# SALI Governance Model (Simplified)

_Last updated: 2025‑12‑01_

## 1. Purpose

- Provide a clear, lightweight governance structure for SALI and the Legal Matter Standard Specification (LMSS).
- Support fast, transparent decision‑making for a small community (~10 active volunteers).
- Make it obvious who decides what, and how contributors can participate.

---

## 2. Structure Overview

- **Board of Directors**
  - President: Toby Brown
  - Ex officio directors: current Chairs of
    - Legal Marketing Association (LMA)
    - Association of Legal Administrators (ALA)
    - International Legal Technology Association (ILTA)
- **Operating Board**
  - Members: Jim Hannigan, Toby Brown, Kelly Harbour, Ron Friedmann
- **Working Groups (WGs)**
  - Time‑boxed or ongoing groups focused on specific domains or projects.

**LMSS Release Cadence (high‑level)**

- **Stable release:** once per year in **January**.
- **Beta stream:** during the year, changes are made to the **beta** of the *next* annual version.
- The following January, the accumulated beta becomes the new stable LMSS release.

All work happens in public GitHub repositories where practical.

---

## 3. Board of Directors

### 3.1 Purpose

- Provide overall strategy, oversight, and accountability for SALI.
- Protect the SALI brand, intellectual property, and community.

### 3.2 Scope and Decision Rights

The Board:

- Approves:
  - Overall strategy and annual priorities.
  - Licensing and intellectual property policies for SALI assets.
  - Code of Conduct and any major changes to it.
  - The **annual LMSS release** each January (on recommendation of the Operating Board).
  - Major/breaking changes to the LMSS that significantly affect users.
  - Major changes to governance (this document).
- Serves as:
  - Final appeal body for significant disputes that cannot be resolved by the Operating Board.
  - Final authority on matters that could materially affect SALI’s reputation, legal position, or long‑term direction.

### 3.3 Composition

- **President (Chair):** Toby Brown.
- **Ex officio directors (voting):**
  - Chair of LMA.
  - Chair of ALA.
  - Chair of ILTA.
- Additional Directors may be appointed or elected in accordance with SALI’s bylaws (if any).

### 3.4 Cadence and Practices

- Meets at least **twice per year**, and as needed for:
  - The January annual release.
  - Policy or governance changes.
  - Escalated disputes.
- Decisions:
  - **Quorum:** more than half of current Directors.
  - **Threshold:** simple majority of Directors present, unless law/bylaws require otherwise.
- Transparency:
  - Brief minutes or decision summaries are recorded and stored in the SALI governance repository.
  - Sensitive topics (personnel, legal matters) may be minuted in summary form only.

---

## 4. Operating Board

### 4.1 Purpose

- Run the day‑to‑day standards program.
- Coordinate technical, editorial, and operational work across SALI projects.
- Support and coordinate Working Groups.

### 4.2 Membership

- **Operating Board Members:**
  - Jim Hannigan
  - Toby Brown
  - Kelly Harbour
  - Ron Friedmann

(Additional members may be added by decision of the Board of Directors.)

### 4.3 Scope and Decision Rights

The Operating Board:

- Owns:
  - LMSS roadmap and priorities.
  - **Annual release plan and beta schedule.**
  - Coordination of Working Groups.
  - GitHub repository configuration and permissions.
- Approves:
  - Creation, modification, and closure of Working Groups.
  - Editorial and structural changes to the LMSS that are:
    - Non‑breaking, or
    - Breaking but consistent with existing policies (subject to Board ratification where needed).
  - Contribution guidelines and technical/editorial standards (within the licensing/policy framework set by the Board).
- Resolves:
  - Disputes within or between Working Groups.
  - Prioritization conflicts when volunteer capacity is limited.

### 4.4 Cadence and Practices

- Meets at least **monthly** (can be virtual and informal).
- Decisions:
  - **Quorum:** 3 of 4 members (or >50% if membership changes).
  - **Threshold:** simple majority of members present.
- Implementation:
  - One or more Operating Board members act as **repo maintainers**:
    - Review and merge pull requests.
    - Tag and document releases.
    - Enforce contribution and CI rules.
- Transparency:
  - Meeting notes or decision summaries are stored in the SALI governance or main repo (e.g., `/governance/` or `/docs/`).
  - Major decisions (e.g., release approvals, structural changes) are noted in a simple `DECISIONS.md` or release notes.

### 4.5 LMSS Release Cadence

To keep the LMSS predictable and stable, SALI uses a **fixed annual release cycle**:

- **Annual Stable Release**
  - One **stable version** of LMSS is released **each January**.
  - This release:
    - Consolidates all accepted changes that have accumulated in the beta stream over the prior year.
    - Is proposed by the Operating Board and **ratified by the Board of Directors**.
  - Versioning is aligned to the calendar year (e.g., `2026`, `2027`) or a similar simple scheme agreed by the Operating Board.

- **Beta Stream for the Next Version**
  - Shortly after each January stable release:
    - A **beta line** (branch or tag strategy) is established for the **next** annual version.
  - Throughout the year:
    - Approved changes (new terms, structures, crosswalks, etc.) are merged into this **beta**.
    - The beta may be updated and tagged periodically (e.g., `2027-beta.1`, `2027-beta.2`) for implementers who want to stay current.
  - In the following January:
    - The current beta is finalized as the next **stable** LMSS release.

- **Fixes to the Current Stable Release**
  - The current January stable release is intended to be **largely frozen** for the year.
  - Only:
    - Critical bug fixes, or
    - Clearly non‑controversial corrections (e.g., obvious typos),
    may be back‑ported to the current stable version.
  - These require **Operating Board approval** and are documented clearly in release notes.

---

## 5. Working Groups (WGs)

### 5.1 Purpose

- Do focused work on specific domains, crosswalks, tooling, or documentation.
- Propose changes to the LMSS and related assets.

Examples:
- LMSS Release WG
- Industry Codes WG
- IHL WG
- Funds WG

### 5.2 Scope and Authority

Within their charter, Working Groups:

- Can:
  - Discuss and design changes.
  - Draft term sets, structures, crosswalks, and guidance.
  - Open GitHub issues and pull requests.
  - Use **lazy consensus** to agree on minor, non‑breaking changes.
- Cannot:
  - Change SALI licensing or policies.
  - Approve breaking changes on their own.
  - Override decisions of the Operating Board or Board of Directors.

### 5.3 Composition and Operation

- Membership:
  - Open to interested contributors, subject to the Code of Conduct.
  - Each WG has at least **one coordinator** (appointed by the Operating Board).
- Cadence:
  - Meets as needed (often monthly or bi‑weekly while active).
  - May work primarily via GitHub and email if meetings are not needed.
- Charters:
  - New WGs are created with a simple written charter:
    - Purpose and scope.
    - Expected outputs.
    - Expected duration (e.g., 6–12 months, or ongoing).
  - Charters are stored in the repository (e.g., `/working-groups/<wg-name>/CHARTER.md`).

### 5.4 Decision‑Making in WGs (Lazy Consensus)

- **What “lazy consensus” means**
  - A proposal is considered approved **if no one objects within a defined time window**.
  - It avoids waiting for explicit “yes” votes from everyone; work moves forward unless someone actively raises a concern.

- **How it works in WGs**
  - For minor, non‑controversial changes:
    - Proposal opened as an issue or PR.
    - At least **7 calendar days** for comments.
    - If no substantial objections (`-1`) are raised, the WG treats it as approved.
  - For larger or more visible changes, WGs may use a longer window (e.g., 14 days).
  - Substantial objections or controversial issues:
    - WG attempts to revise and resolve.
    - If unresolved, the WG coordinator escalates to the Operating Board for decision.

---

## 6. Decision Types and Approval Paths

This section describes how common change types move through the system, and how they align with the **annual January release** and **beta** process.

### 6.1 Minor Content Changes (Non‑breaking)

Examples:
- Typo fixes, synonym additions.
- Clarifying definitions without changing meaning.
- Adding terms within an existing, stable hierarchy.

Path and release handling:

1. WG discussion and lazy consensus (or direct PR if trivial).
2. An Operating Board member (as repo maintainer) reviews:
   - Checks for WG agreement and CI passing.
3. By default, changes are merged into the **beta stream for the next annual version**.
4. For clear, low‑risk corrections to the **current stable** version:
   - The Operating Board may decide to back‑port.
   - Such fixes are documented clearly in release notes.
5. Maintainer merges and updates release notes or changelog as appropriate.

### 6.2 New Term Sets or Domains (Generally Non‑breaking)

Examples:
- New matter type lists.
- New court lists.
- New crosswalks that don’t change existing identifiers.

Path and release handling:

1. WG drafts proposal and data (issue + PR).
2. WG seeks lazy consensus (e.g., 14‑day comment window).
3. Operating Board reviews for:
   - Consistency with existing standards and naming.
   - Licensing compatibility for any external crosswalk targets.
4. Operating Board approves and a maintainer merges into the **beta** of the next annual version.
5. The change is included in the **next January stable release**.
6. Exceptionally, if timing and impact justify it, the Operating Board may:
   - Include limited new content in the current year’s January release (if it’s ready before the cut‑off date).

### 6.3 Structural or Breaking Changes

Examples:
- Renaming or removing identifiers.
- Restructuring major hierarchies.
- Changing identifier or versioning policies.

Path and release handling:

1. WG drafts an RFC (request for comments) describing:
   - Rationale and impact.
   - Migration considerations.
2. WG discussion; unresolved disagreements are documented.
3. Operating Board decides whether to:
   - Approve for inclusion in the **next annual release** (beta first), or
   - Reject or send back for revision.
4. For significant or high‑impact changes:
   - The Operating Board recommends the change to the Board of Directors as part of the annual release plan.
   - The Board of Directors reviews and either:
     - Ratifies the plan and authorizes the January release, or
     - Sends back with questions or conditions.
5. The change is then:
   - Implemented and tested in the **beta** branch.
   - Finalized in the following **January stable release**.

### 6.4 Governance or Policy Changes

Examples:
- Changes to this governance document.
- Changes to contribution, review, or release policies (beyond simple editorial tweaks).

Path:

1. Proposal drafted (typically by the Operating Board or a Board Director).
2. Optional public comment window (e.g., 14 days) via GitHub issue.
3. Operating Board reviews feedback and refines proposal.
4. Board of Directors approves or rejects.
5. Changes are:
   - Merged into `GOVERNANCE.md` (this document).
   - Noted in `DECISIONS.md` or meeting minutes.

---

## 7. Conduct, Licensing, and Transparency

### 7.1 Code of Conduct

- SALI maintains a Code of Conduct that applies to:
  - All meetings (virtual or in‑person).
  - All online spaces (GitHub, email lists, chat, etc.).
- The Board of Directors is responsible for:
  - Approving the Code of Conduct.
  - Handling serious or escalated CoC issues.
- The Operating Board may:
  - Handle minor CoC concerns.
  - Recommend actions or policy changes to the Board.

### 7.2 Licensing and IP

- The Board of Directors approves:
  - The licenses under which SALI data, schemas, and tooling are published.
  - Any substantial change to licensing terms.
- Contributors are expected to:
  - Confirm they have the right to contribute materials.
  - Verify and document any licensing requirements for external crosswalks.

(Exact license text and choices are maintained in LICENSE files in each repository.)

### 7.3 Transparency

- Where feasible:
  - GitHub issues and pull requests are public.
  - WG charters and notes are stored in the repository.
- At minimum:
  - Board and Operating Board decisions that materially affect users or contributors are:
    - Recorded in meeting notes, and/or
    - Logged in a simple `DECISIONS.md` file (with date, summary, and link to relevant issues/PRs).

---

## 8. Escalation and Appeals

- Normal escalation path:
  1. Working Group
  2. Operating Board
  3. Board of Directors
- Any contributor or WG may request Operating Board review if:
  - A decision is blocked or stalled.
  - There is a substantive disagreement within a WG.
- Any Operating Board member may request Board of Directors review for:
  - Matters that are high‑risk, precedent‑setting, or outside existing policy.

---

## 9. Amending this Governance Model

- Proposals to change this document can be made by:
  - Any member of the Operating Board, or
  - Any Director on the Board of Directors.
- Process:
  1. Draft changes as a pull request to `GOVERNANCE.md`.
  2. (Optional) Leave open for community comment for at least 14 days.
  3. Operating Board reviews comments and refines the proposal.
  4. Board of Directors approves or rejects the final version.
- Approved changes:
  - Are merged into the main `GOVERNANCE.md`.
  - May be summarized in `DECISIONS.md` or meeting minutes.

---
