# Samsung SmartThings (smartthings)

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
