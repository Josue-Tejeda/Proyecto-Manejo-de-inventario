# Flask Mobile Inventory Manager

A production-ready inventory tracking and supply management platform designed for mobile device distributors. Built using **Flask** and structured with clean separation of concerns using Flask extensions.

## 🚀 Key Features

*   **Secure Session Authentication**: Fully-featured login, sign-up, and session persistence systems powered by `Flask-Login`.
*   **SQLAlchemy ORM Database**: Structured relational database models using `Flask-SQLAlchemy` with cascade deletes and foreign key mapping.
*   **Data Validation & CSRF Protection**: Form inputs securely verified on both client and server side via `Flask-WTF` and `WTForms`.
*   **Gunicorn Configurations**: Pre-configured `Procfile` and Gunicorn arguments for immediate deployment to PaaS clouds like Render or Heroku.
*   **Clean Settings Control**: Separated secret keys and settings variables utilizing `python-decouple`.

---

## 🛠 Tech Stack

- **Backend Framework**: Python, Flask 2.x
- **ORM / Database**: SQLAlchemy, SQLite (with support for PostgreSQL in production)
- **Forms & Validation**: WTForms, Flask-WTF (with CSRF protection)
- **Session Manager**: Flask-Login
- **Frontend**: Bootstrap 5, Jinja2 template engine

---

## ⚙️ Running Locally

### Prerequisites
- Python 3.8+

### 1. Clone & Set Up Directory
```bash
git clone https://github.com/Josue-Tejeda/Proyecto-Manejo-de-inventario.git
cd Proyecto-Manejo-de-inventario
```

### 2. Configure Virtual Environment
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

### 3. Install Required Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables
Create a `.env` file in the root folder:
```env
SECRET_KEY=your-flask-secret-key
DATABASE_URL=sqlite:///database/inventory.db
DEBUG=True
```

### 5. Launch the Server
```bash
flask run
```
Open `http://127.0.0.1:5000` to interact with the inventory dashboard.
