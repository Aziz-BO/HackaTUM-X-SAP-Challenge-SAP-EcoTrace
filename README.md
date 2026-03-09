# HackaTUM-X-SAP-Challenge-SAP-EcoTrace

Inspiration
With CSRD making sustainability reporting mandatory for almost all companies by 2026, organizations still rely on manual invoice checking, email searching, and spreadsheet work. We wanted a system that automates everything end-to-end.

What it does
SAP EcoTrace automatically:

Detects sustainability-related emails and invoices
Classifies them by category using SAP AI Core
Extracts key ESG metrics (kWh, liters, m³, emissions, cloud usage, costs)
Removes duplicates, harmonizes units, and stores clean data
Flags anomalies through an AI-powered invoice detector
Waits for user validation and syncs the decision back into the database
Displays live ESG analytics in a web dashboard
Generates on-demand or yearly ESG reports including AI explanations and charts
How we built it
SAP Build Process Automation runs two workflows:

Workflow 1: Email + Data Pipeline

Periodic email trigger
SAP AI Core classification + metric extraction
Anomaly detection on the SAP Build side
Validation request sent to the user
Results synced back to the web app
Clean data appended to a Google Sheet ESG database
Workflow 2: Reporting Engine

Triggered yearly or manually from the dashboard
Aggregates all ESG metrics
Builds graphs (time series, spend by category, distributions)
Uses SAP AI Core to generate narrative insights
Assembles a polished ESG PDF report with charts and company branding
Challenges
Handling inconsistent invoice structures Achieving reliable AI extraction and unit harmonization Designing a safe human-in-the-loop validation cycle Embedding charts into PDFs without distortion Keeping workflows stable across multiple systems

Accomplishments
Fully automated pipeline from email → AI → dashboard → ESG report Robust anomaly detection and validation flow Clean, professional reporting with real charts and AI insights A fast, modern sustainability dashboard with time-range filtering and category analytics

What’s next
More document types & suppliers Scope 3 emission estimation Monthly ESG performance predictions Integration with SAP Analytics Cloud Advanced anomaly detection using time-series models
