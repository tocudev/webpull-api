# <img src="card_index_3d.png" width="40" /> webpull-api
``webpull-api`` Is a completely free web API that works instantly! The backend of the API is written in ``python`` Any HTTP client is supported. I hope you enjoy this API and you can read the DOCS below.

## Example usage

```bash
curl "https://api.tocu.click/search?q=hello"
```
```bash
curl -sL -G "https://api.tocu.click/search" --data-urlencode "q=is gta6 coming out soon?"
```

```
{
  "results": [
    {
      "title": "Hello - Wikipedia",
      "url": "https://en.wikipedia.org/wiki/Hello",
      "snippet": "Hello is a salutation or greeting in the English language..."
    }
  ]
}
```
## Parameters
| param | type | required | default | max | description |
|-------|------|----------|---------|-----|-------------|
| q | string | yes | — | — | the search query |
| c | int | no | 200 | 500 | max characters per snippet |

## Terms of service 
By using this API, you agree to the [Terms of Service](TERMS.md). 
This is a free service with rate limits and a security filter. See `/terms` for details.
