# <img src="card_index_3d.png" width="40" /> webpull-api
``webpull-api`` Is a completely free web API you can use instantly! The backend of the API is written in ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) I hope you enjoy this API and you can read the DOCS below.

## Example usage

```bash
curl "https://webpullapi.localhost.cc/search?q=hello"
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
