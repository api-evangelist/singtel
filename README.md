# Singtel (singtel)

Singtel (Singapore Telecommunications Limited) is Singapore's largest mobile network operator and the anchor communications group of Southeast Asia, with a regional footprint that includes Optus in Australia and associate stakes in Airtel, AIS, Globe and Telkomsel. In the network-API value chain Singtel sits on the supply side: it owns the mobile network signals — SIM, line, device, location, call state — that the CAMARA specifications turn into callable APIs, and it packages them for Singapore as SingVerify, a five-API anti-fraud and identity suite built on the GSMA Open Gateway framework. It also operates Paragon, its own 5G/edge/network orchestration platform, which powers the Bridge Alliance API Exchange (BAEx), and it is one of the twelve carrier equity partners in Aduna, the Ericsson-led joint venture that aggregates operator network APIs into a single global commercial channel.

Its API posture, however, is partner-gated and sales-led. As of July 2026 there is no first-party developer portal, no published OpenAPI, no sandbox, no SDKs and no self-serve signup. Developers reach Singtel's network capabilities through aggregators rather than directly from Singtel.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/singtel/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/singtel/refs/heads/main/apis.yml)

## Tags

- Telecommunications
- Singapore
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Anti-Fraud
- CPaaS
- Messaging
- Voice
- IoT
- 5G
- Edge Computing
- Aduna
- Partner Gated

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## Developer surface

There is none. Every developer-portal hostname probed on 2026-07-25 failed to resolve:

| Probe | Result |
| --- | --- |
| `developer.singtel.com` | NXDOMAIN |
| `developers.singtel.com` | NXDOMAIN |
| `docs.singtel.com` | NXDOMAIN |
| `opengateway.singtel.com` | NXDOMAIN |
| `developers.opengateway.singtel.com` | NXDOMAIN |
| `paragon.singtel.com` | NXDOMAIN |
| `api.singtel.com/` | 404 (resolves behind Imperva WAF) |
| `www.singtel.com/developer` | 404 |
| `www.singtel.com/developers` | 404 |
| `www.singtel.com/opengateway` | 404 |
| `www.singtel.com/business/api` | 404 |
| `baex.bridgealliance.com/` | 200 — login wall, "private site reserved for approved BAEx partners" |

The `www.singtel.com` business sitemap contains no documentation path of any kind. Every API page terminates in an enterprise enquiry form. No OpenAPI or Swagger document was found (`/openapi.json`, `/swagger.json`, `/api-docs` all 404), there is no `singtel` GitHub organization, no public Postman workspace, no first-party SDKs, no webhook catalogue and no published authentication scheme.

## CAMARA posture

Genuine CAMARA participant on the supply side, with nothing callable from Singtel itself. SingVerify is a real, commercially sold implementation — not a press release — and a Singtel engineer has signed the CAMARA contributor licence agreement and filed a substantive security issue against the Number Verification auth flow. But a developer cannot obtain a spec, an endpoint or a sandbox from Singtel.

CAMARA APIs with real evidence:

- **Number Verification** — SingVerify Number Verify API (federated with M1 for national coverage)
- **SIM Swap** — SingVerify SIM Swap API
- **Device Location / Location Verification** — SingVerify Device Location API
- **Device Roaming Status / Device Status** — SingVerify Device Roaming API
- **Anti-fraud / Scam Signal** — SingVerify Scam Sniffer API (Singtel-branded)

Not found: Quality on Demand, Carrier Billing, KYC Match, Device Swap, Population Density.

**GSMA Open Gateway:** signatory to the MoU; SingVerify is described as built on the Open Gateway framework. No branded Open Gateway developer portal exists.

**Aduna:** Singtel is one of twelve CSP equity partners in the Ericsson joint venture (transaction completed July 2025).

**TM Forum:** no Open API conformance certificate found published for Singtel.

**Auth:** undocumented. CAMARA specifies OIDC and CIBA; no CIBA endpoint, no OIDC discovery document and no scopes are exposed on any Singtel host.

## Channel to developers

Aggregator-only. The routes to Singtel's network capabilities are Aduna and its platform partners (Vonage, Sinch, Infobip, Google Cloud), the Bridge Alliance API Exchange for regional coverage, identity vendors such as IPification, or a direct enterprise sales conversation.

## APIs

### SingVerify Number Verify API

Network-based verification that the mobile number a user declares is the number of the SIM the request is actually coming from, used to replace or reinforce SMS OTP.

- **Human URL:** [https://www.singtel.com/business/products-services/mobility/singverify/types-of-api](https://www.singtel.com/business/products-services/mobility/singverify/types-of-api)

### SingVerify SIM Swap API

Real-time signal indicating whether the SIM bound to a mobile number has been changed recently, to block account-takeover attempts that rely on intercepting SMS one-time passcodes.

- **Human URL:** [https://www.singtel.com/business/products-services/mobility/singverify/types-of-api](https://www.singtel.com/business/products-services/mobility/singverify/types-of-api)

### SingVerify Device Location API

Verifies whether a mobile device is within an expected area or country at the time of a login or transaction, using network-derived location rather than handset GPS.

- **Human URL:** [https://www.singtel.com/business/products-services/mobility/singverify/types-of-api](https://www.singtel.com/business/products-services/mobility/singverify/types-of-api)

### SingVerify Device Roaming API

Reports whether a subscriber's device is currently roaming outside Singapore, used as a risk signal in fraud and authentication decisions.

- **Human URL:** [https://www.singtel.com/business/products-services/mobility/singverify](https://www.singtel.com/business/products-services/mobility/singverify)

### SingVerify Scam Sniffer API

Detects whether a user is on an active voice call at the moment they attempt a high-value transaction, to interdict authorised-push-payment and social-engineering fraud.

- **Human URL:** [https://www.singtel.com/business/products-services/mobility/singverify/types-of-api](https://www.singtel.com/business/products-services/mobility/singverify/types-of-api)

### Singtel CPaaS SMS API

Application-to-person SMS sending and receiving for business applications.

- **Human URL:** [https://www.singtel.com/business/products-services/mobility/mobility-solutions/singtel-cpaas/sms-api](https://www.singtel.com/business/products-services/mobility/mobility-solutions/singtel-cpaas/sms-api)

### Singtel CPaaS Voice API

Programmable voice / VoIP calling embedded into business applications.

- **Human URL:** [https://www.singtel.com/business/products-services/mobility/mobility-solutions/singtel-cpaas/voice-api](https://www.singtel.com/business/products-services/mobility/mobility-solutions/singtel-cpaas/voice-api)

None of the seven publish a base URL, an authentication scheme, an API reference or a machine-readable specification.

## Links

- [Singtel](https://www.singtel.com/)
- [SingVerify](https://www.singtel.com/business/products-services/mobility/singverify)
- [Singtel CPaaS](https://www.singtel.com/business/products-services/mobility/mobility-solutions/singtel-cpaas)
- [Singtel Paragon](https://www.singtel.com/business/products-services/5g/paragon)
- [Bridge Alliance API Exchange (partner login)](https://baex.bridgealliance.com/)
- [Aduna](https://adunaglobal.com/)
- [CAMARA Project](https://camaraproject.org/)
- [LinkedIn](https://www.linkedin.com/company/singtel)
- [News releases](https://www.singtel.com/about-us/media-centre/news-releases)

## Maintainers

- **Kin Lane** — kin@apievangelist.com
