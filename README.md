![card_index_3d](card_index_3d.png)

completely free web search api. no limits, keys, or sign up.

![free](https://img.shields.io/badge/free-yes-brightgreen)
![api key](https://img.shields.io/badge/api_key-not_required-blue)
![signup](https://img.shields.io/badge/signup-not_required-blue)
![limits](https://img.shields.io/badge/limits-none-brightgreen)

## Example usage

```bash
curl "https://api.webpull.tocu.click/search?q=hello"
```
Returns json

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
