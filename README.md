# TheNewsAPI

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
