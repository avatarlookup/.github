## AvatarLookup

**Public avatar lookups and portrait attribute analysis.**

Check whether an account publishes a usable public avatar — by phone number or email address — and read the portrait attributes of that image. An image can also be analysed directly. Whole lists, across seven platforms, go through the bulk task API.

[**Website**](https://avatarlookup.com) · [**API documentation**](https://avatarlookup.com/api-docs) · [**Pricing**](https://avatarlookup.com/pricing) · [**Get an API key**](https://avatarlookup.com/register)

### Official API example repositories

One repository per product, each mirroring its own product page.

| Repository | Shape | Product code | Contents |
|---|---|---|---|
| **[WhatsApp avatar analysis](https://github.com/avatarlookup/whatsapp-avatar-profile-api)** | Realtime | `ws_avatar` | OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Email avatar analysis](https://github.com/avatarlookup/email-avatar-profile-api)** | Realtime | `email_avatar` | OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Image profile analysis](https://github.com/avatarlookup/image-profile-analysis-api)** | Realtime | `image_profile` | OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Email Bulk Avatar Check](https://github.com/avatarlookup/email-bulk-avatar-api)** | Bulk (async) | `email_avatar_batch` | Input: email · OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[LINE Bulk Avatar Analysis](https://github.com/avatarlookup/line-bulk-profile-api)** | Bulk (async) | `line_profile_batch` | Input: phone · OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[MAX Bulk Number Profile](https://github.com/avatarlookup/max-bulk-profile-api)** | Bulk (async) | `max_profile_batch` | Input: phone · OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Telegram Bulk Number Profile](https://github.com/avatarlookup/telegram-bulk-number-profile-api)** | Bulk (async) | `tg_profile_batch` | Input: phone · OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Telegram Bulk Username Profile](https://github.com/avatarlookup/telegram-bulk-username-profile-api)** | Bulk (async) | `tg_username_profile_batch` | Input: username · OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Viber Bulk Number Profile](https://github.com/avatarlookup/viber-bulk-profile-api)** | Bulk (async) | `viber_profile_batch` | Input: phone · OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[WhatsApp Bulk Avatar Analysis](https://github.com/avatarlookup/whatsapp-bulk-avatar-api)** | Bulk (async) | `ws_profile_batch` | Input: phone · OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Zalo Bulk Number Profile](https://github.com/avatarlookup/zalo-bulk-profile-api)** | Bulk (async) | `zalo_profile_batch` | Input: phone · OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| [avatarlookup-resources](https://github.com/avatarlookup/avatarlookup-resources) | — | — | Technical notes, guides and announcements |

Every example repository carries a machine-readable `product.json`, an `llms.txt` summary for AI clients, an OpenAPI 3.0 contract, and runnable examples in Python, Node.js, Go, Java, C#, PHP and Shell. All request paths, response fields and limits are taken from the live product pages and the published API documentation.

### Realtime or bulk?

A **realtime** check (`POST /api/v1/check`, or `POST /api/v1/batch-check` for up to 100 identifiers) answers inside the same HTTP response — that is the shape for a signup form, a checkout step or a live lookup. A **bulk task** (`POST /api/v1/bulk-tasks`) takes a `.txt`/`.csv` file of 1,000–100,000 entries, returns a task id immediately, and produces a downloadable result file — that is the shape for list cleaning, campaign preparation and enrichment runs. The two are separate endpoints and are not interchangeable.

One bulk task carries **one product**. Phone-number tasks also carry exactly one `country`; email and username tasks have no country at all.

### One key, one balance

Every product on AvatarLookup uses the same API key, the same `X-API-Key` header and the same `code` / `msg` / `data` envelope, and draws from the same account balance.

### Responsible use

Results are **point-in-time signals**: they describe what a provider reported at the moment of the check. They are not identity verification, not proof of ownership, and not permission to contact anyone. Use the API only for identifiers you are authorized to process, and comply with applicable privacy laws and platform terms. Third-party trademarks belong to their respective owners; no affiliation or endorsement is implied.
