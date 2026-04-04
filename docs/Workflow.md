# ActionCheck Workflow

*Every Action Logged. Every Deviation Noted.*

This document outlines the workflow for **ActionCheck**, including development practices, contribution processes, data handling, and release procedures. This ensures consistency, transparency, and alignment with the AGPL‑3.0+ licensing.

---

## 1. Development Workflow

1. **Fork & Clone:** Developers fork the repository and clone it locally.  
2. **Branching:** Create a new branch for each feature, bug fix, or improvement. Branch names should be descriptive, for example: `feature/promise-tracker`, `fix/vote-data-parsing`.  
3. **Environment Setup:** Set up a local development environment according to the README installation instructions.  
4. **Code Implementation:** Write code following repository conventions and maintain proper attribution to **Roxanne Ardary** and [roxanneardary.com](https://www.roxanneardary.com/).  
5. **Testing:** Run local tests to ensure features work as intended and do not break existing functionality. Automated tests should be added where applicable.  
6. **Commit Messages:** Use clear, descriptive commit messages referencing the feature or issue number. Example: `Add AI board membership search`.  
7. **Push & Pull Request:** Push the branch to your fork and submit a pull request for review. The pull request should include a detailed description of changes, data sources, and any new dependencies.  

---

## 2. Promise Tracker Workflow

1. **Data Collection:**  
   - Campaign promises are sourced from official platforms, speeches, press releases, and interviews.  
   - Votes, legislation, and filings are gathered from government APIs, SEC filings, and corporate records.  

2. **Promise Status Assignment:**  
   - ✅ Delivered: Fully implemented as promised.  
   - ⚠️ Partially Delivered: Implementation is incomplete or modified.  
   - ❌ Not Delivered: No action taken or contradicted.  

3. **Evidence Linking:** Each promise must include references to legislation, votes, corporate filings, or other verifiable sources.  

4. **AI Analysis:** NLP and semantic models match promises to actions, detect contradictions, flag potential conflicts of interest, and scan corporate board memberships.  

5. **Crowdsourced Contributions:**  
   - Citizens may submit evidence, corrections, or new promises.  
   - Moderation ensures accuracy before merging into the main dataset.  

---

## 3. Data Management

- **Database:** PostgreSQL or MongoDB stores promises, politicians, votes, financial transactions, and corporate board data.  
- **Data Updates:** Automated scripts fetch updates from APIs and filings regularly.  
- **Audit Trails:** All data changes are logged with timestamps and contributor information for transparency.  

---

## 4. Release Workflow

1. **Versioning:** Semantic versioning is used (MAJOR.MINOR.PATCH).  
2. **Pre-Release Testing:** All new features undergo local and staging testing.  
3. **Release Creation:** Create a release branch, merge tested features, and tag the release in Git.  
4. **Deployment:** Deploy updates to public-facing servers or testing environments.  

---

## 5. Contribution Guidelines

- All contributions must comply with **AGPL‑3.0+** licensing.  
- Contributors must attribute work to **Roxanne Ardary** and [roxanneardary.com](https://www.roxanneardary.com/).  
- Submit pull requests with full documentation, test coverage, and data source references.  
- Community members can propose new features, fixes, or datasets via issues and discussions.  

---

## 6. Security & Privacy

- Sensitive user or contributor data must be protected according to best practices.  
- Do not expose personal data in public commits, discussions, or datasets.  
- Any security vulnerabilities should be reported via the Codeberg issue tracker for responsible disclosure.  

---

## 7. Documentation & Auditing

- All features, data sources, and workflows must be documented clearly in the repository.  
- Promise Tracker status updates and evidence must be auditable by contributors and end-users.  
- Continuous documentation updates ensure the project remains transparent and trustworthy.  

---

This workflow ensures **ActionCheck** remains transparent, auditable, and fully aligned with the mission: *Every Action Logged. Every Deviation Noted.*  