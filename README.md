# bookmarkd

Small bookmark service with search and tags

## Install

```bash
npm install
npm run dev
```

## Features

- REST endpoints: list / create / delete / search
- Morgan logging and centralized error handler
- In-memory store with optional JSON persistence
- Request validation helpers, no framework magic
- env-driven port, runs anywhere Node does

## Usage

```bash
curl -X POST localhost:3000/api/bookmarks \
  -H 'content-type: application/json' \
  -d '{"url": "https://example.com", "tags": ["reading"]}'
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── faq.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   ├── config.js
│   ├── index.js
│   └── store.js
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
└── package.json
```

## License

MIT - see [LICENSE](LICENSE).
