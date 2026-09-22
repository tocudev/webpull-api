![Free](https://img.shields.io/badge/free-yes-brightgreen)
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
