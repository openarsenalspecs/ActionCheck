# ActionCheck

Every Action Logged. Every Deviation Noted.

ActionCheck is an open-source platform that empowers voters to hold politicians accountable by tracking promises, votes, financial activities, and potential conflicts of interest. Fully licensed under GNU Affero General Public License Version 3+ (AGPL‑3.0+), ActionCheck ensures transparency, community contributions, and network-copyleft compliance.

Features

✅ Track campaign promises vs. actual votes

✅ Monitor financial trades and portfolios while in office

✅ Highlight deviations, contradictions, or cronyism

✅ AI-powered search for past or present corporate board memberships

✅ Crowdsourced evidence & citizen contributions

✅ Promise Tracker with detailed status:

✅ Delivered

⚠️ Partially Delivered

❌ Not Delivered

Fully auditable and open-source

Tech Stack

Backend: Python (Django/Flask) or Node.js

Frontend: React + D3.js for interactive dashboards

Database: PostgreSQL or MongoDB

AI / Analysis: NLP & semantic models to match promises to actions, detect deviations, flag conflicts of interest, and scan corporate filings

Data Sources: Government APIs, SEC filings, corporate filings, news & press releases

Installation

Clone the repository:

git clone https://codeberg.org/RoxanneA/ActionCheck.git
cd actioncheck

Set up the backend environment (example for Python/Django):

python -m venv venv
source venv/bin/activate
pip install -r requirements.txt

Configure your database (PostgreSQL recommended) in settings.py.

Run migrations:

python manage.py migrate

Start the development server:

python manage.py runserver

Access the app at http://localhost:8000.

Usage

Browse politicians and view promises with delivery status.

Use the Promise Tracker to see which promises were delivered, partially delivered, or not delivered.

Search for corporate board memberships or financial filings using AI-powered search.

Contribute new promises or evidence through the crowdsourced interface.

Contributing

We welcome contributions from developers, civic tech enthusiasts, and researchers:

Fork the repository

Create a new branch for your feature or fix

Commit your changes with descriptive messages

Submit a pull request for review

Note: All contributions must comply with AGPL‑3.0+ licensing terms.

License

This project is licensed under the GNU Affero General Public License Version 3+ (AGPL‑3.0+).
See LICENSE
 for full details.