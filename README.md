# Blue Cross Canada (canadian-blue-cross)

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
