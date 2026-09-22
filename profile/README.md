## AvatarLookup

**Public avatar lookups and portrait attribute analysis.**

Check whether an account publishes a usable public avatar — by phone number or email address — and read the portrait attributes of that image. An image can also be analysed directly.

[**Website**](https://avatarlookup.com) · [**API documentation**](https://avatarlookup.com/api-docs) · [**Pricing**](https://avatarlookup.com/pricing) · [**Get an API key**](https://avatarlookup.com/register)

### Official API example repositories

| Repository | Product code | Contents |
|---|---|---|
| **[WhatsApp avatar analysis](https://github.com/avatarlookup/whatsapp-avatar-profile-api)** | `ws_avatar` | OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Email avatar analysis](https://github.com/avatarlookup/email-avatar-profile-api)** | `email_avatar` | OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| **[Image profile analysis](https://github.com/avatarlookup/image-profile-analysis-api)** | `image_profile` | OpenAPI contract, `product.json`, `llms.txt`, examples in 7 languages |
| [avatarlookup-resources](https://github.com/avatarlookup/avatarlookup-resources) | — | Technical notes, guides and announcements |

Every example repository carries a machine-readable `product.json`, an `llms.txt` summary for AI clients, an OpenAPI 3.0 contract, and runnable examples in Python, Node.js, Go, Java, C#, PHP and Shell. All request paths, response fields and limits are taken from the live product pages and the published API documentation.

### One key, one balance

Every product on AvatarLookup uses the same API key, the same `X-API-Key` header and the same `code` / `msg` / `data` envelope, and draws from the same account balance.

### Responsible use

Results are **point-in-time signals**: they describe what a provider reported at the moment of the check. They are not identity verification, not proof of ownership, and not permission to contact anyone. Use the API only for identifiers you are authorized to process, and comply with applicable privacy laws and platform terms. Third-party trademarks belong to their respective owners; no affiliation or endorsement is implied.
