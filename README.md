# TheNewsAPI

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

Global news aggregation REST API providing real-time and historical news articles from thousands of sources with filtering by category, language, country, and search. Indexes over 1 million new articles per week from 40,000+ sources across 50+ countries and 35+ languages.

## Base URL

```
https://api.thenewsapi.com/v1
```

## Authentication

All requests require an API token passed as a query parameter:

```
?api_token=YOUR_API_TOKEN
```

Register for free at https://www.thenewsapi.com/register to obtain a token.

## Endpoints

| Endpoint | Method | Path | Plans |
|----------|--------|------|-------|
| All News | GET | /news/all | All |
| Top Stories | GET | /news/top | All |
| Headlines | GET | /news/headlines | Standard+ |
| Similar News | GET | /news/similar/{uuid} | All |
| News by UUID | GET | /news/uuid/{uuid} | All |
| Sources | GET | /news/sources | All |

## Pricing

| Plan | Monthly | Annual | Daily Requests | Articles/Request |
|------|---------|--------|----------------|-----------------|
| Free | $0 | $0 | 100 | 3 |
| Basic | $19 | $16 | 2,500 | 25 |
| Standard | $49 | $41 | 10,000 | 100 |
| Pro | $79 | $66 | 25,000 | 200 |
| Enterprise | Custom | Custom | Custom | Custom |

## Rate Limits

- Daily request quotas enforced per plan
- Burst throttling within any 60-second window (HTTP 429)
- Maximum 20,000 articles retrievable per query via pagination
- Sources endpoint: 50 results per request maximum

## Supported Filters

- **Categories:** general, science, sports, business, health, entertainment, tech, politics, food, travel
- **Countries:** 50+ locales including US, UK, Canada, Australia, India, Japan, Mexico, Brazil
- **Languages:** 35+ including English, Spanish, French, German, Chinese, Japanese, Arabic

## Resources

- [Documentation](https://www.thenewsapi.com/documentation)
- [Pricing](https://www.thenewsapi.com/pricing)
- [Register](https://www.thenewsapi.com/register)
- [Contact](https://www.thenewsapi.com/contact)

---

This repository contains an [APIs.json 0.19](https://apisjson.org) profile for TheNewsAPI maintained by [API Evangelist](https://apievangelist.com).
