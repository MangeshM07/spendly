# Spendly — Personal Expense Tracker

A Flask + SQLite web app for logging and understanding personal expenses.

## Features

- User registration and login
- Add, edit, and delete expenses with category, amount, date, and description
- Category breakdowns and monthly spending summaries
- Filter expenses by custom date ranges

## Tech Stack

- **Backend:** Python / Flask
- **Database:** SQLite (via `database/db.py`)
- **Frontend:** Jinja2 templates, plain CSS + JS

## Setup

```bash
# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the development server
python app.py
```

The app runs at `http://localhost:5001`.

## Project Structure

```
expense-tracker/
├── app.py              # Flask routes
├── requirements.txt
├── database/
│   ├── db.py           # SQLite helpers: get_db, init_db, seed_db
│   └── __init__.py
├── templates/          # Jinja2 HTML templates
│   ├── base.html
│   ├── landing.html
│   ├── login.html
│   └── register.html
└── static/             # CSS and JS assets
```

## Implementation Steps

1. Database setup (`get_db`, `init_db`, `seed_db`)
2. User registration
3. User login / logout
4. Profile page
5–6. Expense listing and filtering
7. Add expense
8. Edit expense
9. Delete expense

## Running Tests

```bash
pytest
```
