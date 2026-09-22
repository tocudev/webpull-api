# webpull-api

completely free web search api. no limits, keys, or sign up.

![free](https://img.shields.io/badge/free-yes-brightgreen)
![api key](https://img.shields.io/badge/api_key-not_required-blue)
![signup](https://img.shields.io/badge/signup-not_required-blue)
![limits](https://img.shields.io/badge/limits-none-brightgreen)

## usage

curl "https://api.webpull.tocu.click/search?q=hello"

returns json:

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
| param | type | required | default | max | description |
|-------|------|----------|---------|-----|-------------|
| q | string | yes | — | — | the search query |
| c | int | no | 200 | 500 | max characters per snippet |
