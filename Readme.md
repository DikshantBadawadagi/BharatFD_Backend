# 🌐 Multilingual FAQ System  

A Django-based FAQ management system with multilingual support, WYSIWYG editor integration, and efficient caching for seamless performance.  

---

## 🚀 Features  

- 🌍 **Multilingual Support:** Manage FAQs in English, Hindi, and Bengali.  
- 📝 **WYSIWYG Editor:** Rich text editing with **django-ckeditor** integration.  
- 🔄 **Automatic Translation:** Powered by the **Google Translate API** for quick language switching.  
- ⚡ **Caching:** Optimized performance with smart caching mechanisms.  
- 📡 **RESTful API:** Flexible API endpoints with dynamic language selection.  
- 🎛️ **Django Admin Interface:** Comprehensive and user-friendly admin dashboard.  

---

## 🛠️ Tech Stack  

- **Framework:** Django  
- **Editor:** django-ckeditor  
- **Translation:** Google Translate API  
- **Caching:** Django Caching Framework  
- **Database:** SQLite (default, can be configured for PostgreSQL/MySQL)  
- **API Testing:** pytest  

---

## 📥 Installation Guide  

### 1️⃣ Clone the Repository  
```bash
https://github.com/DikshantBadawadagi/BharatFD_Backend.git
cd faq_multilingual 
```

### 2️⃣ Create the virtual environment
```bash
# Create virtual environment
python -m venv venv
```

### 3️⃣ Activate the virtual environment
```bash
# Activate on Windows
venv\Scripts\activate

# Activate on macOS/Linux
source venv/bin/activate
```

### 4️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 5️⃣Add your environment variables

### 6️⃣ Apply Migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

### 7️⃣ Run the server
```bash
python manage.py runserver
```
### Your application will be live at:
📍 http://127.0.0.1:8000/

---

### 📡 API Usage

### 🔍 List All FAQs
```bash
GET /api/faqs/
```

### 🌐 Get FAQs in a Specific Language
```bash
GET /api/faqs/?lang=hi   # For Hindi
GET /api/faqs/?lang=bn   # For Bengali
```

### ➕ Create a New FAQ
```bash
POST /api/faqs/
Content-Type: application/json

{
    "question": "How does caching improve website performance?",
    "answer": "Caching stores frequently accessed data temporarily, reducing server load and improving response times."
}
```

---

### ✅ Running Tests
Run the full test suite using pytest:
```bash
pytest
```

---

### 🤝 Contributing
### Fork the repository

### Create your feature branch:
```bash
git checkout -b feature/awesome-feature
```
### Commit your changes:
```bash
git commit -m 'Add awesome feature'
```
### Push toi your branch:
```bash
git push origin feature/awesome-feature
```

---

### 🚀 Made with ❤️ using Django
