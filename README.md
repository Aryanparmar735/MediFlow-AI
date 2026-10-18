# MediFlow AI — Hackathon Prototype

A single-file, responsive prototype for **Smart Health — AI-Driven Health Center and Supply Chain Management**.

## Features
- Dashboard with inventory status and low-stock alerts
- Medicine inventory: search, filter, add medicines, update stock
- Supply orders: create orders and update order status
- Explainable demand estimates based on fictional weekly-usage values
- Health-center network and transfer-review suggestions
- Rule-based supply assistant (no external AI service is falsely claimed)
- CSV inventory export
- Browser localStorage persistence and reset-to-demo-data option
- Basic validation, semantic labels, keyboard focus states, responsive layout

## Run locally
Simply open `index.html` in a modern browser. No build step, API key, or package install is needed.

## Important limitations
- This is a hackathon demo with fictional data, not a production clinical system.
- It does not provide medical diagnosis or treatment recommendations.
- Demand insights are transparent rule-based estimates, not a trained forecasting model.
- Data is stored in the current browser via localStorage; there is no shared backend, authentication, or server-side authorization.
- Do not enter real patient or confidential health data.

## Submission checklist
1. Test adding a medicine and changing its stock.
2. Check that low-stock badges and dashboard counts update.
3. Create a supply order and change its status.
4. Test search, status filter, CSV export, and reset.
5. Upload `index.html` and this README to a **public GitHub repository** if the event requires public source code.
6. Deploy using the platform specifically required by the organizers. If they specifically require a Google Cloud Run URL, follow their Cloud Run instructions; a GitHub Pages URL may not satisfy that field.
7. Paste the public repository URL and deployed URL into the event submission form.
8. Only submit a LinkedIn post URL if required; don't invent one.

## Cloud Run note
This is a static HTML app. Cloud Run typically expects a containerized service. If Cloud Run is mandatory, you can add a tiny web server/container (for example, Nginx) and deploy that container. Verify that the URL is publicly accessible before submission.
