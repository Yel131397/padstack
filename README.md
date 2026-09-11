# padstack

Minimal notes REST API built with Flask

Built for my own use; public in case it helps someone.

## Highlights

- SQLite storage via sqlite3 stdlib
- CRUD endpoints for notes
- Request validation and consistent error shape
- pytest coverage for the happy paths

## Examples

```bash
curl -X POST localhost:5000/notes \
  -H 'content-type: application/json' \
  -d '{"title": "first", "body": "hello"}'
```

## Getting started

```bash
pip install -r requirements.txt
flask --app app run --debug
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_api.py
├── .gitignore
├── CONTRIBUTING.md
├── app.py
└── requirements.txt
```

## FAQ

**Is this production ready?**  
It works for my use case; review the code before relying on it.

**Why no framework?**  
The stdlib covers what this project needs.
