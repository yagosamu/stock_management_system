# Stock Management System (SGE)

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Django](https://img.shields.io/badge/Django-5.0.1-green.svg)
![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)
![GitHub](https://img.shields.io/badge/GitHub-yagosamu%2Fstock__management__system-blue.svg)

A comprehensive **Stock Management System** built with Django and Bootstrap 5, featuring AI-powered insights for intelligent inventory management.

## 🚀 Key Features

### 📦 **Core Inventory Management**
- **Product Registration**: Complete product catalog management with detailed information
- **Brand Management**: Organize products by brands with full CRUD operations
- **Supplier Management**: Comprehensive supplier database and relationship management
- **Category Management**: Hierarchical product categorization system
- **Stock Inflows**: Track all incoming inventory with supplier details and timestamps
- **Stock Outflows**: Monitor sales and inventory movements with detailed records

### 🔍 **Advanced Filtering & Search**
- **Product Filters**: Multi-parameter filtering by title, serial number, category, and brand
- **Smart Search**: Real-time search across all inventory items
- **Dynamic Filtering**: Interactive filter combinations for precise inventory queries

### 📊 **Intelligent Stock Management**
- **Automatic Stock Calculation**: Real-time inventory levels based on inflows and outflows
- **Stock Metrics**: Live tracking of product quantities, costs, and values
- **Inventory Alerts**: Automated notifications for stock level management

### 🔐 **Security & Access Control**
- **User Authentication**: Secure login system with session management
- **Permission Control**: Granular user and group-based access permissions
- **Role-Based Access**: Different access levels for various user types
- **Secure Operations**: Permission-controlled create, read, update, and delete operations

### 📈 **Analytics Dashboard**
- **Sales Metrics**: Comprehensive sales performance tracking
- **Stock Analytics**: Real-time inventory value and quantity metrics
- **Interactive Charts**: Visual representation of sales trends and inventory data
- **Performance Graphs**: Daily sales value and quantity visualization
- **Category Analysis**: Product distribution by categories and brands

### 🤖 **AI-Powered Insights**
- **Intelligent Agent**: OpenAI-powered analysis engine for inventory optimization
- **Automated Reports**: Daily AI-generated insights and recommendations
- **Restock Suggestions**: Smart recommendations for inventory replenishment
- **Sales Analysis**: AI-driven sales pattern recognition and forecasting
- **Business Intelligence**: Actionable insights based on historical data

### 🔌 **Integration Ready**
- **API Ready**: Built-in Django REST Framework support for future integrations
- **Scalable Architecture**: Modular design supporting future automations
- **Database Flexibility**: PostgreSQL support with easy migration capabilities
- **Docker Support**: Containerized deployment for seamless scaling

## 🛠️ Technology Stack

- **Backend**: Django 5.0.1, Python 3.11+
- **Frontend**: Bootstrap 5, Chart.js, Bootstrap Icons
- **Database**: PostgreSQL (with SQLite fallback)
- **AI Integration**: OpenAI GPT-4o-mini
- **Authentication**: Django built-in authentication system
- **Deployment**: Docker & Docker Compose ready

## 📋 Prerequisites

Ensure you have the following installed:

- **Python 3.11+**
- **pip** (Python package manager)
- **PostgreSQL** (for production) or SQLite (for development)
- **Git**

## ⚡ Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/yagosamu/stock_management_system.git
cd stock_management_system
```

**Or if you're setting up an existing project:**
```bash
git init
git remote add origin https://github.com/yagosamu/stock_management_system.git
git branch -M main
git pull origin main
```

### 2. Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Environment Configuration
```bash
cp .env.example .env
# Edit .env file with your configurations
```

### 5. Database Setup
```bash
python manage.py migrate
python manage.py createsuperuser
```

### 6. Run the Development Server
```bash
python manage.py runserver
```

Visit [http://localhost:8000](http://localhost:8000) to access the system.

## 📸 Screenshots

### Dashboard Overview
![Dashboard](assets/home.png)
*Main dashboard showing inventory metrics, sales analytics, and AI-powered insights*

### Brand Management
![Brand Management](assets/brands.png)
*Brand management interface with CRUD operations and organized listing*

### Stock Outflows
![Stock Outflows](assets/outflows.png)
*Outflow management system tracking all inventory movements and sales*

## 🤖 AI Configuration

To enable AI-powered insights:

1. **Get OpenAI API Key**: Sign up at [OpenAI](https://platform.openai.com/)
2. **Configure Environment**: Add your API key to `.env`:
   ```env
   OPENAI_API_KEY='your-api-key-here'
   OPENAI_MODEL='gpt-4o-mini'
   ```
3. **Generate AI Insights**: Run the AI agent manually:
   ```bash
   python manage.py sge_agent_invoke
   ```

## 🐳 Docker Deployment

### Quick Docker Setup
```bash
docker-compose up -d
```

This will start:
- **Web application** on port 8000
- **PostgreSQL database** on port 5432
- **All required services** automatically configured

## 📊 Usage Examples

### Dashboard Analytics
- View real-time inventory metrics
- Monitor sales performance
- Track stock movements
- Analyze category and brand distribution

### Inventory Operations
- Add new products with detailed specifications
- Record stock inflows from suppliers
- Process outflows and sales
- Generate automated stock reports

### AI Insights
- Receive daily inventory recommendations
- Get restock suggestions based on sales patterns
- Analyze sales trends and forecasts
- Optimize inventory levels automatically

## 🔒 Security Features

- **CSRF Protection**: Built-in Django CSRF protection
- **SQL Injection Prevention**: Django ORM protection
- **Permission-Based Access**: Granular control over user actions
- **Session Security**: Secure session management
- **Input Validation**: Comprehensive data validation

## 🚀 Future Integrations

The system is designed to support:
- **ERP Integration**: Connect with enterprise resource planning systems
- **E-commerce APIs**: Integrate with online selling platforms
- **Barcode Scanning**: Mobile app integration for warehouse operations
- **Automated Purchasing**: AI-driven automatic reorder systems
- **Advanced Analytics**: Machine learning-powered demand forecasting


---

**Built using Django and AI intelligence for modern inventory management.**
