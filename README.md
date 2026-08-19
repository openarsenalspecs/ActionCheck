# ActionCheck
**Every Action Logged. Every Deviation Noted.**

---

ActionCheck is an open-source civic accountability platform designed to help citizens track whether elected officials follow through on their promises, how they vote while in office, who they financially benefit, and whether their actions align with the people they serve.

The platform combines public records, legislative data, campaign statements, financial disclosures, corporate filings, and AI-powered analysis into one transparent system for public review.

---

## Mission

Modern voters are often forced to rely on campaign slogans, fragmented news coverage, and selective narratives. ActionCheck was created to provide a factual, evidence-based accountability system that compares what politicians say with what they actually do.

---

## Full Feature List

## [Promise Tracker](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/Promise%20Tracker.md)
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

## [Voting Record Analysis](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/Voting%20Record%20Analysis.md)
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

## [Integrity & Deviation Detection](https://codeberg.org/RoxanneA/ActionCheck/src/branch/main/Integrity%20and%20Deviation%20Detection.md)
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