# Integrity & Deviation Detection Specification

## Version

Version: 1.0.0

## License

GNU Affero General Public License v3.0 or later (AGPL-3.0+)

## Overview

The Integrity & Deviation Detection Specification defines a transparent, auditable, and open implementation framework for analyzing public decision-making patterns, identifying deviations from stated commitments, and detecting measurable indicators of inconsistency, influence, or governance concerns.

This specification enables civic technology platforms, research organizations, journalists, watchdog groups, and public accountability systems to analyze:

- Policy reversals
- Contradictory public statements
- Legislative behavior changes
- Voting patterns
- Potential donor alignment
- Affiliated interest relationships
- Cronyism indicators
- Nepotism indicators
- Public-interest performance measurements

The system is designed as an evidence analysis platform. It does not determine criminal activity, corruption, or intent. It identifies observable patterns from public records and provides structured evidence for human evaluation.

## Module Purpose and Scope

The Integrity & Deviation Detection module exists to create a standardized accountability layer for public information systems.

The module must provide:

- Historical policy tracking
- Public statement comparison
- Legislative behavior analysis
- Relationship mapping
- Influence indicator detection
- Transparency scoring
- Evidence-based reporting

The module scope includes:

- Politicians
- Government officials
- Public agencies
- Legislative bodies
- Political organizations
- Public policy organizations
- Publicly disclosed affiliated entities

The module does not:

- Declare guilt
- Determine illegal conduct
- Replace journalism
- Replace legal investigations
- Make decisions on behalf of users

All findings must be presented as indicators requiring review.

# Core Design Principles

## Evidence-Based Analysis

Every detected pattern must include:

- Source information
- Date recorded
- Original data
- Analysis method
- Confidence score
- Review status

## Neutral Evaluation

The system must evaluate all entities using identical criteria.

The implementation must not:

- Favor political parties
- Favor organizations
- Apply different standards based on ideology
- Modify scoring based on public popularity

## Explainable Results

Every result must explain:

- What was detected
- Why it was detected
- Which records contributed
- How confidence was calculated

## Human Oversight

Automated detection is an analysis assistant.

Final interpretation requires human review.

# Complete Architecture

The Integrity & Deviation Detection system consists of eight primary layers.

## 1. Data Collection Layer

Purpose:

Collect publicly available information from approved sources.

Supported sources include:

- Government legislative databases
- Voting records
- Campaign websites
- Public speeches
- Debate transcripts
- Interview transcripts
- Press releases
- Ethics filings
- Campaign finance records
- Lobbying disclosures
- Procurement databases
- Appointment records

Responsibilities:

- Retrieve source data
- Validate source availability
- Store original documents
- Record timestamps
- Maintain source history

## 2. Data Normalization Layer

Purpose:

Convert different data formats into standardized records.

Responsibilities:

- Remove duplicate records
- Normalize names
- Normalize organizations
- Standardize dates
- Classify issue categories
- Link related entities

Required processing:

- Entity matching
- Document classification
- Statement extraction
- Vote classification
- Relationship extraction

## 3. Evidence Storage Layer

Purpose:

Maintain immutable evidence records.

Requirements:

Every stored evidence record must contain:

- Evidence ID
- Source URL or identifier
- Source organization
- Publication date
- Retrieval date
- Content summary
- Original content reference
- Verification status

## 4. Analysis Engine

Purpose:

Evaluate records and detect patterns.

Components:

- Policy comparison engine
- Contradiction analyzer
- Legislative pattern analyzer
- Relationship analyzer
- Influence indicator engine
- Scorecard calculator

## 5. Relationship Graph Engine

Purpose:

Map connections between entities.

Nodes:

- Individuals
- Organizations
- Companies
- Government agencies
- Legislative bodies
- Donors
- Committees

Edges:

- Employment
- Donations
- Sponsorship
- Appointments
- Contracts
- Family relationships
- Lobbying relationships

## 6. Scoring Engine

Purpose:

Generate transparent accountability measurements.

The scoring engine must:

- Publish formulas
- Display contributing factors
- Allow independent verification
- Maintain calculation history

## 7. Review Layer

Purpose:

Allow humans to validate automated findings.

Capabilities:

- Approve findings
- Reject findings
- Add explanations
- Attach additional evidence
- Correct classifications

## 8. Public Interface Layer

Purpose:

Provide public access to results.

Required features:

- Search
- Entity profiles
- Timeline views
- Evidence displays
- Scorecards
- Reports

# Installation and Deployment Requirements

## System Requirements

Minimum requirements:

- Linux server environment
- Database server
- Application server
- Secure API gateway
- File storage system

Recommended:

- Containerized deployment
- Automated backups
- Monitoring service
- Log aggregation

## Required Software Components

Implementations should include:

- Backend application service
- Relational database
- Search engine
- Graph database
- Document storage
- Authentication service

## Deployment Process

Deployment must include:

1. Install dependencies
2. Configure database
3. Configure storage
4. Import initial data sources
5. Configure analysis modules
6. Run validation tests
7. Deploy user interface
8. Enable monitoring

## Configuration Requirements

Configuration must define:

- Data sources
- Update schedules
- User permissions
- Scoring parameters
- Review requirements
- Security settings

# Data Ingestion Instructions

## Source Registration

Every source must be registered before ingestion.

Required fields:

- Source name
- Source type
- Owner organization
- Access method
- Update frequency
- Reliability classification

## Data Import Workflow

The ingestion process:

1. Retrieve source data
2. Validate format
3. Store original copy
4. Extract structured information
5. Link entities
6. Assign categories
7. Send records for analysis

## Supported Data Types

The system should support:

- HTML documents
- PDFs
- Structured databases
- APIs
- CSV files
- Legislative records
- Financial records

## Data Quality Checks

Before analysis:

- Verify completeness
- Check duplicate records
- Validate dates
- Confirm entity identity
- Flag missing information

# Database Schema Requirements

## Entity Table

Stores analyzed entities.

Required fields:

- entity_id
- entity_name
- entity_type
- jurisdiction
- creation_date
- verification_status

## Statement Table

Stores public statements.

Required fields:

- statement_id
- entity_id
- statement_text
- statement_date
- issue_category
- source_id

## Legislative Record Table

Stores legislative activity.

Required fields:

- record_id
- entity_id
- legislation_id
- vote_position
- vote_date
- committee
- source_id

## Financial Relationship Table

Stores financial relationships.

Required fields:

- relationship_id
- entity_id
- related_entity_id
- relationship_type
- amount
- date
- source_id

## Evidence Table

Stores supporting information.

Required fields:

- evidence_id
- record_type
- record_id
- source_reference
- verification_status
- reviewer_notes

## Analysis Result Table

Stores detection outcomes.

Required fields:

- analysis_id
- entity_id
- detection_type
- confidence_score
- severity_level
- generated_date
- review_status

# Entity Relationship Model

The Integrity & Deviation Detection system uses a relationship-based data model to connect public records, individuals, organizations, and actions.

## Core Entities

## Person

Represents an individual being analyzed.

Attributes:

- Person ID
- Full name
- Public roles
- Jurisdiction
- Political affiliation if publicly available
- Employment history
- Public biography sources

## Organization

Represents entities connected to public activity.

Examples:

- Companies
- Nonprofits
- Government agencies
- Political organizations
- Advocacy groups

Attributes:

- Organization ID
- Organization name
- Organization type
- Industry category
- Location
- Public records

## Policy Position

Represents a stated policy position.

Attributes:

- Policy ID
- Person ID
- Issue category
- Position description
- Date stated
- Source reference
- Confidence rating

## Legislative Action

Represents legislative activity.

Attributes:

- Action ID
- Person ID
- Bill ID
- Vote type
- Vote result
- Sponsorship status
- Committee involvement
- Date

## Financial Relationship

Represents publicly disclosed financial connections.

Attributes:

- Relationship ID
- Donor entity
- Recipient entity
- Amount
- Date
- Disclosure source

## Relationship Record

Represents connections between entities.

Relationship types:

- Employment
- Family
- Donation
- Contract
- Appointment
- Lobbying
- Sponsorship
- Organizational membership

# Detection Algorithms and Workflows

The analysis engine must use transparent rule-based or explainable machine-learning approaches.

All detection results must provide:

- Detection method
- Input records
- Calculation logic
- Confidence score
- Human review status

# Policy Reversal Detection Instructions

## Purpose

Identify significant changes between previously stated policies and later actions.

## Required Workflow

### Step 1: Collect Historical Positions

The system must collect:

- Campaign promises
- Public statements
- Interviews
- Speeches
- Policy documents
- Debate statements

Each statement must be categorized by:

- Issue area
- Position type
- Strength of commitment
- Date

## Step 2: Extract Policy Commitments

The system must identify:

- Supported policies
- Opposed policies
- Promised actions
- Proposed legislation
- Stated priorities

Each commitment receives a classification:

- Strong commitment
- Moderate commitment
- General position
- Opinion statement

## Step 3: Compare Against Actions

The system compares commitments with:

- Votes
- Sponsored legislation
- Administrative decisions
- Public endorsements

## Step 4: Calculate Deviation Score

Example calculation factors:

Commitment strength:
- Strong commitment: higher weight
- General statement: lower weight

Action difference:
- Complete reversal
- Partial change
- Minor adjustment

Time factor:
- Recent changes receive greater attention

## Required Output

Every policy reversal finding must include:

- Original statement
- Later action
- Difference explanation
- Supporting sources
- Deviation score
- Reviewer status

# Contradiction Analysis Instructions

## Purpose

Detect repeated inconsistencies between statements and behavior.

## Workflow

## Statement Collection

Collect statements across:

- Campaign periods
- Legislative periods
- Public interviews
- Official announcements

## Action Collection

Collect:

- Votes
- Sponsorships
- Policy decisions
- Public actions

## Comparison Process

The system evaluates:

Statement:

- Position expressed
- Issue category
- Date

Compared with:

- Later behavior
- Legislative record
- Policy outcome

## Contradiction Categories

The system should classify:

### Direct Contradiction

Example:

A stated position directly conflicts with a later action.

### Partial Contradiction

Example:

An action modifies or weakens a previous position.

### Repeated Contradiction

Example:

Multiple conflicts occur over time.

## Contradiction Score

The score should consider:

- Number of contradictions
- Importance of issue
- Strength of original statement
- Time consistency

## Required Output

Reports must provide:

- Contradiction timeline
- Issue grouping
- Evidence records
- Confidence level

# Legislative Anomaly Detection Instructions

## Purpose

Identify unusual legislative behavior patterns.

## Data Inputs

Required inputs:

- Voting history
- Bill sponsorship
- Committee records
- Amendment records
- Legislative attendance

## Detection Categories

## Voting Pattern Changes

Detect:

- Sudden voting shifts
- Significant deviation from previous patterns
- Unusual issue-specific changes

## Sponsorship Patterns

Analyze:

- Bills introduced
- Industries affected
- Legislative frequency
- Co-sponsorship relationships

## Committee Activity

Analyze:

- Attendance
- Participation
- Voting behavior
- Committee assignments

## Coalition Analysis

Identify:

- Cross-party cooperation
- Unusual voting alliances
- Changing legislative relationships

## Required Output

Each anomaly report must contain:

- Pattern detected
- Historical comparison
- Related legislation
- Statistical measurement
- Explanation

# Donor and Interest Alignment Analysis Instructions

## Purpose

Analyze relationships between disclosed financial interests and policy activity.

## Required Data Sources

Include:

- Campaign contributions
- Lobbying disclosures
- Financial disclosures
- Corporate relationships
- Industry records

## Workflow

## Step 1: Map Financial Relationships

Create relationships between:

- Donors
- Organizations
- Candidates
- Officials

## Step 2: Identify Policy Connections

Compare relationships with:

- Votes
- Sponsored legislation
- Regulatory actions

## Step 3: Calculate Alignment Indicators

Possible factors:

- Frequency of alignment
- Timing relationship
- Industry relevance
- Public disclosure status

## Required Restrictions

The system must not state:

- "Person was bought"
- "Person committed corruption"
- "Person acted illegally"

The system may state:

- "Voting pattern overlaps with disclosed interest category"
- "Financial relationship exists with related industry"
- "Additional review may be appropriate"

## Required Output

Include:

- Financial relationship
- Policy action
- Timeline
- Evidence sources
- Alignment score

# Cronyism Tracking Workflow

## Purpose

Identify patterns where connected organizations repeatedly receive favorable outcomes.

## Data Inputs

Collect:

- Government contracts
- Procurement records
- Regulatory decisions
- Appointments
- Lobbying relationships

## Workflow

### Relationship Identification

Identify:

- Decision makers
- Beneficiaries
- Organizational connections

### Pattern Analysis

Analyze:

- Frequency
- Timing
- Competitive environment
- Relationship history

## Indicators

Possible indicators:

- Repeated contract awards
- Limited competition
- Connected beneficiaries
- Policy advantages

## Required Output

Provide:

- Relationship map
- Event timeline
- Supporting documents
- Indicator score

# Nepotism Tracking Workflow

## Purpose

Identify publicly documented family or personal relationship patterns.

## Data Inputs

Use:

- Public biographies
- Government records
- Appointment records
- Corporate records

## Workflow

Identify:

- Family relationships
- Employment relationships
- Appointment relationships

Analyze:

- Timing
- Role changes
- Benefits received

## Requirements

The system must:

- Verify relationships
- Avoid assumptions
- Require public documentation

## Output

Include:

- Relationship type
- Source evidence
- Timeline
- Review status

# Public-Interest Scoring Methodology

The Public Interest Scorecard provides transparent measurements based on documented activity.

## Score Categories

# Transparency Score

Measures:

- Disclosure completeness
- Public accessibility
- Record availability
- Communication practices

# Accountability Score

Measures:

- Response to oversight
- Public reporting
- Correction practices

# Consistency Score

Measures:

- Alignment between stated positions and actions

# Participation Score

Measures:

- Attendance
- Voting participation
- Committee involvement

# Independence Score

Measures:

- Disclosure quality
- Conflict management
- Relationship transparency

## Scoring Requirements

Every score must include:

- Formula
- Weighting
- Data inputs
- Limitations
- Confidence level

Scores must never be presented without explanation.

# Evidence Verification Requirements

The Integrity & Deviation Detection system must maintain strict evidence verification standards.

## Evidence Classification

Every evidence record must be assigned a verification level.

## Verified Evidence

Verified evidence includes:

- Official government records
- Legislative records
- Court records
- Public filings
- Official statements
- Government databases

## Secondary Evidence

Secondary evidence includes:

- Established journalism
- Academic research
- Recognized organizations

Secondary evidence must be clearly labeled.

## Unverified Evidence

Unverified evidence includes:

- User submissions
- Anonymous claims
- Unconfirmed reports

Unverified evidence must not independently generate final findings.

# Evidence Storage Requirements

Every evidence item must store:

- Evidence identifier
- Source name
- Source location
- Collection timestamp
- Publication timestamp
- Content type
- Verification status
- Related entities
- Related analysis results

## Source Integrity Requirements

The system must:

- Preserve original references
- Track source changes
- Record retrieval dates
- Maintain historical versions

## Evidence Confidence Levels

Each finding must include:

High Confidence:

- Multiple verified sources
- Direct documentation
- Clear relationship

Medium Confidence:

- Strong supporting evidence
- Some interpretation required

Low Confidence:

- Limited documentation
- Requires additional review

# Human Review Process

Automated analysis must always include human review capabilities.

## Review Roles

## Analyst

Responsibilities:

- Review findings
- Verify sources
- Add notes
- Confirm classifications

## Reviewer

Responsibilities:

- Validate analyst conclusions
- Approve or reject findings
- Request additional evidence

## Administrator

Responsibilities:

- Manage permissions
- Configure detection rules
- Audit system activity

# Review Workflow

## Step 1: Detection Generated

The system creates:

- Finding record
- Evidence package
- Confidence score

## Step 2: Analyst Review

The analyst evaluates:

- Source accuracy
- Entity matching
- Classification accuracy
- Context

## Step 3: Reviewer Decision

Possible outcomes:

Approved:

Finding is published.

Rejected:

Finding is archived.

Needs More Evidence:

Finding remains under review.

## Review History

The system must maintain:

- Reviewer identity
- Review timestamp
- Decision
- Explanation
- Changes made

# False-Positive Handling

The system must provide mechanisms to prevent incorrect conclusions.

## False Positive Prevention

Required methods:

- Entity verification
- Source validation
- Multiple evidence requirement
- Confidence thresholds
- Human review

## Correction Process

Users must be able to:

- Submit corrections
- Provide additional evidence
- Request review

## Correction Requirements

Corrections must include:

- Original finding
- Reason for correction
- Supporting information
- Review outcome

## Model Improvement

Detection rules should be updated based on:

- Confirmed false positives
- Review feedback
- New evidence standards

# Transparency Requirements

The system must operate with public accountability principles.

## Required Public Information

Published findings should include:

- Detection category
- Evidence sources
- Methodology
- Confidence score
- Review status

## Methodology Disclosure

The system must disclose:

- Detection rules
- Scoring formulas
- Data sources
- Limitations

## Audit Transparency

Maintain:

- Analysis history
- Rule changes
- Version history
- Correction records

# Security Requirements

The implementation must protect:

- Evidence integrity
- User accounts
- Review records
- System configuration

## Authentication Requirements

Implementations should support:

- Secure authentication
- Role-based access control
- Multi-factor authentication

## Authorization Requirements

Permissions must control:

- Data access
- Review actions
- Administrative changes

## Data Protection

The system must include:

- Encryption in transit
- Encryption at rest
- Secure backups
- Access logging

## Audit Logging

The system must log:

- User actions
- Data changes
- Review decisions
- Configuration changes

# API Specifications

The system should provide REST or equivalent APIs.

## Entity API

Purpose:

Retrieve analyzed entities.

Required operations:

- Create entity
- Update entity
- Retrieve entity
- Search entities

## Evidence API

Purpose:

Retrieve supporting records.

Required operations:

- Submit evidence
- Retrieve evidence
- Verify evidence
- Update evidence status

## Analysis API

Purpose:

Run detection processes.

Required operations:

- Start analysis
- Retrieve results
- Update review status
- Generate reports

## Scorecard API

Purpose:

Provide public-interest measurements.

Required operations:

- Generate scorecard
- Retrieve score history
- Compare entities

## API Security

APIs must support:

- Authentication
- Authorization
- Rate limiting
- Request validation
- Audit logging

# User Interface Requirements

The user interface should provide transparent access to system results.

## Public Dashboard

Required features:

- Entity search
- Scorecards
- Findings
- Evidence access
- Timelines

## Entity Profile Page

Should display:

- Biography information
- Policy history
- Voting record
- Relationships
- Findings
- Scores

## Evidence Viewer

Must display:

- Source information
- Evidence timeline
- Related records
- Verification status

## Analyst Interface

Should support:

- Review queue
- Evidence comparison
- Finding approval
- Notes and annotations

## Administrative Interface

Should support:

- User management
- Rule configuration
- Audit logs
- System settings

# Testing Requirements

All implementations must include testing.

## Unit Testing

Test:

- Data processing
- Entity matching
- Score calculations
- Detection rules

## Integration Testing

Test:

- Data ingestion
- Database operations
- API communication
- User workflows

## Security Testing

Test:

- Authentication
- Authorization
- Data protection
- API security

## Accuracy Testing

Test:

- Detection reliability
- False positive rates
- Evidence matching
- Scoring consistency

## Regression Testing

Required after:

- Rule changes
- Database changes
- Software updates

# Deployment Validation

Before production deployment:

Verify:

- Database integrity
- Security configuration
- Backup systems
- API availability
- Review workflows
- Audit logging

# Version Management

The specification follows semantic versioning.

## Major Versions

Used for:

- Breaking architectural changes
- Database redesigns
- API incompatibility

## Minor Versions

Used for:

- New features
- Additional detection modules
- Compatible improvements

## Patch Versions

Used for:

- Bug fixes
- Documentation updates
- Security improvements

# Contribution Requirements

Contributions must:

- Maintain AGPL-3.0+ compatibility
- Preserve transparency standards
- Include documentation
- Include tests
- Avoid partisan modifications
- Maintain evidence-based analysis

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

---

## License & Notice Requirements

Integrity & Deviation Detection Specification is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Integrity & Deviation Detection specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

**Open Arsenal Hub**  
[https://gitlab.com/Roxanne_Ardary/open-arsenal-specs](https://gitlab.com/Roxanne_Ardary/open-arsenal-specs)