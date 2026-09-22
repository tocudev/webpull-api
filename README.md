![Free](https://img.shields.io/badge/free-yes-brightgreen) ![No API Key](https://img.shields.io/badge/api_key-not_required-blue) ![No Signup](https://img.shields.io/badge/signup-not_required-blue) ![No Limits](https://img.shields.io/badge/limits-none-brightgreen)
```
user
  |
  v
nginx      tls, rate limit
  |
  v
fastapi    /search
  |
  v
searxng    meta search
  |
  v
web
```
```
webgo-api/
├── .github/
│   └── profile/
│       └── README.md
├── docs/
│   ├── architecture.md
│   └── api.md
├── cli/
│   ├── pyproject.toml
│   └── webgo/
│       ├── __init__.py
│       ├── __main__.py
│       ├── cli.py
│       ├── client.py
│       └── config.py
├── server/          (private)
├── LICENSE
├── NOTICE
└── README.md
```
