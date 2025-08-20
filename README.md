
# 🚗 Workshop Management App (English)

**Cross-platform Car Workshop Inventory Management App**  
Manage products, transactions, and stock alerts offline with Flutter & SQLite. Backend powered by Python Flask.

---

## 📋 Project Description

This app is designed to help car workshops track inventory, monitor product movement, and generate alerts for low stock.  

**Key Features:**
- Add, update, and delete products  
- Record incoming/outgoing transactions  
- Low stock automatic alerts  
- Dashboard with stock overview  
- Offline mode with SQLite (optional sync with Flask backend)  
- Cross-platform: Android & iOS  

---

## 🗂 Folder Structure

📁 **backend/**  
├── 📝 `app.py` - Main Flask API  
├── 📝 `models.py` - SQLite Models (Product, Transaction)  
└── 📦 `requirements.txt` - Python dependencies  

📁 **frontend/**  
├── 📝 `pubspec.yaml` - Flutter dependencies  
├── 📁 `lib/`  
│   ├── `main.dart` - Main app + Drawer  
│   ├── 📁 `screens/`  
│   │   ├── `dashboard.dart` - Stock overview + alerts  
│   │   ├── `product_list.dart` - List all products  
│   │   ├── `product_add.dart` - Add new product  
│   │   └── `transaction.dart` - Record transactions  
│   ├── 📁 `services/`  
│   │   └── `database_service.dart` - SQLite CRUD operations  
│   └── 📁 `widgets/`  
│       └── `alert_widget.dart` - Custom low-stock alert (optional)  
└── 📁 `assets/images/` - Icons, logos, screenshots  

---

## 🖼 Screenshots

![Dashboard](assets/images/dashboard.png)  
![Product List](assets/images/product_list.png)  
![Add Product](assets/images/product_add.png)  

*Screenshots are placeholders. Replace with your app UI images.*

---

## 🔧 Setup Instructions

### Backend (Flask)
```bash
cd backend
python -m venv venv       # create virtual environment
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
pip install -r requirements.txt
python app.py
