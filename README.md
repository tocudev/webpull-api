![card_index_3d](card_index_3d.png)
# webpull-api
completely free web search api. no limits, keys, or sign up.

## Example usage

```bash
curl "https://api.webpull.tocu.click/search?q=hello"
```
```json
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
## parameters
| param | type | required | default | max | description |
|-------|------|----------|---------|-----|-------------|
| q | string | yes | — | — | the search query |
| c | int | no | 200 | 500 | max characters per snippet |
