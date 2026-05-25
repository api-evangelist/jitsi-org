# Jitsi (jitsi)

Jitsi is a collection of free and open-source projects for secure, simple, and scalable real-time video conferencing, maintained by 8x8. The Jitsi stack combines a browser-based meeting application (Jitsi Meet), a WebRTC selective forwarding unit (Jitsi Videobridge), conference focus (Jicofo), SIP gateway (Jigasi), and broadcasting infrastructure (Jibri), along with web, mobile, desktop, and low-level SDKs for embedding meetings into other applications. Jitsi is also available as a fully managed offering — Jitsi as a Service (JaaS) — that exposes the same conferencing surface through a JWT-secured API and the Jitsi IFrame/External API.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/jitsi-org/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=opensource-api-evangelist&utm_content=repo)

## Tags

Video Conferencing, WebRTC, Real-Time Communication, Open Source, Voice, Video, SIP, Streaming, Recording, Self-Hosted

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Core Projects

| Project | Repo | What it is |
|---|---|---|
| Jitsi Meet | [jitsi/jitsi-meet](https://github.com/jitsi/jitsi-meet) | TypeScript meeting client (web + mobile + desktop bridge) |
| Jitsi Videobridge | [jitsi/jitsi-videobridge](https://github.com/jitsi/jitsi-videobridge) | WebRTC SFU written in Kotlin |
| lib-jitsi-meet | [jitsi/lib-jitsi-meet](https://github.com/jitsi/lib-jitsi-meet) | Low-level JS API for custom UIs |
| Jicofo | [jitsi/jicofo](https://github.com/jitsi/jicofo) | Conference focus / signaling controller |
| Jigasi | [jitsi/jigasi](https://github.com/jitsi/jigasi) | SIP gateway + transcription |
| Jibri | [jitsi/jibri](https://github.com/jitsi/jibri) | Recording + RTMP live streaming |
| docker-jitsi-meet | [jitsi/docker-jitsi-meet](https://github.com/jitsi/docker-jitsi-meet) | Full stack on Docker Compose |
| Jitsi Meet Electron | [jitsi/jitsi-meet-electron](https://github.com/jitsi/jitsi-meet-electron) | Desktop app |
| Handbook | [jitsi/handbook](https://github.com/jitsi/handbook) | Official developer + operator docs |
| Skynet | [jitsi/skynet](https://github.com/jitsi/skynet) | AI core services for Jitsi |

## APIs

### Jitsi Meet IFrame (External) API
Browser-side JavaScript API that embeds a Jitsi Meet conference into any web page through an iframe. Exposes the `JitsiMeetExternalAPI` constructor with commands, functions, and a rich event surface (`videoConferenceJoined`, `participantJoined`, `audioMuteStatusChanged`, breakout rooms, raise hand). Powers meet.jit.si, self-hosted deployments, and JaaS.

**Human URL:** [https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-iframe](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-iframe)

- [Documentation](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-iframe)
- [IFrame API Functions](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-iframe-functions)
- [IFrame API Events](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-iframe-events)
- [IFrame API Commands](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-iframe-commands)
- [Source — external_api.js](https://github.com/jitsi/jitsi-meet/blob/master/modules/API/external/external_api.js)

### lib-jitsi-meet (Low-Level JavaScript API)
Low-level JavaScript library for building entirely custom video conferencing experiences on top of Jitsi infrastructure. Exposes `JitsiConnection`, `JitsiConference`, `JitsiTrack`, and the XMPP/Colibri signaling primitives that Jitsi Meet itself uses.

**Human URL:** [https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-ljm-api](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-ljm-api)

- [Documentation](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-ljm-api)
- [Source — lib-jitsi-meet](https://github.com/jitsi/lib-jitsi-meet)
- [npm — lib-jitsi-meet](https://www.npmjs.com/package/lib-jitsi-meet)

### Jitsi Videobridge REST API
Administrative HTTP API exposed by Jitsi Videobridge for operators to read bridge state, list active conferences, inspect endpoints, gracefully drain a bridge, and scrape Prometheus metrics. Typically bound to the private network on port 8080.

**Base URL:** `http://localhost:8080`

- [Documentation — Videobridge REST](https://github.com/jitsi/jitsi-videobridge/blob/master/doc/rest.md)
- [Documentation — Statistics](https://github.com/jitsi/jitsi-videobridge/blob/master/doc/statistics.md)
- [Source — jitsi-videobridge](https://github.com/jitsi/jitsi-videobridge)

### Jicofo REST API
Operations REST API exposed by Jicofo (Jitsi Conference Focus) for inspecting in-progress conferences, listing bridge selection state, and triggering graceful shutdowns. Used by operators and orchestrators when running self-hosted Jitsi at scale.

**Base URL:** `http://localhost:8888`

- [Source — jicofo](https://github.com/jitsi/jicofo)

### Jibri REST API
HTTP control API exposed by Jibri (Jitsi BRoadcasting Infrastructure) for starting and stopping recording or live-streaming sessions, reporting health, and surfacing busy/idle state. Used by Jicofo and orchestrators when fanning recording or RTMP load across a Jibri pool.

**Base URL:** `http://localhost:2222`

- [Documentation — Jibri HTTP API](https://github.com/jitsi/jibri/blob/master/doc/http_api.md)
- [Source — jibri](https://github.com/jitsi/jibri)

### JaaS (Jitsi as a Service) REST API
Managed Jitsi as a Service offering from 8x8 that fronts the open-source Jitsi stack with a JWT-secured REST surface for issuing meeting tokens, managing rooms, fetching recordings, controlling participants, and retrieving usage. JaaS uses RS256 JSON Web Tokens signed with a tenant-specific API key/private key pair.

**Base URL:** `https://api.jaas.8x8.vc`

- [JaaS Developer Portal](https://developer.8x8.com/jaas/docs)
- [Getting Started](https://developer.8x8.com/jaas/docs/jaas-getting-started)
- [API Keys & Private Keys](https://developer.8x8.com/jaas/docs/api-keys-private-key)
- [JWT Overview](https://developer.8x8.com/jaas/docs/jwt-overview)
- [JaaS Console](https://jaas.8x8.vc/)

### JaaS IFrame API
JaaS-flavoured IFrame API that loads `external_api.js` from the managed 8x8-vc.com domain and authenticates each meeting with a signed JWT issued for the tenant. Same `JitsiMeetExternalAPI` surface as the open-source IFrame API plus JaaS-specific moderator/participant claims and branding controls.

- [Documentation — JaaS IFrame API](https://developer.8x8.com/jaas/docs/iframe-api-jaas)
- [Authentication — JWT Overview](https://developer.8x8.com/jaas/docs/jwt-overview)

### Jitsi Meet Mobile SDK (Android, iOS, React Native)
Native mobile SDKs that embed the full Jitsi Meet experience inside Android and iOS applications, plus a React Native module published from the jitsi-meet repository. Each SDK exposes a meeting view, a small JS bridge for events and commands, and supports JWT authentication.

- [Android SDK](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-android-sdk)
- [iOS SDK](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-ios-sdk)
- [React Native SDK](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-react-native-sdk)
- [Mobile SDK Samples](https://github.com/jitsi/jitsi-meet-sdk-samples)

### Jitsi Meet Electron SDK
Electron toolkit for embedding Jitsi Meet inside a desktop application, including remote control, always-on-top thumbnails, screen sharing, and native window integration. Powers the official Jitsi Meet desktop app.

- [Documentation](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-electron-sdk)
- [Source — jitsi-meet-electron-sdk](https://github.com/jitsi/jitsi-meet-electron-sdk)
- [Source — jitsi-meet-electron app](https://github.com/jitsi/jitsi-meet-electron)

### Jitsi Meet React SDK
React component wrapper around the Jitsi Meet IFrame API providing idiomatic `<JitsiMeeting />` and `<JaaSMeeting />` components, type definitions, hooks for events, and ref-based command dispatch.

- [Documentation](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-react-sdk)
- [Source — jitsi-meet-react-sdk](https://github.com/jitsi/jitsi-meet-react-sdk)
- [npm — @jitsi/react-sdk](https://www.npmjs.com/package/@jitsi/react-sdk)

## Common

- [Portal](https://jitsi.org)
- [Website](https://jitsi.org)
- [Sandbox — meet.jit.si](https://meet.jit.si)
- [Documentation — Jitsi Handbook](https://jitsi.github.io/handbook/)
- [Getting Started](https://jitsi.github.io/handbook/docs/intro)
- [Projects Overview](https://jitsi.org/projects/)
- [JaaS Developer Portal](https://developer.8x8.com/jaas/docs)
- [Sign Up — JaaS Console](https://jaas.8x8.vc/)
- [Pricing — JaaS](https://jaas.8x8.vc/#/pricing)
- [GitHub Organization](https://github.com/jitsi)
- [Community / Support](https://community.jitsi.org/)
- [Blog](https://jitsi.org/blog/)
- [Release Notes](https://github.com/jitsi/jitsi-meet-release-notes)
- [License — Apache 2.0](https://github.com/jitsi/jitsi-meet/blob/master/LICENSE)
- [Authentication — JaaS JWT](https://developer.8x8.com/jaas/docs/jwt-overview)
- [Company — 8x8, Inc.](https://www.8x8.com)

## Maintainers

- **Kin Lane** — info@apievangelist.com — [apievangelist.com](https://apievangelist.com)
