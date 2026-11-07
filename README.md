# HiLabs RN Case Manager Prototype

An interactive, front-end prototype of a registered-nurse (RN) case-management workbench. It demonstrates how a care team could prioritize a caseload, review a consolidated member record, identify care gaps and medication discrepancies, plan outreach, and document actions with human approval.

> **Prototype / demo only.** This project uses synthetic patient scenarios and illustrative operational metrics. It is not connected to an EHR, claims system, pharmacy, scheduling platform, or other live data source. It is not intended for clinical use and must not be used to make care decisions.

## Live demo

After enabling GitHub Pages, add your published URL here:

`https://<your-github-username>.github.io/<repository-name>/`

## What the prototype demonstrates

- **Prioritized work queue:** explainable, weighted operational priority scoring, escalation flags, filters, and task views.
- **Member 360:** consolidated clinical, medication, timeline, and social-determinants views, with source provenance and freshness labels.
- **Data quality and uncertainty:** facts are labelled Confirmed, Reported, Inferred, Unknown, or Conflicting; discrepancies are surfaced for review rather than silently resolved.
- **AI assistance concept:** draft summaries, care gaps, medication discrepancy reviews, priority explanations, outreach timing, and care-plan suggestions. The nurse remains the decision-maker.
- **Outreach and documentation:** consent-aware channel selection, message review, outcome capture, and approval-oriented documentation flows.
- **Calendar and analytics:** care coordination views, operational metrics, and illustrative performance targets.
- **Role-based views and governance concepts:** RN, VP, CMO, and CIO perspectives, including feed-outage simulation, an AI kill switch, approval gates, and audit-log concepts.
- **Responsive layout:** desktop and mobile navigation/layout adaptations, plus light/dark theme support.

## Run locally

No build step or package installation is required. The prototype is a self-contained HTML file with embedded CSS and JavaScript.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.

Alternatively, run a simple local web server from the repository folder:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploy with GitHub Pages

1. Push `index.html` and this `README.md` to the root of a GitHub repository.
2. Open the repository on GitHub and go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and the `/ (root)` folder, then save.
5. Wait for the Pages deployment to complete. Your public demo URL will look like:

   `https://<your-github-username>.github.io/<repository-name>/`

6. Open the URL in an incognito/private window to confirm that it is publicly accessible.

GitHub Pages can take a few minutes to publish after the first setup or a new deployment.

## Create a QR code for sharing

Once the GitHub Pages URL is live:

1. Copy the exact published URL.
2. Paste it into a QR-code generator you trust, or create a QR code locally.
3. Test the QR code using a phone that is not logged in to GitHub.
4. Put the QR code on your presentation, poster, or resume with a label such as **Scan to explore the prototype**.

**Important:** make the repository public if viewers should be able to access it without being invited. A public GitHub Pages site is viewable by anyone with the URL.

## Suggested repository structure

```text
hilabs-rn-case-manager/
├── index.html
└── README.md
```

## Demo walkthrough

A suggested path for a first-time viewer:

1. Start in **Work Queue** and inspect the prioritized member list.
2. Open a member to explore **Member 360**, including clinical details, medication discrepancies, timeline, and SDOH.
3. Open the AI assistance panel to see example draft outputs and their source/uncertainty framing.
4. Go to **Outreach & Docs** to review the consent-aware outreach and documentation workflow.
5. Explore **Calendar** and **Analytics**.
6. Switch roles to inspect the leadership, clinical governance, and IT/security views.

Some screens and values are deliberately illustrative to communicate a product concept; they are not validated production metrics.

## Important limitations

- All member records and scenarios are synthetic demo data.
- Priority scores and thresholds are illustrative and are not clinically validated.
- AI-style outputs in this standalone prototype are demo logic, not a live AI model or clinical decision-support service.
- Actions such as sending messages, updating records, scheduling appointments, and integrating source systems are not connected to real services.
- Security and compliance items shown as concepts or design statuses are not evidence of certification or regulatory compliance.
- Do not add real patient information, protected health information (PHI), credentials, API keys, or confidential company information to this repository.

## Technology

- HTML
- CSS
- Vanilla JavaScript
- No external package installation required

## License

No license has been specified. Unless you add a license file, others should assume that reuse, modification, and redistribution are not granted by default.
