# Awesome-Cloud-Workload-Protection-CWPP

## Top Cloud Workload Protection (CWPP) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Runtime Security, Agentless Scanning & Cloud-Native Application Protection*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Workload Protection (CWPP)**. These tools protect workloads running in cloud environments—VMs, containers, serverless functions, and Kubernetes clusters—by detecting vulnerabilities, misconfigurations, runtime threats, and anomalous behavior across multi-cloud and hybrid infrastructure.

**Examples** include Wiz, Palo Alto Prisma Cloud, Microsoft Defender for Cloud, Orca Security, Lacework (FortiCNAPP), CrowdStrike Falcon Cloud Workload, Sysdig Secure, Trend Micro Cloud One, Aqua Security, and Tenable Cloud Security (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted vulnerability scanning, runtime threat detection, and Kubernetes security—ideal for security engineers, platform teams, and organizations seeking transparent, vendor-neutral workload protection without per-workload enterprise pricing.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global **Cloud Workload Protection Platform (CWPP) solutions market** was valued at approximately **$21.4 billion (214亿元) in 2025** and is projected to reach **$42.95 billion (429.5亿元) by 2032**, growing at a CAGR of **10.6%** [citation:2]. Agent-based deployments accounted for **63.25%** of the market in 2025 due to deep kernel-level visibility, though **agentless models are scaling at 31.15% CAGR** as hyperscaler APIs mature [citation:15].

The sector is **moderately concentrated with intensifying competition**. The CWPP market includes established players (Palo Alto, Microsoft, Trend Micro, CrowdStrike) alongside high-growth challengers (Wiz, Orca, Sysdig) [citation:2][citation:15]. However, no single vendor dominates—Lacework's valuation collapse from **$8.3 billion to $152.3 million** in three years before its Fortinet acquisition illustrates how quickly market position can shift in this space [citation:7]. The market is far from winner-take-all; open-source tooling (Trivy, Falco, Prowler) and modular point solutions continue to hold significant ground alongside converged CNAPP platforms.

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Wiz](https://www.wiz.io/)** | Agentless CNAPP with graph-based risk prioritization, CSPM, CIEM, and DSPM. Full multi-cloud platform is quote-only, but base tiers are published via AWS Marketplace . | Wiz Essential: **$24,000/yr** (100 workloads, ~$240/workload/yr); Wiz Advanced: **$38,000/yr** (100 workloads); Go Bundle: **$222,000/36 months** (~$74,000/yr) . | **No free tier**; no monthly option; enterprise-only pricing . |
| **[Microsoft Defender for Cloud](https://azure.microsoft.com/en-us/pricing/details/defender-for-cloud/)** | Unified CNAPP with CSPM, workload protection for servers, containers, databases, storage, and APIs. Pay-as-you-go per resource type . | Defender for Servers P1: **$4.906/server/month**; P2: **$14.60/server/month**; Containers: **$6.8693/vCore/month**; SQL: **$15/instance/month** . | **Free**: foundational CSPM features included with Azure subscription; paid plans for advanced workload protection . |
| **[Orca Security](https://orca.security/)** | Agentless cloud security platform using SideScanning technology. Single all-inclusive SKU covering CNAPP, AppSec, and runtime. Pricing via AWS Marketplace private offer . | AWS Marketplace: Small-Medium tier **$124,440/yr**; Medium **$170,800/yr**; Large **$317,200/yr** . | No public free tier; trial via sales . |
| **[Palo Alto Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)** | Comprehensive CNAPP with credit-based licensing. Credits consumed by resource type (hosts, containers, serverless). Quote-only for full platform . | Quote-only (credit-based per resource type) . | No public free tier; trial via sales . |
| **[CrowdStrike Falcon Cloud Workload](https://www.crowdstrike.com/)** | Cloud workload protection extending Falcon's endpoint detection to cloud compute, containers, and Kubernetes . | Flex License: **$233.99** (3-year, per license via CDW) . | No public free tier; trial via sales . |
| **[Lacework (FortiCNAPP)](https://www.lacework.com/)** | Behavioral ML-based CNAPP (Polygraph engine) now integrated into Fortinet Security Fabric. Strong for Fortinet-committed organizations . | Quote-only (standalone or bundled with Fortinet) . | No public free tier; trial via Fortinet sales . |
| **[Sysdig Secure](https://sysdig.com/)** | Cloud-native security with runtime threat detection, CSPM, and compliance. Strong Kubernetes depth; requires agent deployment . | AWS Marketplace: **$72/host/month** (20-host minimum, ~$17,000/yr for 20 nodes) . | No public free tier; trial via sales . |
| **[Trend Micro Cloud One](https://www.trendmicro.com/)** | Workload security module within Trend Micro's CNAPP platform. Per-device subscription licensing . | **$385.03–$435.58** per device (government pricing via CDW) . | No public free tier; trial via sales . |
| **[Aqua Security](https://www.aquasec.com/)** | CNAPP platform with workload-based pricing. Trivy OSS is free; enterprise CNAPP custom-priced . | Enterprise: quote-only (workload-based) . | **Trivy OSS**: free open-source scanner; enterprise trial via sales . |
| **[Tenable Cloud Security](https://www.tenable.com/cloud-security)** | CNAPP with CSPM, CIEM, vulnerability management, and DSPM. Asset-based pricing scaled by billable cloud resources (VMs, containers, serverless) . | Quote-only (asset-based per billable resource) . | No public free tier; trial via sales . |
| **[Druva Cloud Workload Protection](https://www.druva.com/)** | Data protection and cyber resilience for cloud workloads (not a pure CWPP). Backup, DR, and ransomware detection for AWS/Azure VMs and databases . | Quote-only (per TB/month after deduplication) . | No free tier; trial via sales . |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Trivy](https://github.com/aquasecurity/trivy)** | [![Stars](https://img.shields.io/github/stars/aquasecurity/trivy?style=social&color=white)](https://github.com/aquasecurity/trivy/stargazers) | Comprehensive open-source security scanner for containers, Kubernetes, code repositories, and cloud environments. Detects vulnerabilities, misconfigurations, secrets, and licenses. The most widely adopted open-source CNAPP component; free forever (Apache 2.0). |
| **[Prowler](https://github.com/prowler-cloud/prowler)** | [![Stars](https://img.shields.io/github/stars/prowler-cloud/prowler?style=social&color=white)](https://github.com/prowler-cloud/prowler/stargazers) | Open-source cloud security posture management (CSPM) tool for AWS, Azure, GCP, and Kubernetes. 500+ checks mapped to CIS, PCI-DSS, HIPAA, and other frameworks. CLI and dashboard. |
| **[Falco](https://github.com/falcosecurity/falco)** | [![Stars](https://img.shields.io/github/stars/falcosecurity/falco?style=social&color=white)](https://github.com/falcosecurity/falco/stargazers) | CNCF runtime security tool for Kubernetes and containers. Detects anomalous activity using eBPF and syscall monitoring. Complements posture tools with runtime threat detection. |
| **[Kube-bench](https://github.com/aquasecurity/kube-bench)** | [![Stars](https://img.shields.io/github/stars/aquasecurity/kube-bench?style=social&color=white)](https://github.com/aquasecurity/kube-bench/stargazers) | Checks Kubernetes clusters against CIS Kubernetes Benchmark. Lightweight Go binary; runs as Job or CLI. Foundational for Kubernetes security posture validation. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Kube-hunter](https://github.com/aquasecurity/kube-hunter)** | [![Stars](https://img.shields.io/github/stars/aquasecurity/kube-hunter?style=social&color=white)](https://github.com/aquasecurity/kube-hunter/stargazers) | Penetration testing tool for Kubernetes clusters. Discovers weaknesses and attack vectors from an attacker's perspective. |
| **[CloudSploit](https://github.com/aquasecurity/cloudsploit)** | [![Stars](https://img.shields.io/github/stars/aquasecurity/cloudsploit?style=social&color=white)](https://github.com/aquasecurity/cloudsploit/stargazers) | Open-source cloud security scanning for AWS, Azure, GCP, Oracle, and GitHub. Detects misconfigurations and compliance risks. |

**Frameworks for building custom systems**: Combine **Trivy** for vulnerability and misconfiguration scanning, **Prowler** for multi-cloud CSPM checks, **Falco** for runtime threat detection, and **Kube-bench** for Kubernetes CIS compliance—creating a fully open-source CWPP stack without per-workload licensing.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Cloud workload protection platforms require broad read access to cloud APIs and workload metadata; enforce least-privilege IAM roles and audit data access.
- Pricing models (per-workload, per-host, per-credit) vary dramatically and are highly negotiable at enterprise scale; Wiz's published base tiers ($24K/yr for 100 workloads) and Sysdig's $72/host/month provide rare public reference points, but full CNAPP platforms remain quote-only [citation:5][citation:11]. Open-source tools require ongoing tuning and integration effort to match commercial coverage.

---

**Made for security engineers, cloud architects, SOC analysts, and organizations building cloud-native defense.**  
Let's make cloud workload protection more open, transparent, and cost-effective.
