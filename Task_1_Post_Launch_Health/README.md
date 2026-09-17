# Phase 3 — Task 1
## Post-Launch Health, Incident Command & Sprint Planning

### Objective

Analyze post-launch performance using real Phase-2 data and convert the evidence into:

1. Launch Performance Report
2. Ranked Evidence-Backed Problem List
3. Phase-3 Analytics Backlog

The analysis follows the required flow:

Data → Evidence → Problem → Priority → Decision / Action

---

## Data Sources

The analysis uses data from completed Phase-2 work:

- `company_events.csv`
- `job_posted_events.csv`
- `payments_data.csv`
- `Marketplace KPI Metrics.xlsx`

No synthetic or toy data was introduced.

---

## Analysis Flow

### Stage A — Understand & Set the Bar

- Definition of Done reviewed
- Upstream Phase-2 inputs confirmed
- Success criteria defined around evidence-based decision making

### Stage B — Launch Performance Report

The launch was analyzed across:

- Funnel
- Revenue
- Retention
- Quality

Each metric was connected to its source and intended business decision.

### Stage C — Biggest Problems

Problems were identified using:

- Observed evidence
- Business impact
- Data reliability
- Ability to take a concrete action

### Stage D — Phase-3 Analytics Backlog

Evidence-backed problems were converted into actionable analytics tasks with:

- Priority
- Metric
- Source
- Decision
- Next Action

### Stage E — Integration & Verification

The analysis was:

- Integrated end-to-end
- Checked for metric traceability
- Tested against controlled data-quality failures
- Demonstrated using real Phase-2 data

---

## Important Data Limitations

### Retention

Reliable retention cannot currently be measured because a reliable longitudinal user/company activity source has not been established in the available Phase-2 datasets.

This is documented as a measurement gap rather than being estimated using unsupported data.

### Job Posting Source Reconciliation

`company_events.csv` contains job-posting events while `job_posted_events.csv` contains a different number of records.

This difference is treated as a source-coverage/reconciliation issue and is not explained without supporting evidence.

### Data Quality

Missing values are validated at the dataset level. Missing cells are not automatically treated as invalid because some fields may be non-applicable for particular event types.

---

## Final Deliverables

The `outputs/` directory contains:

- `launch_performance_funnel.csv`
- `launch_performance_retention.csv`
- `launch_performance_quality.csv`
- `ranked_evidence_backed_problems.csv`
- `phase3_analytics_backlog.csv`
- `metric_traceability.csv`
- `definition_of_done_check.csv`

---

## Tools Used

- Python
- Pandas
- Jupyter Notebook
- CSV
- Excel

---

## Notebook

Main analysis notebook:

`notebooks/Post_Launch_Health_Analysis.ipynb`

---

## Definition of Done

The task deliverables cover:

- Launch Performance Report
- Ranked evidence-backed problem list
- Phase-3 analytics backlog tied to decisions
- Metric traceability
- Validation and edge-case testing
- End-to-end demonstration using real Phase-2 dataa