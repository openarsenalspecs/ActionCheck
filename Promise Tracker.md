# Promise Tracker Specification
- HTML Mirror:  [https://roxanneardary.com/promise-tracker-specification/](https://roxanneardary.com/promise-tracker-specification/)

---

## Overview

Promise Tracker is an open-source specification for tracking, organizing, and verifying campaign promises made by elected officials and candidates. It provides a standardized framework for collecting promises from speeches, websites, interviews, debates, policy platforms, and public statements, then monitoring their progress through completion, partial fulfillment, reversal, or non-delivery.

The specification enables transparent accountability systems by combining structured promise records, source verification, timeline tracking, evidence management, analytics, and AI-assisted promise extraction.

Promise Tracker is designed for civic platforms, government transparency applications, journalism tools, research organizations, and public accountability systems.

---

## Source Collection

Collects promises from multiple public sources.

Supported sources:

- Campaign websites
- Policy platforms
- Candidate statements
- Speeches
- Interviews
- Debates
- Press releases
- Social media posts
- Public announcements
- Government documents
- Legislative records

Source tracking includes:

- Source URL
- Source type
- Publication date
- Archived copy reference
- Transcript storage
- Citation metadata
- Source reliability rating

---

## Promise Categorization

Organizes promises by issue area and policy domain.

Built-in categories:

- Economy
- Healthcare
- Education
- Housing
- Transportation
- Energy
- Environment
- Taxes
- Immigration
- Public Safety
- Foreign Policy
- Labor
- Technology
- Government Reform
- Veterans
- Agriculture

Features:

- Multiple category assignment
- Custom categories
- Hierarchical category structures
- Keyword tagging
- Topic classification

---

## Promise Status Tracking

Tracks promise progress using standardized fulfillment states.

Supported statuses:

- Proposed
- In Progress
- Delivered
- Partially Delivered
- Not Delivered
- Reversed
- Blocked by Legislature
- Blocked by Courts
- Abandoned

Features:

- Status history tracking
- Status change timestamps
- Reason tracking
- Evidence requirements
- Confidence scoring

---

## Promise Timeline System

Provides chronological tracking of promise progress.

Timeline features:

- Promise announcement date
- Implementation milestones
- Legislative actions
- Executive actions
- Funding events
- Program launches
- Court decisions
- Completion milestones
- Status changes

Timeline views:

- Chronological history
- Progress visualization
- Milestone tracking
- Election cycle comparison

---

## Evidence Management

Maintains supporting documentation for every promise.

Evidence sources:

- Government records
- Legislation
- Executive orders
- Budget documents
- Official statements
- Public reports
- News coverage
- Archived webpages

Evidence metadata:

- Source link
- Source type
- Collection date
- Verification status
- Reliability rating
- Reviewer notes

---

## AI-Assisted Promise Extraction

Provides AI tools for identifying promises from public communications.

AI capabilities:

- Extract promises from speeches
- Analyze campaign websites
- Process debate transcripts
- Analyze interview transcripts
- Extract policy commitments
- Identify measurable goals
- Detect duplicate promises
- Categorize promises automatically
- Generate summaries
- Suggest related evidence
- Identify changes in commitment language

Supported inputs:

- Web pages
- HTML documents
- PDFs
- Text documents
- Audio transcripts
- Video transcripts
- Public statements

---

## Verification Framework

Creates transparent verification workflows.

Features:

- Human review workflows
- Evidence-based verification
- Multi-source confirmation
- Reviewer comments
- Confidence scoring
- Verification history
- Audit trails

Verification levels:

- Unverified
- Low Confidence
- Moderate Confidence
- High Confidence
- Verified

---

## Analytics Dashboard

Provides accountability metrics and reporting.

Analytics include:

- Total promises made
- Promises delivered
- Partial fulfillment rate
- Non-delivery rate
- Reversal rate
- Average completion time
- Fulfillment by issue category
- Fulfillment by election cycle
- Administration comparison
- Progress trends

---

## Search and Discovery

Advanced search tools for exploring promises.

Search features:

- Full-text search
- Candidate search
- Official search
- Issue category search
- Jurisdiction filtering
- Status filtering
- Date filtering
- Election cycle filtering
- Source filtering

---

## Public Transparency Features

Designed for public accountability platforms.

Features:

- Public promise pages
- Shareable records
- Open data exports
- Citation visibility
- Source transparency
- Timeline visualization
- Community review submissions

---

## API Specification

Promise Tracker supports integrations through standardized APIs.

API capabilities:

- Create promise records
- Retrieve promises
- Update promise status
- Add evidence
- Add timeline events
- Search records
- Generate analytics
- Export datasets

---

## Data Model

### Promise Object

Fields:

- Promise ID
- Title
- Description
- Candidate
- Organization
- Jurisdiction
- Election cycle
- Categories
- Status
- Sources
- Evidence
- Timeline events
- Confidence score
- Created date
- Updated date

### Evidence Object

Fields:

- Evidence ID
- Promise ID
- Source URL
- Source type
- Description
- Verification status
- Confidence score
- Date collected

### Timeline Event Object

Fields:

- Event ID
- Promise ID
- Event date
- Event type
- Description
- Supporting evidence

---

## Optional Extensions

Promise Tracker can be extended with:

- Legislative Tracker integration
- Executive action monitoring
- Budget analysis
- Fact-checking systems
- Public submissions
- Crowdsourced verification
- AI accountability scoring
- Notification systems
- Comparative government dashboards
- Open civic data platforms  

---

## Specification Branding License (SBL)

### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/promise-tracker/](https://roxanneardary.com/promise-tracker/)

---

## License & Notice Requirements

Promise Tracker is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Promise Tracker specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  