# ActionCheck
**Every Action Logged. Every Deviation Noted.**
- HTML Mirror:  [https://roxanneardary.com/actioncheck-specification/](https://roxanneardary.com/actioncheck-specification/)

---

ActionCheck is an open-source civic accountability platform designed to help citizens track whether elected officials follow through on their promises, how they vote while in office, who they financially benefit, and whether their actions align with the people they serve.

The platform combines public records, legislative data, campaign statements, financial disclosures, corporate filings, and AI-powered analysis into one transparent system for public review.

---

## Mission

Modern voters are often forced to rely on campaign slogans, fragmented news coverage, and selective narratives. ActionCheck was created to provide a factual, evidence-based accountability system that compares what politicians say with what they actually do.

---

## Full Feature List

## [Promise Tracker](https://github.com/openarsenalspecs/ActionCheck/blob/e1bdd85190801b1957efa8bfe7855a3ee4733449/Promise%20Tracker.md)  
[https://roxanneardary.com/promise-tracker/](https://roxanneardary.com/promise-tracker/)  

- Store campaign promises from speeches, websites, interviews, debates, and policy platforms  
- Categorize promises by issue type  
- Mark each promise as:
  - Delivered
  - Partially Delivered
  - Not Delivered
  - Reversed
  - Blocked by Legislature
- Timeline view of promise progress
- Source links for every promise entry
- AI-assisted promise extraction from speeches and websites

---

## [Voting Record Analysis](https://github.com/openarsenalspecs/ActionCheck/blob/47e9c4643dc19b5ea3de032249e5c7026a411335/Voting%20Record%20Analysis.md)  
[https://roxanneardary.com/voting-record-analysis/](https://roxanneardary.com/voting-record-analysis/)  

- Full voting history by politician
- Compare votes to campaign promises
- Highlight contradictions between promises and votes
- Attendance tracking
- Committee participation records
- Sponsored bills and co-sponsored legislation
- Missed vote alerts
- Cross-party voting history

---

## [Integrity & Deviation Detection](https://github.com/openarsenalspecs/ActionCheck/blob/5789a24263c7e3a72e8698bf40029eafb1c7babe/Integrity%20and%20Deviation%20Detection.md)  
[https://roxanneardary.com/integrity-and-deviation-detection/](https://roxanneardary.com/integrity-and-deviation-detection/)  

- Detect sudden policy reversals
- Identify repeated contradictions
- Flag suspicious legislative patterns
- Detect votes favoring donors or affiliated interests
- Cronyism indicators
- Nepotism pattern tracking
- Public-interest scorecards

---

## [Financial Transparency](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/Financial%20Transparency.md)
[https://roxanneardary.com/financial-transparency/](https://roxanneardary.com/financial-transparency/)  

- Portfolio disclosure tracking
- Stock trade monitoring
- Real estate interest disclosures
- Lobbying-linked investment alerts
- Trade timing anomaly detection
- Wealth growth during office timeline
- Insider advantage pattern review
- Compare trades against committee assignments

---

## [Board Membership & Corporate Ties](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/Board%20Membership%20and%20Corporate%20Ties.md)
[https://roxanneardary.com/board-membership-corporate-ties/](https://roxanneardary.com/board-membership-corporate-ties/)  

- AI-powered search for current board memberships
- AI-powered search for former board memberships
- SEC filing analysis
- Corporate registration record scanning
- Nonprofit board tracking
- Advisory role detection
- Conflict-of-interest alerts
- Corporate relationship maps

---

## [AI Intelligence Engine](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/AI%20Intelligence%20Engine.md)
[https://roxanneardary.com/ai-intelligence-engine/](https://roxanneardary.com/ai-intelligence-engine/)  

- Natural language promise detection
- Speech-to-policy comparison
- Semantic contradiction detection
- Voting intent comparison
- Filing document parsing
- Relationship mapping between entities
- Automated source citation linking
- Trend summaries

---

## [Citizen Tools](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/Citizen%20Tools.md)
[https://roxanneardary.com/citizen-tools/](https://roxanneardary.com/citizen-tools/)  

- Public politician profiles
- Search by city, state, district, party, office
- Election season comparison tools
- Re-election risk reports
- Exportable accountability summaries
- Public dashboards
- Mobile-friendly access
- Community evidence submissions
- Public correction requests

---

## [Data & Auditability](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/Data%20and%20Auditability.md)
[https://roxanneardary.com/data-and-auditability/](https://roxanneardary.com/data-and-auditability/)  

- Source links on all major claims
- Timestamped updates
- Change history logs
- Contributor review trails
- Public methodology documentation
- Open-source transparency
- Self-hostable deployments
- API-ready architecture

---

## [Admin & Moderator Tools](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/Admin%20and%20Moderator%20Tools.md)
[https://roxanneardary.com/admin-and-moderator-tools/](https://roxanneardary.com/admin-and-moderator-tools/)  

- Evidence review queue
- Duplicate promise merge tools
- Source validation workflows
- Contributor management
- Abuse prevention tools
- Audit logs
- Moderation dashboard

---

## Optional Plugin Modules

ActionCheck is designed with a modular architecture that allows organizations, civic groups, election organizations, watchdogs, and communities to install specialized plugins for specific elections, jurisdictions, and accountability requirements. The core platform provides the universal accountability infrastructure, while optional modules focus the system on particular types of elections or organizations.

### Local Election Plugin Modules

#### School Board Accountability

- Track school board candidates and incumbents
- Catalog campaign promises concerning curriculum, budgets, staffing, facilities, transportation, and student services
- Compare campaign promises with board votes and meeting minutes
- Track attendance and committee participation
- Monitor school district budgets and major expenditures
- Compare candidate positions with subsequent decisions

#### Municipal Election Module

- Track mayors, city council members, commissioners, and other municipal officials
- Monitor local ordinances and votes
- Track zoning, development, contracts, taxes, fees, and municipal spending
- Compare campaign platforms with municipal actions
- Track relationships with developers, contractors, and local businesses

#### County Election Module

- Track county commissioners and other county-level elected officials
- Monitor county budgets, contracts, infrastructure, public services, and taxation
- Analyze votes against campaign commitments
- Track major vendors and contractors
- Identify recurring relationships between officials and outside organizations

#### State Legislative Module

- Track state representatives and senators
- Compare campaign platforms with legislative voting records
- Monitor sponsored and co-sponsored legislation
- Track committee assignments and votes
- Analyze state-level financial disclosures

#### Runoff Election Module

- Identify races proceeding to a runoff
- Create side-by-side candidate comparisons
- Carry forward the complete Promise Tracker
- Compare first-round and runoff positions
- Track endorsements and newly announced commitments
- Highlight policy changes between the primary and runoff
- Produce voter-focused runoff accountability reports

#### Primary Election Module

- Compare candidates within the same party or primary contest
- Track competing platforms
- Analyze endorsements
- Identify changes in campaign positions
- Compare incumbents against challengers

#### Special Election Module

- Support elections outside the normal election cycle
- Create temporary race profiles
- Track candidates, deadlines, platforms, and results
- Monitor promises made during abbreviated campaigns

#### Recall Election Module

- Track officials subject to recall
- Record recall grounds and supporting claims
- Compare original campaign promises with subsequent actions
- Track recall responses and replacement candidates
- Provide evidence-linked accountability timelines

#### Judicial Election Module

- Track elected judges and judicial candidates
- Record publicly stated positions where legally and ethically appropriate
- Track endorsements and campaign funding
- Monitor financial disclosures
- Maintain separation between factual records and legal conclusions

### Organization-Specific Plugin Modules

Organizations can develop or deploy plugins focused on their own accountability requirements, including:

- School District Plugin
- Municipal Watchdog Plugin
- County Watchdog Plugin
- Taxpayer Accountability Plugin
- Education Accountability Plugin
- Infrastructure Oversight Plugin
- Government Contracting Plugin
- Local Ethics Plugin
- Campaign Finance Plugin
- Election Comparison Plugin
- Candidate Research Plugin

### Plugin Architecture

The ActionCheck Core provides universal functionality used across all election types and organizational deployments.

#### ActionCheck Core

- Politician profiles
- Promise Tracker
- Voting records
- Financial disclosures
- Corporate relationships
- AI analysis
- Evidence management
- Source verification
- Audit trails
- Search
- User permissions
- Reporting

Optional plugins extend the core through a modular structure:

**Plugin → Election Type → Jurisdiction → Data Sources → Specialized Analysis → Reports**

This architecture allows the same ActionCheck installation to support small local elections, such as school board races, as well as municipal, county, state, and statewide elections without requiring every organization to use every available feature.

### Configuration-Driven Plugins

Plugins should be configuration-driven whenever practical rather than requiring modifications to the ActionCheck core.

Organizations can configure:

- Election type
- Jurisdiction
- Offices being tracked
- Applicable public-record sources
- Data collection methods
- Accountability criteria
- Analysis methods
- Reporting requirements
- User permissions
- Organization-specific workflows

This allows organizations to deploy ActionCheck for their specific jurisdiction and mission while maintaining compatibility with the core platform.

### AI Accountability Principles

AI-powered ActionCheck modules should identify, analyze, organize, and explain evidence rather than independently declaring that a politician is corrupt or guilty of wrongdoing.

The system may identify and flag:

- Potential conflicts of interest
- Potential cronyism
- Potential nepotism
- Policy deviations
- Contradictory statements
- Unusual financial patterns
- Relationships requiring review
- Evidence requiring additional investigation

Every significant AI-generated finding should provide supporting sources and distinguish between documented facts, analytical findings, unresolved questions, and allegations.

The objective is to provide citizens with transparent evidence and useful analysis while allowing voters, journalists, researchers, and organizations to make their own informed determinations.

### Plugin Independence

Optional plugins should remain modular and independently maintainable.

Plugins should:

- Avoid unnecessary modifications to the ActionCheck Core
- Maintain their own documentation
- Identify their required data sources
- Document their methodology
- Maintain compatibility requirements
- Preserve ActionCheck attribution requirements
- Comply with the AGPL-3.0+ license
- Maintain auditability of plugin-generated results

Organizations may develop private organizational modules while maintaining compliance with the applicable ActionCheck licensing requirements.

### Plugin Ecosystem

The long-term goal is to create an ecosystem of specialized ActionCheck modules that can be adapted to different communities, elections, jurisdictions, and organizations while maintaining a common accountability framework.

This modular approach allows ActionCheck to function as a general civic accountability platform while giving individual organizations the ability to focus on the elections and public officials most relevant to their communities.

---

## Tech Stack

- Frontend: React
- Data Visualization: D3.js / Chart systems
- Backend: Python (Django / FastAPI / Flask) or Node.js
- Database: PostgreSQL / MariaDB / MongoDB
- Search: OpenSearch / Elasticsearch
- AI Layer: NLP / Semantic Analysis / LLM workflows
- Data Pipelines: Government APIs, SEC filings, campaign sites, public records
- Deployment: Docker / Linux / Self-hosted / Cloud  

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
  - [https://roxanneardary.com/actioncheck/](https://roxanneardary.com/actioncheck/)

---

## License & Notice Requirements

ActionCheck is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- ActionCheck specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.  
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
