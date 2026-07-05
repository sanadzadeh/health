# Khaled Sanad Portfolio

A personal portfolio of standalone browser-native analytical and decision-support artefacts, built entirely with HTML, CSS, and vanilla JavaScript. No build system, no framework, no node_modules, no package.json. Every artefact is a single self-contained file that runs directly in the browser and deploys to GitHub Pages without a compilation step.

The portfolio is designed to demonstrate applied capability in data architecture, analytics, AI-assisted development, decision support, governance, risk assessment and executive-facing communication.

The current portfolio context is calibrated toward healthcare data, public-sector health analytics, hospital operations, digital health transformation and health service reporting. The artefacts are fictional, but the logic is deliberately realistic: patient flow, service demand, data quality, privacy, access governance, clinical reporting risk, funding pressure, operational bottlenecks and leadership decision-making.

Please check my portfolio: sanadzadeh.github.io/Portfolio

## Client context: Asterion Health Analytics

All artefacts are scoped to Asterion Health Analytics, a fictional multi-site healthcare analytics and decision-support unit supporting a network of hospitals, community health services and executive health planning teams.

Asterion Health Analytics does not provide clinical advice and does not replace clinician judgement. Its role is to improve the quality, reliability and usability of operational and strategic health data. It supports hospital executives, clinical operations teams, finance, workforce planning, quality and safety, privacy, data governance and digital health teams.

The flagship programme is the Health Service Intelligence Uplift FY26 to FY28, moving from fragmented local reporting to a more governed, consistent and executive-ready analytics environment.

The programme covers:

Patient demand forecasting

Emergency department and inpatient flow

Elective surgery backlog visibility

Bed occupancy and discharge planning

Workforce capacity and roster pressure

Clinical quality and safety reporting

Funding and activity-based management

Privacy, consent and access governance

Data quality remediation

Digital health reporting modernisation

The fictional client gives the artefacts a consistent operating environment. The analytical logic, risk frameworks, scoring models and governance structures are transferable across healthcare, government, banking, insurance and enterprise transformation. Asterion Health Analytics simply provides the health-sector stakes.

## Portfolio structure

The portfolio is served from GitHub Pages at sanadzadeh.github.io/Portfolio from the main branch root.

Repository structure:

/
├── index.html
├── cv.html
├── apps/
│   ├── forecasting-dashboard.html
│   ├── deployment-strategy-dashboard.html
│   ├── decision-matrix.html
│   ├── data-risk-assessment.html
│   ├── initiative-tracker.html
│   ├── stakeholder-mapping.html
│   ├── business-case-builder.html
│   └── ledger.html
└── TEMPLATE.html

The portfolio shell renders a grid of tiles. Clicking a tile opens the artefact in a full-screen overlay iframe using openOverlay(href, title). The overlay sets overlayFrame.src from the tile href attribute and calls history.pushState once.

The overlay back button, browser back and Escape key all return directly to index.html. This prevents browser history issues when artefacts are opened and closed repeatedly.

No artefact should call history.pushState, history.back() or modify window.location internally. Internal navigation inside artefacts should use class toggling on sibling div elements. This keeps each artefact self-contained and prevents iframe navigation from corrupting the parent page history.

## Design system

The design reference for the suite is the Decision Matrix artefact. Each artefact uses a shared visual language with its own accent colour.

The suite is intentionally restrained. It avoids decorative icons and relies on typography, spacing, grids, panels, status colours and executive interpretation strips.

Typography:

Cormorant Garamond is used for headers, hero titles, large numerics and executive interpretation text.

DM Mono is used for body text, labels, tags, descriptors and interactive elements.

Colour tokens:

--bg: #141414

--surface: #1c1c1c

--surface-alt: #222222

--surface-hi: #282828

--border: rgba(255,255,255,0.07)

--border-soft: rgba(255,255,255,0.04)

--ink: #f5f2ed

--ink-2: rgba(245,242,237,0.55)

--ink-3: rgba(245,242,237,0.25)

Status colours:

--green: #5f9a78 for healthy, complete, on track or low risk

--amber: #c49a55 for moderate risk, caution or pressure

--red: #b4685d for high risk, critical exposure or hard deadline

--blue: #6b8fa8 for informational signals

Each artefact declares its own accent colour in the root block. The accent drives recommendation strips, active tabs, pills, badges and selected states.

The 1px hairline grid is the main layout device. It creates a dense analytical feel without heavy borders.

Recommendation and interpretation boxes use a 3px left border in the artefact accent colour. This gives leadership-facing sections a consistent visual treatment across the suite.

## Artefacts

## CV

The CV is a single-page curriculum vitae consistent with the suite’s visual system.

It presents professional experience, technical capability, portfolio artefacts, education and certifications in a compact executive format. The layout uses a sticky header, a sidebar for skills and credentials, and a main column for summary, portfolio and experience.

The CV is written to position the portfolio as evidence of applied analytical delivery rather than a collection of disconnected demos. It supports applications across healthcare data, public sector analytics, risk analytics, business intelligence and transformation reporting.

## Forecasting Dashboard

The Forecasting Dashboard is a multi-scenario planning workspace for healthcare demand and service capacity.

It models health service pressure across scenarios such as base demand, winter surge, elective surgery recovery and workforce constraint. Assumption sliders drive live recalculation of outputs rather than switching between static charts.

Potential healthcare use cases include:

Emergency department demand

Bed occupancy

Elective surgery backlog

Workforce availability

Discharge delays

Outpatient service pressure

Activity-based funding exposure

The artefact demonstrates forecasting logic, scenario modelling, executive interpretation and interactive assumptions management.

It is designed to show how complex planning variables can be made visible to decision-makers without requiring them to inspect raw data models.

## Deployment Strategy Dashboard

The Deployment Strategy Dashboard tracks a digital health or reporting modernisation programme across multiple workstreams.

It can represent an EMR reporting uplift, health data platform rollout, operational dashboard deployment or enterprise analytics modernisation programme.

The artefact includes:

Programme confidence

Milestone tracking

Workstream progress

Risk status

Budget variance

Readiness scoring

Executive decision gates

Healthcare calibration should frame this as a health analytics transformation dashboard. The focus is not software delivery for its own sake. The focus is whether the organisation is ready to adopt better reporting, improve governance and make operational decisions from trusted data.

## Decision Matrix

The Decision Matrix is a weighted evaluation tool for health-sector prioritisation decisions.

Possible healthcare uses include:

Selecting the first hospital site for rollout

Prioritising clinical reporting domains

Comparing data platform options

Assessing models of care

Choosing between backlog reduction interventions

Prioritising analytics initiatives under funding constraints

The tool compares options across weighted criteria and recalculates scores live as weights change.

For healthcare applications, this artefact is useful because health organisations often need to make defensible decisions under resource constraints. The tool shows structured judgement, transparent criteria and traceable reasoning.

## Data Risk Assessment

The Data Risk Assessment is one of the strongest healthcare-aligned artefacts.

It evaluates risk across patient data quality, access governance, consent, privacy, reporting integrity, source system reliability and remediation confidence.

Healthcare-specific risk domains include:

Patient identifier quality

Duplicate records

Incomplete clinical coding

Delayed source system feeds

Incorrect access permissions

Privacy and consent exposure

Unclear data ownership

Reporting definitions that differ across sites

Manual spreadsheet dependency

Audit weakness in executive reporting

The point of this artefact is simple: healthcare analytics is only useful if the data is safe, governed and reliable enough to support decisions.

This artefact should be central in applications to NSW Health, private health insurers, hospitals, digital health teams, PHNs and public-sector reporting teams.

## Initiative Tracker

The Initiative Tracker is a portfolio-level view of health analytics and operational improvement initiatives.

It tracks initiatives across workstreams such as data governance, operational reporting, clinical quality, workforce planning and digital health enablement.

Potential initiatives include:

Emergency department dashboard uplift

Patient flow reporting

Elective surgery backlog analytics

Workforce capacity model

Clinical quality data remediation

Privacy access review

Activity reporting standardisation

Executive reporting pack automation

The artefact shows how leadership can see pressure, status, funding exposure, dependencies and decision requirements in one place.

It is useful for demonstrating portfolio thinking, not just dashboard-building.

## Stakeholder Mapping Tool

The Stakeholder Mapping Tool supports engagement planning across health analytics programmes.

Healthcare data work depends heavily on stakeholder alignment. Data teams often need to work across clinicians, operations managers, executives, finance, privacy, ICT, quality and safety, and external reporting bodies.

The tool maps stakeholders by influence and interest, then assigns an engagement posture.

Healthcare examples include:

Chief Medical Information Officer

Nursing operations

ED leadership

Clinical coding

Finance and activity-based funding teams

Privacy and legal

Data governance committee

Hospital executives

Digital health platform owners

Quality and safety teams

This artefact demonstrates that analytics delivery is not only technical. The work also depends on trust, adoption, governance and communication.

## Business Case Builder

The Business Case Builder creates a structured investment case for analytics, automation or reporting uplift.

In a healthcare context, it can support funding proposals for:

Data quality remediation

Executive reporting automation

Patient flow analytics

Digital health reporting uplift

Workforce planning dashboards

Clinical quality reporting

Operational forecasting

Privacy and access governance improvements

The artefact guides the user through problem statement, options analysis, cost-benefit logic, risk, recommendation and executive summary.

This is useful for healthcare roles because many health data initiatives need funding justification, not just technical delivery.

## Ledger

The Ledger should be repositioned for healthcare applications.

The original blockchain and digital asset framing is less relevant to healthcare data jobs and may distract employers. The better healthcare version is a Health Data Glossary or Health Analytics Ledger.

It should explain key concepts such as:

Patient administration systems

Electronic medical records

Master patient index

Activity-based funding

Clinical coding

Emergency department flow

Admitted and non-admitted activity

Data governance

Privacy and consent

Role-based access control

Data lineage

Reporting definitions

Data quality rules

Operational dashboards

Forecasting assumptions

This artefact can become a plain-language knowledge base showing the ability to explain complex health data concepts to non-technical stakeholders.

## Development conventions

All artefacts are standalone HTML files.

No build system is used.

No framework is used.

No package manager is required.

All development should occur on feature branches.

Changes should be submitted through pull request.

Commit messages should be descriptive and content-specific.

Internal artefact navigation should use class toggling only.

Artefacts should not call history.pushState, history.back() or modify window.location internally.

No icons are used across the suite. The upward arrow glyph may be used only for external navigation.

## Healthcare positioning

This portfolio is not intended to claim direct clinical expertise. It is intended to show transferable capability in healthcare data environments.

The strongest positioning is:

I build clear, governed and usable decision-support tools for complex operational environments. In healthcare, that means helping teams make better use of patient flow, service demand, workforce, quality, funding and risk data.

The portfolio should support applications for roles such as:

Health Data Analyst

Senior BI Developer

Health Analytics Consultant

Data Governance Analyst

Reporting Analyst

Digital Health Analyst

Population Health Analyst

Performance Reporting Analyst

Healthcare Business Intelligence Specialist

Data Risk and Controls Analyst

Analytics and Insights Consultant

The core message is that healthcare organisations do not only need dashboards. They need reliable reporting logic, defensible assumptions, safe data handling, clear stakeholder communication and tools that help leaders make decisions under pressure.

## Application relevance

For healthcare employers, the portfolio demonstrates:

Power BI-adjacent dashboard thinking, even though the artefacts are browser-native

Data modelling and decision-support logic

Scenario analysis and forecasting

Risk assessment and governance thinking

Stakeholder and delivery awareness

Executive communication

Ability to convert messy operational concepts into structured tools

Healthcare data applications should not overstate clinical knowledge. The safer and stronger claim is that the artefacts demonstrate the kind of analytical thinking needed in healthcare settings where data quality, privacy, operational pressure and executive reporting all matter.

The portfolio is therefore positioned as evidence of applied data judgement, not as a technical gimmick.
