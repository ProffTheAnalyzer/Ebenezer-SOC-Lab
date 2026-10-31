# Ebenezer SOC Lab — Hands-on Cybersecurity Portfolio

Lab write-ups migrated from the **published EB Practice Lab Google Sites export** (October 30, 2026). The projects focus on SOC engineering, detection, incident analysis, threat simulation, identity controls, and Microsoft security platforms.

> **Source:** The eight original labs were migrated from the published Google Sites Takeout export (October 30, 2026). The Wazuh deployment was documented separately using screenshots from October 30–31, 2026. These are personal lab records; results have not been independently retested.

## Labs

### Microsoft Sentinel and Defender XDR labs

| Lab | Focus | Screenshots |
|---|---|---:|
| [Lab Setup & VM Onboarding](labs/01-vm-setup-and-onboarding/README.md) | May 2026 | 35 |
| [Atomic Red Team Simulation & Detection](labs/02-atomic-red-team-simulation/README.md) | May 2026 | 14 |
| [Cloud Storage Phishing — Email Header & Payload Analysis](labs/03-cloud-storage-phishing-analysis/README.md) | Not specified | 15 |
| [Custom Analytic Rule & Detection](labs/04-custom-analytic-rules/README.md) | March 2026 | 19 |
| [Basic Sentinel Playbooks via Logic Apps](labs/05-sentinel-logic-apps-automation/README.md) | March 2026 | 15 |
| [Conditional Access Policy Test](labs/06-conditional-access-policy/README.md) | May 2026 | 22 |
| [Microsoft Sentinel Workbooks](labs/07-sentinel-workbooks/README.md) | Not specified | 9 |
| [Email Policies & Threat Protection](labs/08-defender-email-threat-protection/README.md) | Not specified | 21 |

## Wazuh SIEM/XDR Lab

[Wazuh XDR/SIEM — Ubuntu Server Installation & Windows 11 Agent Onboarding](labs/wazuh-siem/README.md) — 17 screenshots covering VirtualBox networking, SSH access, installation troubleshooting, the Wazuh dashboard, Windows agent registration, and initial event collection. Sysmon and custom detection testing remain future work.

## Background

The original portfolio also includes an [About page](ABOUT.md) and [Home page content](source-home-content.md).

## Publication checks

- Review every screenshot for identities, tenant IDs, email addresses, IPs, credentials, access tokens, internal hostnames and other details you do not want searchable on GitHub.
- Verify any documented claims and references before treating them as production guidance.
- Do not upload a real `.env`, password, API key, tenant secret, or live configuration file.
- Keep the original Google Sites Takeout archive in private backups. The eight migrated labs use PUBLISHED content and exclude Google Sites HTML/JavaScript wrappers.

## Original public website

[EB Practice Lab](https://www.ebpracticelab.org/)

## Documentation workflow

New labs use [LAB_TEMPLATE.md](LAB_TEMPLATE.md). Add a short project overview, tested setup and troubleshooting steps, supporting screenshots, observed security telemetry, and next steps. Wazuh installer credentials and other secrets are excluded from this public portfolio.
