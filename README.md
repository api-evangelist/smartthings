# Samsung SmartThings

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

Samsung SmartThings is a smart-home IoT platform for connecting, controlling, and automating devices across a home. The SmartThings API is a RESTful interface (base https://api.smartthings.com/v1) that lets integrations control devices, read device status, manage locations, rooms, and modes, build automations with Rules and Scenes, define and inspect capabilities, and build SmartApps that subscribe to events and run schedules. Authentication is via a Personal Access Token (PAT) for testing or OAuth 2.0 for production integrations. SmartThings publishes a real OpenAPI/Swagger definition at swagger.api.smartthings.com/public/st-api.yml. Event delivery is push-based over HTTP webhooks (SmartApp lifecycle callbacks and the Enterprise Eventing API sinks/subscriptions), not a public WebSocket.

**Areas:** Smart Home · IoT · Home Automation · Devices · Samsung

## Samsung SmartThings on APIs.io

Everything profiled for Samsung SmartThings is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/smartthings/](https://apis.io/providers/smartthings/)** — or go straight to one of the APIs or properties below.

### APIs (14)

- [Samsung SmartThings Apps API](https://apis.io/apis/smartthings/smartthings-apps-api/) — SmartApp registrations (Lambda or webhook endpoints).
- [Samsung SmartThings Capabilities API](https://apis.io/apis/smartthings/smartthings-capabilities-api/) — Standard and custom capability definitions.
- [Samsung SmartThings Device Commands & Status API](https://apis.io/apis/smartthings/smartthings-device-commands-status-api/) — Execute commands, create events, and read device/component/capability status.
- [Samsung SmartThings Devices API](https://apis.io/apis/smartthings/smartthings-devices-api/) — Access, control, install, update, and delete devices.
- [Samsung SmartThings History API](https://apis.io/apis/smartthings/smartthings-history-api/) — Event history for devices and locations.
- [Samsung SmartThings Installed Apps API](https://apis.io/apis/smartthings/smartthings-installed-apps-api/) — Per-user installations of a SmartApp.
- [Samsung SmartThings Locations API](https://apis.io/apis/smartthings/smartthings-locations-api/) — Locations (homes) and their Modes.
- [Samsung SmartThings Presentations API](https://apis.io/apis/smartthings/smartthings-presentations-api/) — Device presentation and configuration metadata.
- [Samsung SmartThings Rooms API](https://apis.io/apis/smartthings/smartthings-rooms-api/) — Groupings of devices within a Location.
- [Samsung SmartThings Rules API](https://apis.io/apis/smartthings/smartthings-rules-api/) — Condition/action Automations over connected devices.
- [Samsung SmartThings Scenes API](https://apis.io/apis/smartthings/smartthings-scenes-api/) — Saved sets of device states that can be executed on demand.
- [Samsung SmartThings Schedules API](https://apis.io/apis/smartthings/smartthings-schedules-api/) — Future/cron executions for Installed Apps.
- [Samsung SmartThings Subscriptions API](https://apis.io/apis/smartthings/smartthings-subscriptions-api/) — Event subscriptions for Installed Apps.
- [Samsung SmartThings Virtual Devices API](https://apis.io/apis/smartthings/smartthings-virtual-devices-api/) — Software devices for testing automations and integrations.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Smartthings Agentic Access](https://apis.io/agentic-access/smartthings/smartthings-agentic-access/)

#### Collections (15)

Postman and Open Collection request collections.

- [Samsung SmartThings API](https://apis.io/collections/smartthings/open-smartthings/)
- [Samsung SmartThings Apps API](https://apis.io/collections/smartthings/open-smartthings-apps-api/)
- [Samsung SmartThings Apps Capabilities API](https://apis.io/collections/smartthings/open-smartthings-capabilities-api/)
- [Samsung SmartThings Apps Device Commands & Status API](https://apis.io/collections/smartthings/open-smartthings-device-commands-status-api/)
- [Samsung SmartThings Apps Devices API](https://apis.io/collections/smartthings/open-smartthings-devices-api/)
- [Samsung SmartThings Apps History API](https://apis.io/collections/smartthings/open-smartthings-history-api/)
- [Samsung SmartThings Apps Installed Apps API](https://apis.io/collections/smartthings/open-smartthings-installed-apps-api/)
- [Samsung SmartThings Apps Locations API](https://apis.io/collections/smartthings/open-smartthings-locations-api/)
- [Samsung SmartThings Apps Presentations API](https://apis.io/collections/smartthings/open-smartthings-presentations-api/)
- [Samsung SmartThings Apps Rooms API](https://apis.io/collections/smartthings/open-smartthings-rooms-api/)
- [Samsung SmartThings Apps Rules API](https://apis.io/collections/smartthings/open-smartthings-rules-api/)
- [Samsung SmartThings Apps Scenes API](https://apis.io/collections/smartthings/open-smartthings-scenes-api/)
- [Samsung SmartThings Apps Schedules API](https://apis.io/collections/smartthings/open-smartthings-schedules-api/)
- [Samsung SmartThings Apps Subscriptions API](https://apis.io/collections/smartthings/open-smartthings-subscriptions-api/)
- [Samsung SmartThings Apps Virtual Devices API](https://apis.io/collections/smartthings/open-smartthings-virtual-devices-api/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Smartthings Authentication](https://apis.io/security/smartthings/smartthings-authentication/)
- [Smartthings Domain Security](https://apis.io/security/smartthings/smartthings-domain-security/)
- [Smartthings Vulnerability Disclosure](https://apis.io/security/smartthings/smartthings-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Smartthings Scopes](https://apis.io/scopes/smartthings/smartthings-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Smartthings Plans Pricing](https://apis.io/plans/smartthings/smartthings-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Smartthings Rate Limits](https://apis.io/rate-limits/smartthings/smartthings-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Smartthings Finops](https://apis.io/finops/smartthings/smartthings-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.smartthings.com)
- [Documentation](https://developer.smartthings.com/docs)
- [GitHub](https://github.com/SmartThingsCommunity)

## API Evangelist rating

**Kin Score 26.2** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 40.2 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 29.8 |
| Access clarity | 5.3 |

**Agent readiness 20.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 27.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/smartthings/](https://apis.io/providers/smartthings/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Samsung SmartThings: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/smartthings/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
