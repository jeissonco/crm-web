# CRM Web (Flask + HTMX + Tailwind)

MVP to convert the CLI CRM into a modern web app using Flask (+ HTMX for snappy UX).

## Quickstart

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
export FLASK_APP=src/crm_web/app.py  # Windows PowerShell: $env:FLASK_APP="src/crm_web/app.py"
python src/crm_web/app.py    # or: flask --app src/crm_web/app.py run
```

Open http://127.0.0.1:5000/customers

## Run tests

```bash
pytest -q
```

## Project Layout

```
crm-web/
├─ src/crm_web/
│  ├─ app.py
│  ├─ models.py
│  ├─ routes/customers.py
│  ├─ templates/
│  │  ├─ base.html
│  │  └─ customers.html
│  └─ static/css/tailwind.css
├─ tests/test_customers.py
├─ requirements.txt
├─ README.md
└─ .github/workflows/python-ci.yml
```

## Next Steps (per roadmap)
- Week 2: swap in SQLite via SQLAlchemy, add proper validation & searching
- Week 3: export JSON/CSV + charts (Chart.js)
- Week 4: add login and deploy to Render/Railway
