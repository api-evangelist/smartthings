# Samsung SmartThings (smartthings)

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

Samsung SmartThings is a smart-home IoT platform for connecting, controlling, and automating devices across a home. The SmartThings API is a RESTful interface (base `https://api.smartthings.com/v1`) that lets integrations control devices, read device status, manage Locations, Rooms, and Modes, build Automations with Rules and Scenes, define and inspect Capabilities, and build SmartApps that subscribe to events and run Schedules. Authentication is via a Personal Access Token (PAT) for testing or OAuth 2.0 for production integrations, passed as `Authorization: Bearer {token}`. SmartThings publishes a real OpenAPI/Swagger definition at [swagger.api.smartthings.com/public/st-api.yml](https://swagger.api.smartthings.com/public/st-api.yml).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/smartthings/refs/heads/main/apis.yml)

## Tags

- Smart Home
- IoT
- Home Automation
- Devices
- Samsung

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### SmartThings Devices API

List, install, get, update, and delete the devices connected to a SmartThings account, and read a device's description, components, and health state.

- **Human URL:** [https://developer.smartthings.com/docs/devices/device-basics](https://developer.smartthings.com/docs/devices/device-basics)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Device Commands & Status API

Execute capability commands on a device, create device events, and read full device status or the status of a single component or capability.

- **Human URL:** [https://developer.smartthings.com/docs/devices/commands](https://developer.smartthings.com/docs/devices/commands)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Locations API

Create, list, get, update, and delete the Locations (homes) that group hubs, devices, and automations, and manage a Location's Modes and current Mode.

- **Human URL:** [https://developer.smartthings.com/docs/locations/locations](https://developer.smartthings.com/docs/locations/locations)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Rooms API

Create, list, get, update, and delete Rooms, which group devices within a Location.

- **Human URL:** [https://developer.smartthings.com/docs/locations/rooms](https://developer.smartthings.com/docs/locations/rooms)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Scenes API

Create, list, get, update, delete, and execute Scenes - saved sets of device states that can be triggered on demand.

- **Human URL:** [https://developer.smartthings.com/docs/automations/scenes](https://developer.smartthings.com/docs/automations/scenes)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Rules API

Create, list, get, update, delete, and execute Rules - the condition/action Automations that operate on SmartThings connected devices.

- **Human URL:** [https://developer.smartthings.com/docs/automations/rules](https://developer.smartthings.com/docs/automations/rules)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Capabilities API

List and retrieve standard and custom Capabilities - the typed attributes and commands (switch, temperatureMeasurement, lock, etc.) that describe what a device can do, by capability id and version.

- **Human URL:** [https://developer.smartthings.com/docs/devices/capabilities/capabilities-reference](https://developer.smartthings.com/docs/devices/capabilities/capabilities-reference)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Subscriptions API

Create, list, get, and delete an Installed App's event Subscriptions - filters that determine which device, capability, mode, or device-lifecycle events are delivered to the app's webhook via the EVENT lifecycle callback.

- **Human URL:** [https://developer.smartthings.com/docs/connected-services/subscriptions](https://developer.smartthings.com/docs/connected-services/subscriptions)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Schedules API

Create, list, and delete Schedules for an Installed App - once or cron-style future executions that trigger the app's EXECUTE lifecycle callback.

- **Human URL:** [https://developer.smartthings.com/docs/connected-services/schedules](https://developer.smartthings.com/docs/connected-services/schedules)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Apps API

Register and manage SmartApps - the AWS Lambda or webhook endpoints that implement the SmartThings lifecycle (PING, CONFIGURATION, INSTALL, UPDATE, EVENT, UNINSTALL) - including creating, listing, updating, deleting, and rotating OAuth settings.

- **Human URL:** [https://developer.smartthings.com/docs/connected-services/smartapp-basics](https://developer.smartthings.com/docs/connected-services/smartapp-basics)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Installed Apps API

List, get, and delete a user's Installed Apps and read their configurations, and create Installed App events - the per-user installations of a SmartApp within a Location.

- **Human URL:** [https://developer.smartthings.com/docs/connected-services/lifecycles](https://developer.smartthings.com/docs/connected-services/lifecycles)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Presentations API

Generate, create, and retrieve device Presentations and device configurations - the metadata that drives how a device is rendered and controlled in the SmartThings app.

- **Human URL:** [https://developer.smartthings.com/docs/devices/device-presentation](https://developer.smartthings.com/docs/devices/device-presentation)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings History API

Query the paginated event History for devices and locations - the time-ordered record of device state changes and events.

- **Human URL:** [https://developer.smartthings.com/docs/devices/device-history](https://developer.smartthings.com/docs/devices/device-history)
- **Base URL:** `https://api.smartthings.com/v1`

### SmartThings Virtual Devices API

Create and manage Virtual Devices and push events to them - software devices with prototype or standard profiles used for testing automations and integrations without physical hardware.

- **Human URL:** [https://developer.smartthings.com/docs/devices/virtual-devices](https://developer.smartthings.com/docs/devices/virtual-devices)
- **Base URL:** `https://api.smartthings.com/v1`

## Authentication

- **Personal Access Token (PAT):** generate at [account.smartthings.com/tokens](https://account.smartthings.com/tokens) with the scopes you need (for testing / personal use).
- **OAuth 2.0:** create an OAuth-In App via the SmartThings CLI, then use `https://api.smartthings.com/oauth/authorize` and exchange the code at `https://api.smartthings.com/oauth/token` (for production integrations).

All requests pass the token as `Authorization: Bearer {token}`.

## Eventing

SmartThings does not expose a documented public WebSocket API. Real-time events are delivered outbound over HTTP webhooks: a SmartApp creates Subscriptions and receives matching events via the EVENT lifecycle callback POSTed to its endpoint, and the Enterprise Eventing API lets service accounts register account-level webhook "sinks." See [review.yml](review.yml) for the full WebSocket assessment.

## Rate Limits

The API applies per-endpoint rate limits and platform guardrails per token / per app / per device. Responses carry `X-RateLimit-Limit`, `X-RateLimit-Remaining`, and `X-RateLimit-Reset` headers. Exceeding a rate limit returns HTTP 429; exceeding a guardrail returns HTTP 422. See [rate-limits/smartthings-rate-limits.yml](rate-limits/smartthings-rate-limits.yml).

## Common Properties

- [GitHub Organization](https://github.com/SmartThingsCommunity)
- [LinkedIn](https://www.linkedin.com/showcase/smartthings)
- [Website](https://www.smartthings.com)
- [Documentation](https://developer.smartthings.com/docs)
- [Plans](plans/smartthings-plans-pricing.yml)
- [Rate Limits](rate-limits/smartthings-rate-limits.yml)
- [Fin Ops](finops/smartthings-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
