# Singtel (singtel)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
