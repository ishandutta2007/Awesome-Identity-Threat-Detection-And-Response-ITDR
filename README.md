# Awesome-Identity-Threat-Detection-And-Response-ITDR

## Top Identity Threat Detection and Response (ITDR) Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Active Directory & Identity Attack Detection, Credential Abuse Prevention, Privilege Escalation Visibility, Deception & Identity Resilience*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Identity Threat Detection and Response (ITDR)**. These solutions detect and respond to attacks targeting identity infrastructure—especially Active Directory, Entra ID, and authentication protocols—covering reconnaissance, credential theft, privilege escalation, lateral movement, and identity-based persistence.



**Examples** include Microsoft Defender for Identity, CrowdStrike Falcon Identity Protection, Silverfort, Tenable Identity Exposure, SentinelOne Singularity Identity, Semperis, Quest Software, Illusive Networks, Netwrix, and Attivo Networks (the category leaders).



**Open-source emphasis**: Production-grade, continuous ITDR with real-time sensors and automated response is dominated by commercial platforms. Strong open-source tooling exists for attack-path analysis, AD security assessment, and detection engineering—especially **BloodHound** and related projects. This section expands those while remaining realistic about the commercial gap.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Microsoft Defender for Identity](https://www.microsoft.com/en-us/security/business/siem-and-xdr/microsoft-defender-identity)**  

  Microsoft’s ITDR solution that deploys sensors on domain controllers to detect identity attacks and feeds signals into Microsoft Defender XDR.



- **[CrowdStrike Falcon Identity Protection](https://www.crowdstrike.com/products/identity-protection/)**  

  Identity threat detection and protection tightly integrated with the Falcon platform, correlating identity events with endpoint telemetry.



- **[Silverfort](https://www.silverfort.com/)**  

  Identity security platform providing inline MFA and protection for legacy protocols (Kerberos, NTLM, LDAP) and service accounts.



- **[Tenable Identity Exposure](https://www.tenable.com/products/tenable-identity-exposure)**  

  Continuous identity risk assessment and exposure management focused on Active Directory and hybrid identity environments.



- **[SentinelOne Singularity Identity](https://www.sentinelone.com/platform/singularity-identity/)**  

  Identity threat detection and deception capabilities (including former Attivo Networks technology) integrated with the Singularity platform.



- **[Semperis](https://www.semperis.com/)**  

  Specialist platform for Active Directory threat detection, prevention, and forest recovery / resilience.



- **[Quest Software](https://www.quest.com/)**  

  Suite of Active Directory management, auditing, recovery, and security tools used for identity hygiene and threat response.



- **[Illusive Networks](https://illusive.com/)**  

  Identity deception and attack-surface reduction platform (now part of broader identity security portfolios).



- **[Netwrix](https://www.netwrix.com/)**  

  Identity and access auditing, change monitoring, and threat detection focused on Active Directory and hybrid environments.



- **[Attivo Networks](https://www.attivo.com/)**  

  Identity deception and lateral-movement detection technology (now integrated into SentinelOne Singularity Identity).



## Open-Source GitHub Projects

- **[BloodHound](https://github.com/SpecterOps/BloodHound)**  

  Industry-standard open-source tool for mapping Active Directory attack paths, privilege relationships, and identifying high-risk identity configurations.



- **[SharpHound](https://github.com/SpecterOps/SharpHound)**  

  Data collector for BloodHound that enumerates Active Directory objects, sessions, and ACLs to build the attack-path graph.



- **[BloodHound Community Edition & related tools](https://github.com/SpecterOps)**  

  Official and community tooling around BloodHound for continuous or periodic identity attack-path analysis.



- **[ImproHound](https://github.com/improsec/ImproHound)**  

  Open-source tool that analyzes BloodHound data to identify attack paths that break intended Active Directory tiering models.



- **[NetworkHound and related AD topology tools](https://github.com/)**  

  Community projects that extend BloodHound-compatible graphs with network and infrastructure context.



- **[AD security assessment scripts (PowerView, ADRecon, etc.)](https://github.com/)**  

  Classic and modern open-source scripts for enumerating Active Directory configuration, trusts, and security posture.



- **[Velociraptor](https://github.com/Velocidex/velociraptor)**  

  Open-source endpoint visibility and digital forensics platform frequently used for identity-related incident response and hunting.



- **[Detection rules and Sigma for identity attacks](https://github.com/SigmaHQ/sigma)**  

  Community detection content targeting Kerberos attacks, credential dumping, Golden/Silver Ticket, and other identity threats.



- **[Documentation and BloodHound operational playbooks](https://bloodhound.specterops.io/)**  

  Guides for collecting data, analyzing attack paths, and integrating findings into detection and remediation workflows.



- **[Self-hosted identity deception and honeytoken projects](https://github.com/)**  

  Community approaches to deploying decoy accounts, SPNs, and canaries for early detection of identity reconnaissance.



### Additional Strong Open-Source Options

- Running **BloodHound** (and SharpHound collectors) on a regular cadence to surface attack paths and misconfigurations.

- Combining AD enumeration tools with SIEM detection rules for continuous monitoring.

- Using **Velociraptor** or similar for targeted identity incident response.

- Accepting that real-time domain-controller sensors, inline protocol protection, automated response, and managed AD recovery still require commercial ITDR platforms (Defender for Identity, CrowdStrike, Silverfort, Semperis, SentinelOne, etc.).

- Focusing open-source efforts on visibility, attack-path understanding, and detection engineering rather than full replacement of commercial ITDR.



**Frameworks for building custom systems**: Periodic BloodHound collection → attack-path analysis and prioritization → detection rules in SIEM/EDR → response playbooks with Velociraptor or native AD tools. Suitable for security teams with AD expertise. Most enterprises pair open tooling with commercial ITDR for continuous coverage and support.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- Identity threat tools interact with critical authentication infrastructure. Open-source collectors can generate noise or require careful scoping. This list is not operational or security advice.



---

**Made for identity security teams, blue teams, and open security tooling advocates.**

Let's keep identity attacks visible, containable, and as open as practical.
