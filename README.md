# NTT Docomo (ntt-docomo)

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

NTT DOCOMO, Inc. is Japan's largest mobile network operator and a wholly owned subsidiary of Nippon Telegraph and Telephone (NTT), serving roughly 90 million mobile subscriptions in its home market of Japan across the docomo, ahamo and irumo brands, alongside the d ACCOUNT identity, d POINT loyalty, d Payment wallet and Lemino media franchises. In the telecom value chain DOCOMO is a facilities-based incumbent carrier — it owns the 5G radio, core and subscriber identity — but it does not sell that capability to developers directly. Its API posture is partner-gated and sales-led.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ntt-docomo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ntt-docomo/refs/heads/main/apis.yml)

## Tags

- Telecommunications
- Japan
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- Aduna
- Carrier Identity
- SIM Swap
- Number Verification
- Carrier Billing
- 5G
- Partner Gated

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## The Honest Developer Picture

There is no NTT DOCOMO developer portal. Every conventional developer host on `docomo.ne.jp` — `developer.`, `developers.`, `docs.`, `api.`, `opengateway.` — fails DNS resolution, and `/developer/`, `/developers/`, `/api/` and `/opengateway/` all return HTTP 404 on the main site.

The first-party programme that once existed is gone. **docomo Developer support** (`dev.smt.docomo.ne.jp`) opened in October 2013 as an API marketplace carrying DOCOMO and partner APIs — speech recognition, speech synthesis, chat dialogue, transit search, image recognition. It shut down on **31 March 2021**, and the DNS record has since been removed entirely, so even the archived documentation is off the live web. Third-party SDKs written against it now point at a host that does not resolve.

One public developer page survives — [www.docomo.ne.jp/service/developer/](https://www.docomo.ne.jp/service/developer/) (HTTP 200). It is open and requires no registration, but it documents handset and content technology (Machi-Chara, Deco-mail, emoji packages, NFC / Osaifu-Keitai, docomo Mail features, device spec lists, sp-mode server IP ranges), not an HTTP API. No keys, no sandbox, no REST reference, no machine-readable definition.

**No OpenAPI, Swagger or AsyncAPI definition is published anywhere on an NTT DOCOMO host.** This repository has no `openapi/` directory because there was nothing real to harvest.

## CAMARA Posture

**Press release, not implementation.**

In its own [30 January 2026 release](https://www.docomo.ne.jp/english/info/media_center/pr/2026/0130_00.html), DOCOMO states it "has participated in the GSMA Open Gateway initiative" and that it has collaborated with **Aduna** — the Ericsson-and-carrier joint venture — since June 2025, concluding a formal partnership agreement on 29 January 2026 to distribute its network APIs internationally. The release names two starting APIs:

- **Number Verification**
- **SIM Swap**

Nothing is callable. There is no CAMARA endpoint, no CAMARA OpenAPI hosted on a DOCOMO domain, no sandbox, no DOCOMO-branded Open Gateway portal and no credential path. And as of 2026-07-25, Aduna's own operator wall does not yet list NTT DOCOMO among its connected operators. A developer cannot call a DOCOMO network API today by any documented public route — not first-party, and not yet through the aggregator DOCOMO announced.

No TM Forum Open API conformance certification was confirmed for NTT DOCOMO, Inc. No public NEF/SCEF, network-slicing or edge/MEC API was found.

## Channel to Developers

NTT DOCOMO reaches developers only through intermediaries:

- **Network APIs** → Aduna (announced; not yet live on the aggregator).
- **Carrier billing (d払い)** → payment gateways such as GMO Payment Gateway, PAYGENT and SB Payment Service, who carry the integration specs DOCOMO does not publish.
- **Enterprise / wholesale** → `docomo.ne.jp/biz` redirects to `www.ntt.com`, the site of **NTT DOCOMO BUSINESS, Inc.** (the renamed NTT Communications), a separate legal entity on a separate domain, which runs the group's actual login-gated API gateway portal at `developer.ntt.com`. That entity is profiled separately in this network as `ntt-com` and is not counted here.

## APIs

### d ACCOUNT Connect

DOCOMO's carrier identity service for businesses — OpenID Connect social login backed by network line authentication and device biometrics, against roughly 90 million d ACCOUNT registrations and approximately 2,000 implemented sites.

- **Human URL:** [https://id.smt.docomo.ne.jp/src/index_business.html](https://id.smt.docomo.ne.jp/src/index_business.html)
- **Base URL:** `https://conf.uw.docomo.ne.jp/`

A live, anonymous OpenID Connect discovery document is served at [https://conf.uw.docomo.ne.jp/.well-known/openid-configuration](https://conf.uw.docomo.ne.jp/.well-known/openid-configuration) (HTTP 200, fetched 2026-07-25):

- issuer `https://conf.uw.docomo.ne.jp/`
- authorization endpoint `https://id.smt.docomo.ne.jp/cgi8/oidc/authorize`
- token endpoint `https://conf.uw.docomo.ne.jp/token`
- userinfo endpoint `https://conf.uw.docomo.ne.jp/userinfo`
- `response_types_supported: [code]`, `subject_types_supported: [pairwise]`, ID token signing HS256/RS256

**No `backchannel_authentication_endpoint` is advertised — CIBA, the grant CAMARA specifies for network-based authorization, does not appear.** The integration manual and support libraries download only after a use application and DOCOMO's review. No OpenAPI definition is published.

#### Properties

- [Documentation](https://id.smt.docomo.ne.jp/src/index_business.html)
- [API Reference](https://id.smt.docomo.ne.jp/src/dlogin/ctop_method.html)
- [OpenID Connect Discovery](https://conf.uw.docomo.ne.jp/.well-known/openid-configuration)

### docomo Mail IMAP Interface

The one machine-interface specification NTT DOCOMO publishes openly, without registration. It documents how a mail client connects to the docomo Mail service over IMAP, distributed as a 96-page Japanese PDF (`mail_imap_spec_260126.pdf`, HTTP 200, `application/pdf`, 1,229,737 bytes, revision dated 2026-01-26). This is an IMAP protocol interface, not an HTTP API — no REST surface, no OpenAPI, no key issuance, no sandbox.

- **Human URL:** [https://www.docomo.ne.jp/service/developer/smart_phone/application/imap/](https://www.docomo.ne.jp/service/developer/smart_phone/application/imap/)

#### Properties

- [Documentation](https://www.docomo.ne.jp/service/developer/smart_phone/application/imap/)
- [API Reference (PDF)](https://www.docomo.ne.jp/binary/pdf/service/developer/smart_phone/application/imap/mail_imap_spec_260126.pdf)

## Links

- [Website](https://www.docomo.ne.jp/)
- [Website (English)](https://www.docomo.ne.jp/english/)
- [Developer Information](https://www.docomo.ne.jp/service/developer/)
- [Developer Terms](https://www.docomo.ne.jp/service/developer/policy/index.html)
- [GitHub](https://github.com/docomo) — organisation exists, zero public repositories
- [LinkedIn](https://www.linkedin.com/company/ntt-docomo)
- [Press Releases (English)](https://www.docomo.ne.jp/english/info/media_center/pr/)
- [Press Releases (Japanese)](https://www.docomo.ne.jp/info/news_release/)
