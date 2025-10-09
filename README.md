# 📖 BytesStories

BytesStories is a **Flask-based blogging application** where users can **create posts, comment, and manage their accounts**.  
It follows a modular architecture using Blueprints and the App Factory pattern, with PostgreSQL as the database.  

---

## 🚀 Features
- 📝 **Post & Comment** – Users can write blog posts, upload content images, and leave comments.  
- 👤 **User Accounts** – Register, log in, update profiles with profile pictures.  
- 🔒 **Authentication** – Secure login system with password hashing (Flask-Bcrypt + Flask-Login).  
- 🧩 **Blueprints** – Separated modules for `users`, `posts`, `main`, and `errors`.  
- ⚡ **App Factory Pattern** – Uses `create_app()` for clean initialization.  
- 📑 **Pagination** – Posts and user profiles support pagination.  
- ❌ **Custom Error Handlers** – Friendly error pages (403, 404, 500, etc.).  
- 🖼️ **File Uploads** – Profile pictures and post content images supported.  
- 🐘 **PostgreSQL** – Reliable relational database for storing users, posts, and comments.  

---

## 🛠️ Tech Stack
- **Backend:** Flask  
- **Database:** PostgreSQL with SQLAlchemy ORM  
- **Authentication:** Flask-Login & Flask-Bcrypt  
- **Forms & Validation:** Flask-WTF + WTForms  
- **Templating:** Jinja2  

---

## 📦 External Libraries / Dependencies
The project uses the following Python libraries:

- **Flask** – Web framework for building the application.  
- **Flask-SQLAlchemy** – ORM for interacting with the PostgreSQL database.  
- **Flask-Bcrypt** – For secure password hashing.  
- **Flask-Login** – User session management and authentication.  
- **Flask-WTF** – Form handling and CSRF protection.  
- **WTForms** – Form fields and validation (StringField, PasswordField, EmailField, FileField, etc.).  
- **PostgreSQL** – Relational database to store users, posts, and comments.  

---

## ⚙️ Setup & Installation

### 1. Clone the repository:
   
   ```bash
   git clone https://github.com/your-username/BytesStories.git
   cd BytesStories
   ```
### 2. Create & activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

### 3. Install dependencies:

``` bash
Copy code
pip install -r requirements.txt
```

### 4. Configure PostgreSQL in config.py:

```bash
SQLALCHEMY_DATABASE_URI = "postgresql://username:password@localhost/bytestories"
```

### 5.Initialize the database:
```bash
flask db init
flask db migrate
flask db upgrade
```

### 6. Run the application:

```bash
Copy code
python run.py
```