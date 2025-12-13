# Demo SOC — Simulated Security Operations Center

> A compact, hands-on SOC lab showcasing centralized logging, IDS/IPS detection, WAF-like filtering, and incident handling across a multi-OS environment.

![Architecture](/assets/Architecture.png)

## Tech Badges

Core Stack:

![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-2D63FF)
![Suricata](https://img.shields.io/badge/Suricata-IDS%2FIPS-orange)
![Nginx](https://img.shields.io/badge/Nginx-Load%20Balancer-009639?logo=nginx&logoColor=white)
![OWASP Juice Shop](https://img.shields.io/badge/OWASP-Juice%20Shop-000000?logo=owasp&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?logo=docker&logoColor=white)

Platforms & Infra:

![Ubuntu](https://img.shields.io/badge/Ubuntu-24.04%20LTS-E95420?logo=ubuntu&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-10%20Pro-0078D6?logo=windows&logoColor=white)
![ParrotOS](https://img.shields.io/badge/ParrotOS-Attacker-00A35C)
![VirtualBox](https://img.shields.io/badge/Oracle-VirtualBox-183A61?logo=virtualbox&logoColor=white)
![VMware](https://img.shields.io/badge/VMware-Workstation-607078?logo=vmware&logoColor=white)

Attack & Test Tooling:

![Hydra](https://img.shields.io/badge/Hydra-Brute%20Force-444444)
![smbclient](https://img.shields.io/badge/smbclient-SMB-2C3E50)
![cURL](https://img.shields.io/badge/cURL-HTTP%20Tests-073551)
![Nmap](https://img.shields.io/badge/Nmap-Network%20Scan-4B8BBE)

## Overview

- Centralized event collection and correlation with `Wazuh` (SIEM)
- Network-level detection/prevention with `Suricata` IDS/IPS (incl. anti-XSS rules)
- Request routing and basic WAF-like filtering via `Nginx`
- PoC attacks: SSH brute-force, SMB auth attempts, XSS against Juice Shop
- Multi-OS lab: Ubuntu + Windows + ParrotOS with DNS-esque routing via hosts files

## Quick Start

- Nginx config: `configs/nginx.conf`
- Suricata rules (XSS PoC): `configs/xss.rules`
- Wazuh agent configs:
	- Ubuntu: `configs/ubuntu/ossec.conf`
	- Windows: `configs/windows/ossec.conf`
- Hosts entries used for name resolution:
	- Ubuntu/Parrot: `configs/ubuntu/hosts`
	- Windows: `configs/windows/hosts`

## Demo & Reports

- Report: `reports/GalievNguenZevadskii_report.md`
- Demo video: `recordings/GalievNguenZavadskii-demo.mp4`

## Authors

- [Galiev Arsen](https://github.com/projacktor) — a.galiev@innopolis.university
- [Nguen Ilya-Linh](https://github.com/ilyalinhnguyen) — i.nguen@innopolis.university
- [Zavadskii Peter](https://github.com/Abraham14711) — p.zavadskii@innopolis.university

## Why This Lab

This tested emphasizes the importance of centralized telemetry and layered defenses. It provides a reproducible foundation for expanding into SOAR, CTI integration, and hybrid cloud deployments while validating detection logic with realistic attack simulations.

 