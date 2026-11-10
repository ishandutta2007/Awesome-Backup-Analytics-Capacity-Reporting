# Awesome-Backup-Analytics-Capacity-Reporting
# Awesome-Backup-Analytics-Capacity-Reporting

## Top Backup Analytics & Capacity Reporting Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Backup Infrastructure Monitoring, Storage Capacity Forecasting & Compliance Reporting*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Backup Analytics & Capacity Reporting**. These tools help IT and backup administrators monitor backup job health, analyze storage consumption trends, forecast capacity needs, validate SLA/RPO compliance, and generate audit-ready reports across hybrid and multi-cloud environments.

**Examples** include Druva Analytics and Reporting, Veeam ONE, Commvault Report Manager, Cohesity Analytics, Rubrik Security Cloud Reports, Datadog Infrastructure Analytics, Splunk Dashboards, Tableau Cloud, Microsoft Power BI, and Looker (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted backup reporting, Prometheus/Grafana-based monitoring, and lightweight analytics exporters—ideal for backup administrators, SREs, platform teams, and developers building transparent, vendor-neutral backup observability stacks.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Druva Analytics and Reporting](https://www.druva.com/)**  
  Cloud platform reports covering backup/restore operations, storage consumption, license usage, alert history, and workload health; supports granular insights, chargeback analysis, and up to two years of historical trend data for compliance audits .

- **[Veeam ONE](https://www.veeam.com/)**  
  Monitoring and analytics suite for Veeam-protected environments with 340+ prebuilt alarms, 150+ reports, capacity planning for VMware/Hyper-V/backup storage, chargeback billing, and ransomware anomaly alerts across backup infrastructure .

- **[Commvault Report Manager (Command Center)](https://documentation.commvault.com/)**  
  Centralized reporting suite with predefined reports for backup/restore summaries, SLA compliance, storage utilization, CommCell readiness, and audit trails; supports automated scheduled report delivery and multi-CommCell monitoring .

- **[Cohesity Analytics (IT Analytics)](https://www.cohesity.com/)**  
  Unified IT analytics platform with dashboards for backup/storage insights, predictive capacity planning, SLA/RTO/RPO compliance tracking, ransomware detection, and chargeback/showback; now available as SaaS with Cohesity Copilot for natural-language report generation .

- **[Rubrik Security Cloud Reports](https://www.rubrik.com/)**  
  API-driven reporting for workload metrics including storage usage, compliance status, SLA assignment, protection status, and backup activity; integrates with Grafana via community plugins for custom dashboards and capacity forecasting .

- **[Datadog Infrastructure Analytics](https://www.datadoghq.com/)**  
  General-purpose observability platform with infrastructure monitoring, log management, and custom dashboards; can ingest backup telemetry via integrations for unified monitoring alongside application and cloud infrastructure metrics .

- **[Splunk Dashboards](https://www.splunk.com/)**  
  SIEM and analytics platform with Druva App/Add-on integration for ingesting backup events; enables centralized monitoring, correlation of backup telemetry with security events, and custom dashboards for operational and compliance reporting .

- **[Tableau Cloud](https://www.tableau.com/)**  
  Visual analytics platform for building custom backup capacity and compliance dashboards from extracted CSV/API data; commonly paired with backup vendor exports for executive-level reporting.

- **[Microsoft Power BI](https://powerbi.microsoft.com/)**  
  Business analytics platform for creating interactive backup reporting dashboards from Commvault, Veeam, or custom data sources; supports scheduled refresh and row-level security for departmental chargeback views.

- **[Looker](https://looker.com/)**  
  Google Cloud's enterprise BI platform for modeling backup data and building governed dashboards; suitable for organizations standardizing analytics across IT operations and finance.

## Open-Source GitHub Projects

- **[Bacula-Web](https://github.com/bacula-web/bacula-web)**  
  Open-source reporting and monitoring tool for Bacula backup infrastructure; provides dashboards for job status, volume usage, weekly statistics, pool/volume reports, and multi-director views with read-only access to the Bacula catalog database .

- **[duplicacy-exporter](https://github.com/geiserx/duplicacy-exporter)**  
  Prometheus exporter for Duplicacy backups that tracks backup duration, files, bytes uploaded, exit codes, and revision numbers per snapshot; ships with a ready-made Grafana dashboard and alert rules for failed or stale backups .

- **[backup-reporter](https://github.com/relaxdiego/backup-reporter)**  
  Python tool with reporter and collector modes: reporter collects backup metadata and uploads to S3; collector aggregates files into CSV and pushes to Google Sheets for centralized reporting across machines .

- **[rdiffweb](https://github.com/ikus060/rdiffweb)**  
  Web interface for rdiff-backup repositories with dashboard showing backups per day, oldest backup, storage usage, average duration, activity metrics, and quota visualization .

- **[rsbackup-graph](https://github.com/richardkettlewell/rsbackup)**  
  Graph generation tool for rsbackup state, producing visual representations of backup coverage and history across hosts and volumes for capacity and compliance overviews .

- **[resticprofile Grafana Dashboard](https://github.com/creativeprojects/resticprofile)**  
  Grafana/Loki dashboard that parses restic backup logs to visualize ingest volume, file counts, success/error rates, time spent, and backup-count diffs for alerting on missed runs .

- **[Rubrik Security Cloud Grafana Plugin](https://grafana.com/grafana/plugins/crestdata-rubriksecuritycloud-datasource/)**  
  Community Grafana data source plugin for Rubrik Security Cloud providing workload metrics, protection/job health, workload inventory, and SLA compliance dashboards without custom API scripting .

### Additional Strong Open-Source Options

- **[Prometheus](https://github.com/prometheus/prometheus)** and **[Grafana](https://github.com/grafana/grafana)** as the foundational open-source stack for backup metrics collection and visualization when paired with exporters.
- **[node_exporter](https://github.com/prometheus/node_exporter)** and **[blackbox_exporter](https://github.com/prometheus/blackbox_exporter)** for host and endpoint-level metrics that complement backup health monitoring.
- **Custom Python/Go exporters** for Veeam, Commvault, and Cohesity APIs to bridge vendor telemetry into Prometheus.
- **Loki** and **Promtail** for log-based backup event parsing and alerting when backup jobs fail or produce anomalous output.
- Many community **Bacula/Zmanda reporting dashboards** and **SQL-based capacity forecasting queries** for custom analytics.

**Frameworks for building custom systems**: Combine **Bacula-Web** for Bacula environments, **duplicacy-exporter** for Prometheus-native backup metrics, **Grafana** for unified dashboards, and **backup-reporter** for spreadsheet-based reporting—or build a custom pipeline with **Prometheus + Loki + Grafana** for full observability across heterogeneous backup tools.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Backup analytics tools must be configured with appropriate data retention and access controls; capacity forecasts are only as reliable as the historical data feeding them.
- Self-hosted open-source solutions require proper metric cardinality management, dashboard maintenance, and alert tuning to remain useful at scale.

---

**Made for backup administrators, SREs, platform teams, and IT finance analysts.**  
Let's make backup analytics more open, observable, and actionable.
