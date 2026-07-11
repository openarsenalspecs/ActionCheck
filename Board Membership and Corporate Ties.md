# Board Membership & Corporate Ties Specification

Version: 1.0  
License: GNU Affero General Public License v3.0 or later (AGPL-3.0+)  
Author Attribution Requirement: Roxanne Ardary  
Website: https://www.roxanneardary.com/

---

# 1. Purpose

The Board Membership & Corporate Ties module is designed to identify, track, and analyze the relationships between individuals, corporations, nonprofit organizations, advisory boards, and affiliated entities. The module provides a comprehensive view of corporate influence, governance relationships, and potential conflicts of interest by continuously monitoring public records and applying artificial intelligence to relationship discovery.

The system enables researchers, journalists, watchdog organizations, compliance departments, and transparency platforms to understand how individuals and organizations are interconnected across public companies, private entities, nonprofits, and advisory groups.

---

# 2. Objectives

The module shall:

- Discover current board memberships
- Discover former board memberships
- Analyze SEC filings
- Scan corporate registration records
- Track nonprofit board participation
- Detect advisory positions
- Identify conflicts of interest
- Build corporate relationship maps
- Monitor changes in relationships over time
- Generate evidence-based alerts
- Provide explainable AI findings
- Support human review and verification

---

# 3. Core Features

## 3.1 Current Board Membership Search

The system shall perform AI-powered searches to identify active board memberships.

### Data Sources

- SEC EDGAR
- Annual reports
- Proxy statements
- Corporate websites
- Investor relations pages
- Corporate governance pages
- Press releases
- State corporate registries
- International corporate registries
- Professional biographies
- University board pages
- Foundation websites
- News articles

### Discovery Methods

- Named entity recognition
- Executive title extraction
- Director extraction
- Biography analysis
- Document classification
- Cross-document verification
- Confidence scoring

### Captured Information

- Organization name
- Position title
- Start date
- Appointment date
- Compensation information
- Committee memberships
- Board status
- Source documents
- Verification score

---

# 4. Former Board Membership Search

The system shall identify historical board positions.

### Historical Sources

- Archived SEC filings
- Historical annual reports
- News archives
- Press releases
- Archived websites
- Corporate history documents
- Nonprofit filings
- Bankruptcy records
- Merger documents

### Historical Data Fields

- Organization
- Position
- Service dates
- Departure date
- Reason for departure
- Successor information
- Historical compensation
- Historical committees

---

# 5. SEC Filing Analysis

## Supported Filing Types

- DEF 14A
- 10-K
- 10-Q
- 8-K
- S-1
- 13D
- 13G
- Form 3
- Form 4
- Form 5

---

## Extraction Requirements

The AI system shall extract:

- Board members
- Executive officers
- Compensation data
- Related party transactions
- Governance structures
- Ownership information
- Committee assignments
- Family relationships
- Related entities
- Consulting agreements
- Advisory agreements

---

## Analysis Engine

The system shall:

1. Download filings.
2. Convert documents into structured text.
3. Extract entities.
4. Link entities.
5. Build relationships.
6. Calculate confidence scores.
7. Store evidence.

---

# 6. Corporate Registration Record Scanning

## Supported Registries

- Secretary of State databases
- Business registration databases
- International company registries
- Beneficial ownership databases
- Corporate transparency databases
- Public procurement databases

---

## Extracted Information

- Directors
- Officers
- Registered agents
- Managers
- Owners
- Company addresses
- Formation dates
- Dissolution dates
- Amendments
- Name changes

---

## Entity Resolution

The module shall:

- Normalize names
- Detect aliases
- Identify name variations
- Match entities across jurisdictions
- Resolve duplicates
- Link subsidiaries
- Link parent organizations

---

# 7. Nonprofit Board Tracking

## Supported Sources

- IRS Form 990
- Charity reports
- Foundation filings
- Nonprofit annual reports
- State nonprofit registries
- University foundation reports
- NGO disclosures

---

## Data Fields

- Board member names
- Officers
- Trustees
- Advisory members
- Compensation
- Committee assignments
- Terms of service
- Family relationships

---

## Monitoring Functions

- Appointment detection
- Resignation detection
- Compensation changes
- Governance changes
- Board expansion detection

---

# 8. Advisory Role Detection

The system shall identify advisory relationships that may not be formally disclosed.

## Sources

- Professional biographies
- Company websites
- Press releases
- News articles
- Conference materials
- LinkedIn-style public profiles
- Academic institutions
- Industry associations
- Consulting agreements

---

## Advisory Roles

- Strategic advisor
- Senior advisor
- Industry advisor
- Scientific advisor
- Technology advisor
- Investment advisor
- Policy advisor
- Advisory board member
- Fellow
- Consultant

---

## Detection Methods

- Natural language processing
- Title extraction
- Relationship classification
- Semantic similarity analysis
- Cross-document validation

---

# 9. Conflict-of-Interest Alerts

The module shall continuously analyze relationships to identify potential conflicts.

---

## Conflict Categories

### Financial Conflicts

- Board memberships and investments
- Stock ownership
- Compensation relationships
- Vendor relationships

### Government Conflicts

- Public office and private board service
- Procurement relationships
- Regulatory influence
- Policy influence

### Nonprofit Conflicts

- Self-dealing
- Related organizations
- Shared directors
- Grant recipient relationships

### Corporate Governance Conflicts

- Interlocking directorates
- Undisclosed affiliations
- Circular ownership
- Family relationships

---

## Alert Severity Levels

### Informational

Low risk relationships.

### Moderate

Potential conflicts requiring review.

### High

Significant conflict indicators.

### Critical

Relationships requiring immediate investigation.

---

## Alert Workflow

1. Detect relationship.
2. Verify evidence.
3. Score risk.
4. Generate alert.
5. Route for review.
6. Document resolution.

---

# 10. Corporate Relationship Maps

The module shall create interactive relationship maps.

---

## Supported Relationships

- Board membership
- Executive relationships
- Ownership
- Subsidiaries
- Parent companies
- Advisory roles
- Investment relationships
- Family relationships
- Nonprofit affiliations
- Government affiliations

---

## Visualization Features

- Network graph
- Timeline mode
- Geographic mode
- Ownership tree
- Influence map
- Interlocking directorate map
- Historical snapshots

---

## Graph Database Requirements

Recommended technologies:

- Neo4j
- ArangoDB
- JanusGraph
- Amazon Neptune

---

# 11. Database Schema Requirements

## Person Table

Fields:

- person_id
- full_name
- aliases
- birth_year
- biography
- confidence_score

---

## Organization Table

Fields:

- organization_id
- organization_name
- organization_type
- jurisdiction
- status
- website

---

## Board Position Table

Fields:

- board_position_id
- person_id
- organization_id
- title
- start_date
- end_date
- active_status

---

## Advisory Position Table

Fields:

- advisory_position_id
- person_id
- organization_id
- title
- start_date
- end_date

---

## Relationship Table

Fields:

- relationship_id
- source_entity
- target_entity
- relationship_type
- confidence_score
- evidence_count

---

## Alert Table

Fields:

- alert_id
- alert_type
- severity
- entity_id
- evidence
- status
- created_at

---

# 12. AI Architecture

## Components

### Entity Recognition Engine

Identifies:

- People
- Organizations
- Titles
- Dates
- Locations

### Relationship Discovery Engine

Identifies:

- Governance relationships
- Ownership relationships
- Influence relationships
- Historical relationships

### Conflict Detection Engine

Identifies:

- Direct conflicts
- Indirect conflicts
- Hidden conflicts
- Emerging conflicts

### Explainability Engine

Provides:

- Evidence
- Sources
- Confidence scores
- Reasoning chain

---

# 13. Search and Indexing Requirements

The system shall support:

- Full text search
- Fuzzy matching
- Alias search
- Historical search
- Relationship search
- Timeline search
- Geographic search
- Organization search

---

# 14. API Requirements

## Search API

- Search by person
- Search by organization
- Search by board position
- Search by advisory role

---

## Relationship API

- Relationship graph retrieval
- Influence graph retrieval
- Historical relationship retrieval

---

## Alert API

- Retrieve alerts
- Resolve alerts
- Export alerts

---

# 15. Evidence Requirements

Every finding shall include:

- Source URL
- Source document
- Retrieval date
- Verification status
- Confidence score
- Evidence text
- Supporting documents

---

# 16. Human Review Requirements

All high-risk findings shall require review.

Reviewers shall be able to:

- Approve findings
- Reject findings
- Modify findings
- Add notes
- Attach evidence
- Escalate investigations

---

# 17. Security Requirements

- Encryption at rest
- Encryption in transit
- Role-based access control
- Audit logging
- Immutable evidence storage
- API authentication
- Data integrity verification

---

# 18. Deployment Requirements

Supported deployments:

- Standalone server
- Container deployment
- Kubernetes
- Private cloud
- Public cloud
- Air-gapped environment

---

# 19. Export Requirements

Supported formats:

- JSON
- CSV
- XML
- PDF
- GraphML
- Neo4j export
- REST API feeds

---

# 20. Compliance Requirements

The module shall comply with:

- AGPL-3.0+
- Data protection regulations
- Public records laws
- Open data standards
- Evidence preservation requirements
- Audit requirements

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
  - [https://roxanneardary.com/board-membership-corporate-ties/](https://roxanneardary.com/board-membership-corporate-ties/)

---

## License & Notice Requirements

Board Membership & Corporate Ties Specification is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Board Membership & Corporate Ties specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

**Open Arsenal Hub**  
[https://gitlab.com/Roxanne_Ardary/open-arsenal-specs](https://gitlab.com/Roxanne_Ardary/open-arsenal-specs)