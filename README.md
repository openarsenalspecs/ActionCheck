# ActionCheck

*Every Action Logged. Every Deviation Noted.*

ActionCheck is an **open-source platform** that empowers citizens to hold politicians accountable. It tracks campaign promises, votes, financial activity, corporate board memberships, and potential conflicts of interest, providing transparency and civic engagement tools. Licensed under **GNU Affero General Public License Version 3+ (AGPL‑3.0+)**.

---

## Features

- ✅ Track campaign promises vs. actual votes  
- ✅ Monitor financial trades and portfolios while in office  
- ✅ Highlight deviations, contradictions, or cronyism  
- ✅ **AI-powered search for past or present corporate board memberships**  
- ✅ Crowdsourced evidence and citizen contributions  
- ✅ Promise Tracker with detailed status:  
  - ✅ Delivered  
  - ⚠️ Partially Delivered  
  - ❌ Not Delivered  
- Fully auditable and open-source  

---

## Tech Stack

- **Backend:** Python (Django/Flask) or Node.js  
- **Frontend:** React + D3.js for interactive dashboards  
- **Database:** PostgreSQL or MongoDB  
- **AI / Analysis:** NLP & semantic models to match promises to actions, detect deviations, flag conflicts of interest, and scan corporate filings  
- **Data Sources:** Government APIs, SEC filings, corporate filings, news & press releases  

---

## Installation

1. Clone the repository using your Git client, for example: `git clone https://codeberg.org/RoxanneA/actioncheck.git` and `cd actioncheck`.  
2. Set up a Python virtual environment if using Django or Flask: `python -m venv venv` and activate it with `source venv/bin/activate`.  
3. Install dependencies: `pip install -r requirements.txt`.  
4. Configure your database (PostgreSQL recommended) in `settings.py`.  
5. Run migrations using: `python manage.py migrate`.  
6. Start the development server: `python manage.py runserver`.  
7. Access the app in your browser at `http://localhost:8000`.  

> *For Node.js backend, follow equivalent steps using `npm install` and `npm start`.*  

---

## Usage

- Browse politicians and view promises with delivery status.  
- Use the **Promise Tracker** to see which promises were delivered, partially delivered, or not delivered.  
- Search for corporate board memberships or financial filings using AI-powered search.  
- Contribute new promises or evidence through the crowdsourced interface.  

---

## Contributing

We welcome contributions from developers, civic tech enthusiasts, and researchers:

1. Fork the repository  
2. Create a new branch for your feature or fix  
3. Commit your changes with descriptive messages  
4. Submit a pull request for review  

**Note:** All contributions must comply with **AGPL‑3.0+** licensing terms and include proper attribution to **Roxanne Ardary** and [roxanneardary.com](https://www.roxanneardary.com/).  

---

## License

This project is licensed under the **GNU Affero General Public License Version 3+ (AGPL‑3.0+)**.  
See LICENSE for full details.  

---

## Contact / Community

- Codeberg: [https://codeberg.org/RoxanneA/actioncheck](https://codeberg.org/RoxanneA/actioncheck)  
- Issues & feature requests: Open a ticket on the repository  
- Discussions & collaboration: Use the Codeberg discussion board  

*This repository is maintained for civic transparency and educational purposes.*