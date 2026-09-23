# <img src="card_index_3d.png" width="40" /> webpull-api
``webpull-api`` Is a completely free web API you can use instantly! The backend of the API is written in ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) I hope you enjoy this API and you can read the DOCS below.

## Example usage

```bash
curl "https://api.tocu.click/search?q=hello"
```
```bash
curl -G "http://api.tocu.clickc/search" --data-urlencode "q=what is honeypot?"
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
