# Jitsi

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

Jitsi is a collection of free and open-source projects for secure, simple, and scalable real-time video conferencing, maintained by 8x8. The Jitsi stack combines a browser-based meeting application (Jitsi Meet), a WebRTC selective forwarding unit (Jitsi Videobridge), conference focus (Jicofo), SIP gateway (Jigasi), and broadcasting infrastructure (Jibri), along with web, mobile, desktop, and low-level SDKs for embedding meetings into other applications. Jitsi is also available as a fully managed offering — Jitsi as a Service (JaaS) — that exposes the same conferencing surface through a JWT-secured API and the Jitsi IFrame/External API.

**Areas:** Video Conferencing · WebRTC · Real-Time Communication · Open Source · Voice · Video · SIP · Streaming · Recording · Self-Hosted

## Jitsi on APIs.io

Everything profiled for Jitsi is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/jitsi-org/](https://apis.io/providers/jitsi-org/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [Jitsi Meet IFrame (External) API](https://apis.io/apis/jitsi-org/jitsi-meet-iframe-api/) — Browser-side JavaScript API (also called the External API) that embeds a Jitsi Meet conference into any web page through an iframe. Exposes the…
- [lib-jitsi-meet (Low-Level JavaScript API)](https://apis.io/apis/jitsi-org/lib-jitsi-meet-api/) — Low-level JavaScript library for building entirely custom video conferencing experiences on top of the Jitsi infrastructure. Exposes JitsiConnection,…
- [Jitsi Videobridge REST API](https://apis.io/apis/jitsi-org/jitsi-videobridge-rest-api/) — Administrative HTTP API exposed by Jitsi Videobridge for operators to read bridge state, list active conferences, inspect endpoints, gracefully drain a…
- [Jicofo REST API](https://apis.io/apis/jitsi-org/jicofo-rest-api/) — Operations REST API exposed by Jicofo (Jitsi Conference Focus) for inspecting in-progress conferences, listing the bridge selection state, and triggering…
- [Jibri REST API](https://apis.io/apis/jitsi-org/jibri-rest-api/) — HTTP control API exposed by Jibri (Jitsi BRoadcasting Infrastructure) for starting and stopping recording or live-streaming sessions, reporting health, and…
- [JaaS (Jitsi as a Service) REST API](https://apis.io/apis/jitsi-org/jaas-rest-api/) — Managed Jitsi as a Service offering from 8x8 that fronts the open-source Jitsi stack with a JWT-secured REST surface for issuing meeting tokens, managing…
- [JaaS IFrame API](https://apis.io/apis/jitsi-org/jaas-iframe-api/) — JaaS-flavoured IFrame API that loads external_api.js from 8x8-vc.com (the managed Jitsi domain) and authenticates each meeting with a signed JWT issued for…
- [Jitsi Meet Mobile SDK (Android, iOS, React Native)](https://apis.io/apis/jitsi-org/jitsi-meet-mobile-sdk/) — Native mobile SDKs that embed the full Jitsi Meet experience inside Android and iOS applications, plus a React Native module published from the jitsi-meet…
- [Jitsi Meet Electron SDK](https://apis.io/apis/jitsi-org/jitsi-meet-electron-sdk/) — Electron toolkit for embedding Jitsi Meet inside a desktop application, including remote control, always-on-top thumbnails, screen sharing, and native…
- [Jitsi Meet React SDK](https://apis.io/apis/jitsi-org/jitsi-meet-react-sdk/) — React component wrapper around the Jitsi Meet IFrame API that provides idiomatic <JitsiMeeting /> and <JaaSMeeting /> components, type definitions, hooks…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Jitsi Org Domain Security](https://apis.io/security/jitsi-org/jitsi-org-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://jitsi.org)
- [Documentation](https://jitsi.github.io/handbook/)
- [Getting started](https://jitsi.github.io/handbook/docs/intro)
- [Pricing](https://jaas.8x8.vc/#/pricing)
- [Support](https://community.jitsi.org/)
- [Blog](https://jitsi.org/blog/)
- [Terms of service](https://8x8.com/terms-conditions)
- [Privacy policy](https://www.8x8.com/terms-and-conditions/privacy-policy)
- [GitHub](https://github.com/jitsi)

## API Evangelist rating

**Kin Score 33.3** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 6.5 |
| Contract governance | 0.0 |
| Operational transparency | 28.9 |
| Developer ergonomics | 73.8 |
| Access clarity | 34.2 |

**Agent readiness 3.8** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 15.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/jitsi-org/](https://apis.io/providers/jitsi-org/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Jitsi: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/jitsi-org/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
