# Voting Record Analysis Specification

**Version:** 1.0.0  
**License:** GNU Affero General Public License v3.0 or later (AGPL-3.0+)  

## Overview

The Voting Record Analysis Specification defines a standardized, open-source framework for collecting, structuring, analyzing, and presenting legislative voting records for elected officials. The specification enables transparent tracking of voting activity, legislative participation, campaign promise comparisons, and historical voting patterns.

The system is designed to provide verifiable civic information by connecting official legislative records, campaign commitments, attendance data, committee activity, and sponsored legislation into a unified analysis framework.

---

# Purpose

The purpose of this specification is to establish a common data model and processing framework for:

- Tracking complete voting histories of elected officials
- Comparing legislative votes against publicly stated campaign commitments
- Identifying potential inconsistencies between promises and voting actions
- Monitoring legislative participation and attendance
- Providing transparent access to legislative activity records
- Supporting civic education, journalism, research, and public accountability tools

---

# Core Features

## 1. Complete Voting History

The system MUST support recording the complete voting history of a politician.

Each vote record SHOULD include:

- Official name
- Office held
- Legislative chamber
- Jurisdiction
- Session or legislative term
- Bill or resolution identifier
- Vote date
- Vote type
- Vote position:
  - Yes
  - No
  - Abstained
  - Present
  - Excused
  - Did Not Vote
- Official vote source
- Supporting documentation links

The system SHOULD preserve historical records without modification.

---

# 2. Campaign Promise Comparison

The system MUST support comparing legislative voting activity with documented campaign promises.

Campaign promise records SHOULD include:

- Promise statement
- Source type:
  - Campaign website
  - Speech
  - Interview
  - Debate
  - Policy platform
  - Public statement
- Publication date
- Source reference
- Issue category
- Related legislation
- Promise status

Promise comparison statuses:

- Supported by voting record
- Partially aligned
- Not aligned
- Contradictory
- Insufficient voting data

The system MUST provide source references for all comparisons.

---

# 3. Promise and Vote Contradiction Analysis

The system SHOULD identify differences between publicly stated positions and recorded legislative actions.

Contradiction analysis MAY include:

- Promise keywords
- Policy category matching
- Legislative vote comparison
- Timeline analysis
- Position changes
- Supporting or opposing votes

The system MUST clearly distinguish:

- Verified voting facts
- Documented statements
- Automated analysis
- Human interpretation

Automated analysis MUST NOT be presented as definitive intent.

---

# 4. Attendance Tracking

The system MUST support legislative attendance tracking.

Attendance records SHOULD include:

- Official name
- Legislative body
- Session period
- Meeting date
- Attendance status:
  - Present
  - Absent
  - Excused
  - Unknown
- Attendance source

The system SHOULD calculate:

- Total sessions
- Sessions attended
- Sessions missed
- Attendance percentage
- Attendance trends over time

---

# 5. Committee Participation Records

The system MUST support tracking committee involvement.

Committee records SHOULD include:

- Committee name
- Committee type
- Membership dates
- Role:
  - Member
  - Chair
  - Ranking member
  - Other position
- Hearings attended
- Committee votes
- Committee assignments

Historical committee assignments SHOULD be preserved.

---

# 6. Sponsored Bills and Co-Sponsored Legislation

The system MUST support tracking legislative sponsorship.

Bill sponsorship records SHOULD include:

- Bill identifier
- Bill title
- Sponsor name
- Co-sponsor list
- Date introduced
- Legislative category
- Current status
- Related committees
- Final outcome

The system SHOULD track:

- Number of sponsored bills
- Number of co-sponsored bills
- Legislative activity by category
- Bill progression history

---

# 7. Missed Vote Alerts

The system SHOULD provide notifications for missed legislative votes.

Alert conditions MAY include:

- Missed floor votes
- Repeated absences
- Important legislation missed
- Committee votes missed

Alerts SHOULD include:

- Date
- Legislative item
- Official record source
- Attendance status
- Historical comparison data

---

# 8. Cross-Party Voting History

The system MUST support analysis of voting patterns across party lines.

Cross-party voting records SHOULD include:

- Party affiliation at time of vote
- Vote outcome
- Party majority position
- Individual vote position
- Legislative category

The system MAY calculate:

- Cross-party voting frequency
- Bipartisan voting patterns
- Voting trends over time

Metrics MUST be transparent and include calculation methods.

---

# Data Model

## Politician Entity

Fields:

- Identifier
- Full name
- Office
- Jurisdiction
- Party affiliation
- Terms served
- Official sources

---

## Vote Entity

Fields:

- Vote identifier
- Bill identifier
- Date
- Chamber
- Vote result
- Individual vote position
- Source reference

---

## Promise Entity

Fields:

- Promise identifier
- Statement
- Source
- Date
- Category
- Related issue

---

## Legislation Entity

Fields:

- Bill identifier
- Title
- Description
- Sponsor
- Co-sponsors
- Status
- Committees

---

## Committee Entity

Fields:

- Committee identifier
- Name
- Members
- Assignments
- Meetings

---

# Data Integrity Requirements

The implementation MUST:

- Preserve original source records
- Maintain historical accuracy
- Include citations for all legislative data
- Track changes over time
- Prevent unauthorized modification of verified records
- Separate factual records from analysis layers

---

# Transparency Requirements

All analytical outputs MUST include:

- Data sources used
- Calculation methods
- Confidence indicators
- Last update date
- Limitations

The system MUST avoid presenting automated analysis as confirmed motivation or intent.

---

# API Requirements

Implementations SHOULD provide APIs for:

- Politician lookup
- Voting history retrieval
- Bill tracking
- Promise comparison
- Attendance queries
- Committee records
- Sponsorship records

API responses SHOULD support:

- JSON
- Structured metadata
- Source references
- Historical records

---

# User Interface Requirements

Applications implementing this specification SHOULD provide:

- Politician profile pages
- Voting timeline views
- Legislative activity dashboards
- Promise comparison views
- Attendance summaries
- Committee history
- Bill sponsorship tracking
- Downloadable public records

---

# Security Requirements

Implementations MUST:

- Protect user accounts
- Prevent unauthorized data alteration
- Log administrative changes
- Preserve source attribution
- Secure stored records

---

# Accessibility Requirements

User interfaces SHOULD support:

- Screen readers
- Keyboard navigation
- Clear data visualization
- Mobile accessibility
- Plain-language explanations

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
  - [https://roxanneardary.com/voting-record-analysis/](https://roxanneardary.com/voting-record-analysis/)

---

## License & Notice Requirements

Voting Record Analysis is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Voting Record Analysis specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

**Open Arsenal Hub**  
[https://gitlab.com/Roxanne_Ardary/open-arsenal-specs](https://gitlab.com/Roxanne_Ardary/open-arsenal-specs)

---

# Contributing

Contributions are welcome.

All contributions must:

- Follow the AGPL-3.0+ license
- Preserve specification neutrality
- Maintain transparency requirements
- Include appropriate documentation
- Avoid removing attribution requirements

---

# Specification Goals

The Voting Record Analysis Specification exists to create an open, transparent, and interoperable standard for understanding legislative activity through verifiable public records.