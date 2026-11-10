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
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The backup analytics, storage capacity planning, and data protection reporting market is estimated at approximately **$12B–$15B** globally (growing at an 11–14% CAGR through 2030), driven by exponential data growth, compliance mandates (GDPR/HIPAA/DORA), and cyber-resilience demands. The sector is **moderately fragmented** rather than winner-take-all: while mega-cap hyperscalers (Microsoft, Alphabet) dominate horizontal enterprise BI and observability giants (Datadog, Splunk) capture centralized telemetry, specialized data protection vendors (Veeam, Cohesity, Rubrik, Commvault, Druva) maintain entrenched, indispensable moats around workload-specific metadata, catalog intelligence, and immutable backup compliance reporting.

## SaaS/Hosted Platforms

| Product | Company Size (Valuation / Revenue) | Starting Pricing | Free Tier / Free Trial Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Power BI](https://powerbi.microsoft.com/)** | **~$3.1T Market Cap** *(Parent: Microsoft; FY24 Rev: $245B)* | **$14.00/user/month** (Power BI Pro, billed annually) | **Free Forever Tier**: Free for personal use via Power BI Desktop/Fabric Free; sharing/collaboration disabled, 1 GB dataset model size limit, manual refreshes only. | Business analytics platform for creating interactive backup reporting dashboards from Commvault, Veeam, or custom data sources; supports scheduled refresh and row-level security for departmental chargeback views. |
| **[Looker](https://looker.com/)** | **~$2.1T Market Cap** *(Parent: Alphabet; FY24 Rev: $350B)* | **$5,000/month** (Looker Standard Platform, annual contract; Looker Studio Pro starts at $9/user/month) | **30-day Free Trial**: Full access to Looker Cloud Core platform (underlying BigQuery/cloud infrastructure usage billed separately; base Looker Studio has a free forever tier). | Google Cloud's enterprise BI platform for modeling backup data and building governed dashboards; suitable for organizations standardizing analytics across IT operations and finance. |
| **[Tableau Cloud](https://www.tableau.com/)** | **~$280B Market Cap** *(Parent: Salesforce; FY24 Rev: $34.9B)* | **$15.00/user/month** (Tableau Cloud Viewer, billed annually; requires min. 1 Creator at $75/user/month) | **14-day Free Trial**: Full evaluation access to Tableau Cloud and Tableau Desktop at Creator tier with full authoring and data connection capabilities; no credit card required. | Visual analytics platform for building custom backup capacity and compliance dashboards from extracted CSV/API data; commonly paired with backup vendor exports for executive-level reporting. |
| **[Splunk Dashboards](https://www.splunk.com/)** | **$28B Valuation** *(Acquired by Cisco; Observability Cloud from $15/host/mo)* | **$15.00/host/month** (Splunk Observability Cloud; Splunk Cloud Platform quote-based by workload/SVC or daily ingest) | **14-day Free Trial**: Splunk Cloud Platform trial capped at 5 GB/day data ingestion; no credit card required (Self-hosted Splunk Free tier offers 500 MB/day free forever, single-user, no alerting). | SIEM and analytics platform with Druva App/Add-on integration for ingesting backup events; enables centralized monitoring, correlation of backup telemetry with security events, and custom dashboards for operational and compliance reporting. |
| **[Datadog Infrastructure Analytics](https://www.datadoghq.com/)** | **~$40B Market Cap** *(FY24 Rev: $2.68B)* | **$15.00/host/month** (Infrastructure Pro, billed annually or $18 on-demand) | **Free Forever Tier**: Free for up to 5 hosts with 1-day metric retention (14-day full Pro free trial also available with unlimited hosts). | General-purpose observability platform with infrastructure monitoring, log management, and custom dashboards; can ingest backup telemetry via integrations for unified monitoring alongside application and cloud infrastructure metrics. |
| **[Rubrik Security Cloud Reports](https://www.rubrik.com/)** | **~$21B Market Cap** *(NYSE: RBRK; FY25 Rev: ~$900M+)* | **$130.00/TB/month** (~$1,560/TB/year for infrastructure BETB; SaaS M365 edition starts at $3.80–$6.00/user/month) | **30-day Free Trial / PoC**: Guided proof of concept; SaaS trials typically capped at 500 users and up to 10 TB data protection capacity; requires sales coordination. | API-driven reporting for workload metrics including storage usage, compliance status, SLA assignment, protection status, and backup activity; integrates with Grafana via community plugins for custom dashboards and capacity forecasting. |
| **[Veeam ONE](https://www.veeam.com/)** | **$15B Valuation** *(2024 secondary; $1.7B+ ARR)* | **$12.90/workload/month** (packaged at ~$155–$230/workload/year under Veeam Universal Licensing / Data Platform) | **Free Forever Tier (Community Edition)**: Free forever for up to 10 workloads/instances (7-day monitoring history, 24-hr report retention); 30-day full-feature trial for unrestricted workloads. | Monitoring and analytics suite for Veeam-protected environments with 340+ prebuilt alarms, 150+ reports, capacity planning for VMware/Hyper-V/backup storage, chargeback billing, and ransomware anomaly alerts across backup infrastructure. |
| **[Cohesity Analytics (IT Analytics)](https://www.cohesity.com/)** | **~$7B+ Valuation** *(Merged with Veritas Enterprise; FY24 Pro Forma Rev: $1.7B)* | **$242.50/TB/month** ($29,100/year for 10 Back-End TB minimum entry block on AWS Marketplace; quote-based multi-year terms) | **30-day Free Trial**: Full access to Cohesity DataProtect as a Service / Cloud Services; requires partner/marketplace registration or PoC request. | Unified IT analytics platform with dashboards for backup/storage insights, predictive capacity planning, SLA/RTO/RPO compliance tracking, ransomware detection, and chargeback/showback; now available as SaaS with Cohesity Copilot for natural-language report generation. |
| **[Commvault Report Manager (Command Center)](https://documentation.commvault.com/)** | **~$6.8B Market Cap** *(NASDAQ: CVLT; FY25 Rev: $996M)* | **$58.50/TB/month** (Commvault Cloud File & Object storage backup; M365 protection from $1.70–$4.50/user/month) | **30-day Free Trial**: Commvault Cloud free evaluation across hybrid cloud workloads, databases, and SaaS applications; no credit card required. | Centralized reporting suite with predefined reports for backup/restore summaries, SLA compliance, storage utilization, CommCell readiness, and audit trails; supports automated scheduled report delivery and multi-CommCell monitoring. |
| **[Druva Analytics and Reporting](https://www.druva.com/)** | **~$2B Valuation** *(Last priced Series H; ~$200M+ ARR)* | **$8.00/user/month** (Endpoints/SaaS protection starting tier; hybrid storage backup starts via credit packs based on deduplicated TB volume) | **30-day Free Trial**: Full access to cloud data protection platform, workload configuration, and analytics features; no credit card required. | Cloud platform reports covering backup/restore operations, storage consumption, license usage, alert history, and workload health; supports granular insights, chargeback analysis, and up to two years of historical trend data for compliance audits. |

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
