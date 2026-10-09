# Awesome-Security-Health-Assessment

# Top Security Health Assessment Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Cloud Security Posture, Compliance Assessment & Self-Hosted Security Scanners*  
**Last updated: October 2026**

This repository tracks notable **commercial security health assessment platforms** and **open-source projects** that evaluate an organization's security posture, identify misconfigurations, assess compliance against benchmarks, and generate prioritized remediation roadmaps.

**Examples** include Salesforce Health Check, AppOmni, Adaptive Shield, Wing Security, Palo Alto Prisma Cloud, Wiz, Orca Security, Tenable Cloud Security, Rapid7 InsightCloudSec, and Qualys Cloud Platform (the category leaders).

**Open-source emphasis**: Security health assessment is one of the strongest open-source domains. **Prowler** leads with 561 AWS checks, 139 Azure checks, 77 GCP checks, and 83 Kubernetes checks across 30+ compliance frameworks . **Fix Inventory** brings graph-based cloud security with 40+ base resource kinds for multi-cloud policy enforcement . **cnspec** delivers cross-platform policy-as-code spanning clouds, Kubernetes, SaaS, IaC, and IoT devices . **SentinelAudit** provides cross-platform endpoint security auditing with risk scoring . **Postura** delivers NIST CSF-based self-service assessment with prioritized PDF remediation reports . **ClosedSSPM** offers open-source SaaS security posture management . This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Salesforce Health Check](https://help.salesforce.com/)**  
  **Salesforce's built-in security assessment** — evaluates org settings against Salesforce's baseline security standards . **Provides actionable recommendations to improve security posture** . **Best for Salesforce orgs wanting native security assessment** .

- **[AppOmni](https://appomni.com/)**  
  **SaaS security posture management (SSPM)** — continuous monitoring and configuration assessment for SaaS applications . **Best for enterprise SaaS security** .

- **[Adaptive Shield](https://www.adaptiveshield.com/)**  
  **SaaS security posture management** — misconfiguration detection and remediation . **Best for SSPM** .

- **[Wing Security](https://www.wing.security/)**  
  **SaaS security platform** — discovery, posture management, and shadow IT detection . **Best for SaaS security automation** .

- **[Palo Alto Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)**  
  **Comprehensive CNAPP** — posture management, workload protection, and compliance . **Best for large enterprises** .

- **[Wiz](https://www.wiz.io/)**  
  **The leading CNAPP with graph-based attack path analysis** — agentless scanning with modern UX . **Best for multi-cloud organizations seeking modern UX and attack path context** .

- **[Orca Security](https://orca.security/)**  
  **Agentless CNAPP with SideScanning™ technology** . **Best for mid-market and enterprises wanting agentless scanning** .

- **[Tenable Cloud Security](https://www.tenable.com/)**  
  **CIEM and CSPM platform** (from Ermetic acquisition) — permissions analysis and posture management . **Best for multi-cloud entitlement management** .

- **[Rapid7 InsightCloudSec](https://www.rapid7.com/)**  
  **Cloud security posture management** — continuous compliance and risk assessment . **Best for Rapid7 ecosystem users** .

- **[Qualys Cloud Platform](https://www.qualys.com/)**  
  **Comprehensive security and compliance platform** — vulnerability management and cloud posture assessment . **Best for enterprise security programs** .

## Open-Source GitHub Projects

### Multi-Cloud Security Assessment

- **[Prowler](https://github.com/prowler-cloud/prowler)**  
  **The leading open-source cloud security assessment tool**, Apache-2.0 licensed . **561 AWS checks, 139 Azure checks, 77 GCP checks, and 83 Kubernetes checks** across 30+ compliance frameworks including CIS, NIST 800, NIST CSF, CISA, RBI, FedRAMP, PCI-DSS, GDPR, HIPAA, FFIEC, SOC2, GXP, AWS Well-Architected Framework Security Pillar, AWS Foundational Technical Review (FTR), and ENS (Spanish National Security Scheme) . **CLI with dashboard, Docker Compose deployment, and Prowler App web interface** . **Install via pip or containers** . **Best for comprehensive multi-cloud security assessment** .

- **[Fix Inventory](https://github.com/someengineering/fixinventory)**  
  **Graph-based cloud security posture management**, open-source . **Agentless collection of cloud infrastructure metadata** from AWS, GCP, Azure, and Kubernetes . **Normalizes data into a graph schema with 40+ base kinds** for common resources like database or ip_address . **Enables single set of policies across all clouds** . **Dependency and access graph** — queryable for risk analysis, blast radius, and privilege escalation paths . **Resource lifecycle tracking** with hourly snapshots and diff views . **Use cases**: CSPM, AI-SPM, cloud compliance, CIEM, cloud asset inventory, container/Kubernetes security, security data fabric, and policy-as-code . **Best for graph-based multi-cloud security assessment** .

- **[cnspec](https://github.com/mondoohq/cnspec)**  
  **Open-source, cloud-native security and policy project**, open-source . **Scans public and private clouds (AWS, GCP, Azure), Kubernetes clusters, containers and registries, server endpoints (Linux, macOS, Windows), SaaS platforms (Microsoft 365, Atlassian, Okta), infrastructure as code (Terraform HCL/plan/state), network hosts and DNS records, version control (GitHub, GitLab), IoT/OPC-UA devices, and VMware platforms** . **Policy-as-code engine built on a security data fabric** — codify checks and run at scale . **Default policies ship out of the box** . **Best for cross-platform policy enforcement** .

### Endpoint & Host Security Assessment

- **[SentinelAudit](https://github.com/APonder-Dev/sentinel-audit)**  
  **Cross-platform endpoint security auditing and assessment tool**, open-source . **Collects host posture telemetry** — system info, hostname, OS details, architecture, local IP, listening ports, firewall status, running processes with privilege context, and disk encryption status (BitLocker, FileVault, LUKS) . **Security findings engine** — analyzes firewall telemetry, risky listening ports (FTP, Telnet, RDP, VNC, SMB, database ports), privileged process counts, and disk encryption . **Risk scoring system** with severity penalties (High -20, Medium -10, Low -5) and ratings (Low Risk 90-100, Moderate Risk 70-89, Elevated Risk 50-69, High Risk 0-49) . **JSON and Markdown report exports** . **Python 3.12+ with Rich CLI output** . **Best for endpoint security auditing** .

- **[ohbs-host](https://pypi.org/project/ohbs-host/)**  
  **Host security benchmark scanner** with fleet scan, drift detection, and watch mode . **CIS benchmark-based scanning** with variables, waivers, and dry-run . **Fleet scan** aggregates results across multiple hosts into a single HTML/JSON report . **Drift detection** classifies rule changes (new failures, regressions, recoveries, waiver transitions) with CI exit codes . **Apply verification** reports which rules were fixed and which regressed due to remediation . **Watch mode** with edge-triggered, de-duplicated alerting — a rule alerts when it starts failing and again when it clears . **Export formats**: SARIF, XCCDF, JUnit, Prometheus . **Best for host security compliance scanning** .

### Compliance & Posture Assessment

- **[Postura](https://github.com/cypher-labs/postura)**  
  **Self-service NIST CSF security assessment tool**, open-source . **Scores organization's cybersecurity posture across 30 controls** covering all 5 NIST CSF functions (Identify, Protect, Detect, Respond, Recover) . **Weighted maturity scoring** (Priority 1=3, Priority 2=2, Priority 3=1) . **Gap classification** as Critical/High/Medium per failing control . **Radar chart visualization** and **PDF remediation report** with prioritized roadmap . **User accounts, assessment history, side-by-side compare, and anonymous mode** . **Python 3.10+ / Flask / SQLite / ReportLab** . **Best for NIST CSF-based security assessment** .

- **[closedsspm](https://pkg.go.dev/github.com/PiotrMackowski/ClosedSSPM/cmd/closedsspm)**  
  **Open-source SaaS Security Posture Management**, Go-based . **Audits SaaS platforms including Jira** . **Connector registry architecture** for adding new platforms . **Collects, evaluates, and exposes security findings via MCP** . **Best for SaaS security posture management** .

### Additional Strong Open-Source Options

- **ScoutSuite** — Multi-cloud security auditing tool from NCC Group for AWS, Azure, GCP, Alibaba Cloud, and Oracle Cloud . **Best for multi-cloud security audits** .
- **CloudSploit** — Cloud security scanner (acquired by Aqua Security) for misconfiguration detection . **Best for cloud misconfiguration detection** .
- **kube-bench** — Kubernetes CIS Benchmark checks . **Best for Kubernetes security assessment** .
- **Trivy** — Container and IaC vulnerability scanner . **Best for container and IaC security** .
- **Checkov** — IaC security scanning for Terraform, CloudFormation, and Kubernetes . **Best for IaC security assessment** .
- **tfsec** — Terraform security scanner . **Best for Terraform security assessment** .
- **ohbs-cloud** — Cloud security benchmark scanner with CIS controls for AWS, Azure, GCP, Alibaba, and Tencent . **Best for cloud compliance scanning** .
- **sentinel-audit** — Cross-platform endpoint security audit tool . **Best for endpoint posture assessment** .

**Frameworks for building custom security health assessment solutions**: Combine **Prowler** for comprehensive multi-cloud security assessment with 30+ compliance frameworks . Use **Fix Inventory** for graph-based cloud security with dependency and access analysis . Deploy **cnspec** for cross-platform policy-as-code spanning clouds, Kubernetes, SaaS, IaC, and IoT . Integrate **SentinelAudit** for endpoint security auditing with risk scoring . Choose **Postura** for NIST CSF-based organizational assessment with PDF remediation reports . Use **closedsspm** for SaaS security posture management . Note that true enterprise CNAPP with graph-based attack path analysis, agentless scanning, and executive UI (Wiz, Prisma Cloud, Orca) remains primarily commercial territory; open-source stacks provide strong multi-cloud assessment, endpoint auditing, and compliance foundations that require integration for complete security health assessment.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Security health assessment platforms handle sensitive infrastructure configuration data and may access cloud credentials. Self-hosted solutions require proper security hardening, read-only credentials, access controls, and compliance with data privacy regulations.
- **Assessment tools require read-only credentials** — never grant write access to assessment tools. Use dedicated service accounts with least-privilege policies for scanning .
- **Open-source covers 70-80% of basic needs** — Prowler + ScoutSuite + Steampipe combination is often sufficient for SMBs under 500 cloud resources. Commercial CNAPP (Wiz, Prisma Cloud) justifies cost for >500 resources with dedicated security teams, providing attack path context and executive UI .
- **License considerations**: Prowler uses Apache-2.0 , Fix Inventory is open-source , cnspec is open-source , SentinelAudit is open-source , Postura is open-source , and closedsspm is open-source . Verify licensing against your use case before committing.
- The open-source ecosystem provides strong multi-cloud assessment, endpoint auditing, and compliance foundations, but **graph-based attack path analysis, agentless scanning, and executive UI** remain primarily commercial offerings.

---

**Made for security engineers, cloud architects, and organizations seeking security health assessment sovereignty.**
Let's make security health assessment more open, transparent, and effective.
