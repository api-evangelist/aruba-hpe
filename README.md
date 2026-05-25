# HPE Aruba Networking (aruba-hpe)

HPE Aruba Networking is the networking business unit of Hewlett Packard Enterprise (NYSE HPE), born of Aruba Networks (founded 2002, acquired by HPE in 2015) and reinforced by the acquisitions of Silver Peak (SD-WAN, 2020), Pensando (smart switches / DPUs, 2022), and Axis Security (SSE, 2023). Its portfolio covers campus and branch Wi-Fi, AOS-CX and AOS-Switch data-center and campus switching, the Aruba Central cloud management plane, ClearPass network access control, EdgeConnect SD-WAN, the HPE Aruba Networking SSE cloud security service, the User Experience Insight (UXI) synthetic-monitoring sensors, and the HPE Aruba Networking Fabric Composer data-center fabric controller. Aruba is one of the most API-first vendors in enterprise networking — its developer hub publishes REST, streaming, and webhook documentation, and its GitHub org carries 50+ public repositories including official Python SDKs, a Go SDK, Ansible collections, a Terraform provider, the Network Analytics Engine script library, and YANG models that back AOS-CX.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/aruba-hpe/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Networking, Switching, Wi-Fi, SD-WAN, NAC, Network Access Control, Cloud Networking, AIOps, Data Center, Campus, Branch, Edge, SSE, SASE, HPE

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### HPE Aruba Networking Central REST API
Primary programmatic surface for the Aruba Central cloud network management platform. Covers configuration, monitoring, AIOps, troubleshooting, AppRF visibility, user management, and MSP workflows across Aruba access points, AOS-CX and AOS-Switch hardware, and gateways. OAuth 2.0 via the Central API Gateway. Regional gateways for US, EU, APAC, Canada, and China clusters. Documented at v2.5.8.

**Human URL:** [https://devhub.arubanetworks.com/docs/aruba-central](https://devhub.arubanetworks.com/docs/aruba-central)

### HPE Aruba Networking Central Streaming API
Real-time telemetry and event streams (location, presence, AppRF, audit, security, monitoring) over a long-lived connection. Official Python streaming client published through the developer hub.

### HPE Aruba Networking Central Webhooks
Alert and event delivery to external endpoints with HMAC-authenticated payloads. Standard integration path for ITSM, SIEM, and SOAR tooling reacting to Central alerts.

### AOS-CX REST API
On-box REST API running on every AOS-CX switch (CX 6000/8000/9000/10000 series). Exposes the full configuration and state surface — system, VRFs, VLANs, interfaces, LAGs, OSPF, BGP, EVPN, VSF, VSX, ACLs, QoS — backed by a YANG model. Foundation for pyaoscx, aoscxgo, the AOS-CX Ansible collection, and the AOS-CX Terraform provider.

**Repo:** [https://github.com/aruba/pyaoscx](https://github.com/aruba/pyaoscx)

### HPE Aruba Networking ClearPass Policy Manager REST API
Network access control surface — endpoints, devices, guests, onboarded users, sessions, policies, certificates, TACACS, and OnGuard posture. Integration backbone for ClearPass Exchange partners. Wrapped by the official pyclearpass Python SDK.

**Repo:** [https://github.com/aruba/pyclearpass](https://github.com/aruba/pyclearpass)

### HPE Aruba Networking EdgeConnect Orchestrator API
SD-WAN orchestration (formerly Silver Peak Orchestrator) — appliances, business intent overlays, tunnels, segments, application definitions, security policies, performance telemetry. Wrapped by pyedgeconnect.

**Repo:** [https://github.com/aruba/pyedgeconnect](https://github.com/aruba/pyedgeconnect)

### HPE Aruba Networking Fabric Composer API
Data-center fabric provisioning across AOS-CX leaf-spine, VSX, and EVPN-VXLAN deployments. Wrapped by pyafc and the hpeanfc-ansible-collection.

**Repo:** [https://github.com/aruba/pyafc](https://github.com/aruba/pyafc)

### HPE Aruba Networking User Experience Insight API
UXI sensor cloud API — synthetic test results, sensor health, network and SaaS application performance scores, incident data. Wrapped by pyhpeuxi.

**Repo:** [https://github.com/aruba/pyhpeuxi](https://github.com/aruba/pyhpeuxi)

### HPE Aruba Networking SSE API
Cloud-delivered ZTNA, SWG, and CASB surface from the Axis Security / HPE SSE platform — policy management, user and device enrollment, event reporting. Wrapped by pyhpesse.

**Repo:** [https://github.com/aruba/pyhpesse](https://github.com/aruba/pyhpesse)

### AOS-CX Network Analytics Engine (NAE)
On-box programmable telemetry and analytics framework that runs Python agents inside AOS-CX switches. The nae-scripts repo carries analytics agents for BGP, OSPF, EVPN, link health, hardware counters, and security events.

**Repo:** [https://github.com/aruba/nae-scripts](https://github.com/aruba/nae-scripts)

## Developer Resources

- **Developer Hub:** [https://devhub.arubanetworks.com](https://devhub.arubanetworks.com)
- **Developer Portal (redirect):** [https://developer.arubanetworks.com](https://developer.arubanetworks.com)
- **GitHub org:** [https://github.com/aruba](https://github.com/aruba) (50+ public repos under the HPE Networking org)
- **Community:** [Airheads Community](https://community.arubanetworks.com/)
- **Blog:** [Aruba Blog](https://www.arubanetworks.com/blog/)
- **Support:** [Aruba Support Portal](https://asp.arubanetworks.com/)
- **Parent:** [Hewlett Packard Enterprise](https://www.hpe.com)

## Official SDKs and Tooling

| Project | Language | Purpose |
|---|---|---|
| [pycentral](https://github.com/aruba/pycentral) | Python | Aruba Central SDK |
| [pyaoscx](https://github.com/aruba/pyaoscx) | Python | AOS-CX SDK |
| [pyclearpass](https://github.com/aruba/pyclearpass) | Python | ClearPass SDK |
| [pyedgeconnect](https://github.com/aruba/pyedgeconnect) | Python | EdgeConnect / Orchestrator SDK |
| [pyafc](https://github.com/aruba/pyafc) | Python | Fabric Composer SDK |
| [pyhpeuxi](https://github.com/aruba/pyhpeuxi) | Python | UXI SDK |
| [pyhpesse](https://github.com/aruba/pyhpesse) | Python | HPE SSE SDK |
| [pyarubaimc](https://github.com/aruba/pyarubaimc) | Python | Aruba IMC SDK |
| [aoscxgo](https://github.com/aruba/aoscxgo) | Go | AOS-CX SDK |
| [aruba-central-ansible-collection](https://github.com/aruba/aruba-central-ansible-collection) | Ansible | Central automation |
| [aoscx-ansible-collection](https://github.com/aruba/aoscx-ansible-collection) | Ansible | AOS-CX automation |
| [aos-switch-ansible-collection](https://github.com/aruba/aos-switch-ansible-collection) | Ansible | AOS-Switch automation |
| [hpeanfc-ansible-collection](https://github.com/aruba/hpeanfc-ansible-collection) | Ansible | Fabric Composer automation |
| [terraform-provider-aoscx](https://github.com/aruba/terraform-provider-aoscx) | Terraform | AOS-CX provider |
| [central-automation-studio](https://github.com/aruba/central-automation-studio) | JS / Web | Graphical front-end for Central API workflows |
| [aoscx-yang](https://github.com/aruba/aoscx-yang) | YANG | AOS-CX data models |
| [nae-scripts](https://github.com/aruba/nae-scripts) | Python | AOS-CX on-box analytics agents |

## Key Features

- Aruba Central — single-pane cloud network management for AP, switch, gateway, SD-WAN
- AOS-CX — modern switch OS with full on-box REST API and YANG models
- AOS-Switch — classic Aruba (HPE ProCurve lineage) switching automation
- ClearPass Policy Manager — RADIUS / TACACS / 802.1X NAC with REST API and ClearPass Exchange ecosystem
- EdgeConnect SD-WAN (Silver Peak) — Orchestrator and on-box APIs with business intent overlays
- HPE Aruba Networking Fabric Composer — EVPN-VXLAN leaf-spine fabric automation
- User Experience Insight (UXI) — synthetic sensors for Wi-Fi, wired, and SaaS
- HPE Aruba Networking SSE — cloud SASE / ZTNA / SWG / CASB (Axis Security)
- Network Analytics Engine (NAE) — on-box Python analytics inside AOS-CX
- Aruba IoT Operations — BLE / Zigbee / USB IoT gateway services on Aruba APs
- Aruba Central API Gateway with OAuth 2.0 and per-customer API tokens
- HMAC-signed webhooks for Central alerts and events
- Streaming API for real-time monitoring, location, presence, and AppRF telemetry
- Backed by Hewlett Packard Enterprise — public NYSE company, Fortune 500

## Maintainers

- **Kin Lane** — info@apievangelist.com — [apievangelist.com](https://apievangelist.com) — X: [@apievangelist](https://x.com/apievangelist)

## Specification

`specificationVersion: '0.16'` (APIs.yml / APIs.json)
