# Tokyo Institute of Technology (tokyo-institute-of-technology)

Tokyo Institute of Technology (Tokyo Tech / Titech) was a national research university in Tokyo, Japan, ranked **#76 in the QS World University Rankings 2025**. In October 2024 it merged with Tokyo Medical and Dental University to form the **Institute of Science Tokyo (Science Tokyo)**, with its public web presence now at [isct.ac.jp](https://www.isct.ac.jp/en) while legacy `titech.ac.jp` services remain online. This repository catalogs the institution's public, machine-readable developer/API footprint as an APIs.json profile.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/tokyo-institute-of-technology/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=tokyo-institute-of-technology-api-evangelist&utm_content=repo

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Japan, Research, Open Access, Institutional Repository, OAI-PMH

## APIs

- **T2R2 Research Repository OAI-PMH** — OAI-PMH 2.0 metadata harvesting interface for the Science Tokyo / Tokyo Tech Research Repository (papers, theses, manuscripts, patents); public, no signup. Docs: https://t2r2.star.titech.ac.jp/index_en.html — Base: `https://t2r2.star.titech.ac.jp/oaipmh/OAIHandler`
- **GakuNin Shibboleth Identity Provider (SAML)** — Federated SAML 2.0 / Shibboleth institutional single sign-on via Japan's GakuNin federation; an authentication endpoint, not a public OAuth/OpenID Connect developer API. Docs: https://www.gsic.titech.ac.jp/en

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/tokyo-institute-of-technology-plans-pricing.yml](plans/tokyo-institute-of-technology-plans-pricing.yml)
- Rate Limits: [rate-limits/tokyo-institute-of-technology-rate-limits.yml](rate-limits/tokyo-institute-of-technology-rate-limits.yml)
- FinOps: [finops/tokyo-institute-of-technology-finops.yml](finops/tokyo-institute-of-technology-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.isct.ac.jp/en
- GitHub (research group, no official institutional org): https://github.com/prg-titech
- LinkedIn: https://www.linkedin.com/school/sciencetokyo/
- Twitter/X: https://twitter.com/sciencetokyo_en
- Authentication (GakuNin Shibboleth IdP): https://idp-gakunin.nap.gsic.titech.ac.jp/idp/shibboleth
- Review: [review.yml](review.yml)

## Notes

- Verification caveats: the T2R2 OAI-PMH endpoint was confirmed live (HTTP 200, valid OAI-PMH 2.0 `Identify` response). The GSIC pages return 403 to bot user agents but are browser-accessible. The LinkedIn school page returns 999 (LinkedIn bot block) yet resolves in a browser. The Shibboleth IdP is a SAML metadata entity, not a REST API.
- No official institution-wide REST developer portal or open-data API was found. There is no official Science Tokyo institutional GitHub organization; only lab/research-group orgs exist (e.g., `prg-titech`). No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
