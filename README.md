<p align="center">
  <img src="5049.png" width="300" />
  <br />
  <img src="https://img.shields.io/badge/SearXNG-3050FF?logo=searxng&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" />
<a href="https://github.com/sponsors/tocudev">
  <img src="https://custom-icon-badges.demolab.com/badge/Sponsor-ea4aaa?style=flat&logo=heart&logoColor=white" />
</a>
</p>

`webpull-api` is a completely free web API that works instantly. The backend is written in `python`, and any HTTP client is supported. I hope you enjoy this API — you can read the docs below.

webpull is a free search API that returns fancy and clean ``JSON``, no API key, no signup.
<p align="center">
  <img src="5074.png" width="300" />
</p>

> [!IMPORTANT]
> This is NOT a paid service, please open a issue if you are reporting abuse!

```bash
curl "https://api.tocu.click/search?q=hello"
```

```json
[
  {
    "title": "Hello - Wikipedia",
    "url": "https://en.wikipedia.org/wiki/Hello",
    "snippet": "Hello is a salutation or greeting in the English language...",
    "date": "2026-09-18"
  }
]
```

<p align="center">
  <img src="5078.png" width="300" />
</p>

### `GET /`

API index. Lists all available endpoints.

```bash
curl "https://api.tocu.click/"
```

```json
{
  "name": "WebPull",
  "status": "ok",
  "endpoints": [
    {
      "method": "GET",
      "path": "/search?q=<query>&category=<category>",
      "description": "Search the web and return JSON results."
    },
    {
      "method": "GET",
      "path": "/health",
      "description": "Health check."
    },
    {
      "method": "GET",
      "path": "/",
      "description": "This API index."
    }
  ]
}
```

### `GET /search`

Search the web and return structured JSON results.

| param | type | required | default | description |
|-------|------|----------|---------|-------------|
| `q` | string | yes | — | The search query. Max 500 characters. |
| `category` | string | no | `general` | Filter by category. Allowed: `general`, `news`, `images`, `videos`, `music`, `it`, `science`. |
| `c` | int | no | `200` | Max characters per snippet. Min 1, max 500. |

**Example request:**

```bash
curl "https://api.tocu.click/search?q=hello"
```

**Example with all params:**

```bash
curl -G "https://api.tocu.click/search" \
  --data-urlencode "q=is gta6 coming out soon?" \
  --data-urlencode "category=news" \
  --data-urlencode "c=300"
```

**Example response:**

```json
[
  {
    "title": "Grand Theft Auto VI is Now Set to Launch November 19, 2026",
    "url": "https://www.rockstargames.com/newswire/article/ak3ak31a49a221/",
    "snippet": "Hi everyone, Grand Theft Auto VI will now release on Thursday, November 19, 2026...",
    "date": "2026-09-18"
  }
]
```

<p align="center">
  <img src="5074.png" width="300" />
</p>

> [!NOTE]
> hi gay

> [!TIP]
> HI

<details>
<summary>Click to see the full API reference</summary>

Here's the hidden content. It can include **markdown** and code blocks.

</details>

- [x] Search endpoint
- [x] Rate limiting
- [ ] Economy module