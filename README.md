# Blue Cross Canada (canadian-blue-cross)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Blue Cross Canada (bluecross.ca) is the national consumer-facing brand of the Canadian Association of Blue Cross Plans, the association that owns the Blue Cross trademark in Canada and coordinates a federation of independent, largely not-for-profit regional Blue Cross plans — Alberta Blue Cross, Pacific Blue Cross, Manitoba Blue Cross, Saskatchewan Blue Cross, Ontario and Quebec Blue Cross (Canassurance), and Medavie Blue Cross. Operating in Canada since 1938, the federation covers roughly eight million Canadians a year across supplementary health and dental benefits, group and employee benefits, retiree plans, travel medical insurance, and term life and critical illness cover.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/canadian-blue-cross/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/canadian-blue-cross/refs/heads/main/apis.yml)

## Tags

- Insurance
- Canada
- Health Insurance
- Dental Benefits
- Travel Insurance
- Life Insurance
- Employee Benefits
- Group Benefits
- Claims
- Carrier
- Association
- No Public API

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

**None.** Blue Cross Canada publishes no public API.

This is the honest record, not a gap in the research. bluecross.ca is a WordPress marketing and region-routing site. There is no developer portal, no API reference, no SDK, no Postman collection, no GraphQL endpoint, no webhook or event catalog, and no OpenAPI, Swagger, or AsyncAPI document.

- The `developer`, `developers`, `docs`, and `api` subdomains of `bluecross.ca` do not resolve (NXDOMAIN).
- `/developers`, `/developer`, `/api`, `/integrations`, `/partners`, `/openapi.json`, `/swagger.json`, `/api-docs`, and `/graphql` all return **404**.
- The only machine-readable endpoint on the domain is the default WordPress REST route at `/wp-json/` (**200**, `application/json`) — an artifact of the publishing platform, not an insurance API, and deliberately not listed as one.
- The same probes were run against the operating member plans (`pac.bluecross.ca`, `on.bluecross.ca`, `sk.bluecross.ca`, `www.medaviebc.ca`): 404 on every developer path, with no `api.`/`developer.` subdomains resolving. `ab.bluecross.ca` returns **403** to non-browser clients.

Integration happens behind authentication — member portals and mobile apps, group-benefit employer portals, broker channels, and health-care provider e-claims rails.

### ACORD posture

**No ACORD reference found.** Zero occurrences of `ACORD`, `AL3`, `ACORD XML`, or `NGDS` across all 40 pages fetched from the site. ACORD is a property-and-casualty standards body; Blue Cross Canada is a health, dental, travel, group-benefits and life carrier federation, so its standards seam is health-claim adjudication rather than ACORD — and none of that is publicly documented either.

### Quote / bind / issue / FNOL

None exposed publicly. Quoting is HTML web flow, claims submission ("Make a Claim") lives inside authenticated member portals and mobile apps.

### Auth model

Human web session login only — member, plan-sponsor, and provider portals. No API keys, no OAuth2, no mTLS partner onboarding, and no OIDC discovery document (`/.well-known/openid-configuration` returns 404).

### Market context

Canada has no open-insurance mandate. OSFI supervises federally-regulated insurers prudentially while the provinces regulate market conduct (FSRA in Ontario, AMF in Quebec), and Consumer-Driven Banking — Canada's open-banking framework — excludes insurance entirely. A zero-API posture here is compliant behaviour, not a lag.

## Links

- [Website](https://www.bluecross.ca/)
- [About](https://www.bluecross.ca/about/)
- [News](https://www.bluecross.ca/news/)
- [Contact](https://www.bluecross.ca/contact/)
- [Members (login)](https://www.bluecross.ca/memberweb/)
- [Terms of Use & Privacy](https://www.bluecross.ca/terms-of-use-privacy/)

## Review

See [review.yml](review.yml) for the full probe log, HTTP statuses, ACORD evidence, and reviewer findings.
