# Saintgits College Kiosk

A comprehensive web-based kiosk system designed for college environments, enabling seamless food and item ordering, inventory management, and classroom delivery tracking.

## 🚀 Overview

The Saintgits College Kiosk is a full-stack web application that streamlines the process of ordering items from the college canteen or kiosk. It provides distinct interfaces for students, staff, and administrators, ensuring a smooth workflow from order placement to delivery/pickup.

## ✨ Key Features

### 👤 User Management
- **Role-Based Access:** Dedicated interfaces for Admins, Staff, and regular Users.
- **Secure Authentication:** Password hashing using SHA-256.
- **Approval Workflow:** New user registrations require administrator approval before access is granted.

### 🍴 Menu & Inventory
- **Dynamic Menu:** Categorized item listing with real-time availability.
- **Stock Tracking:** Automatic stock deduction upon successful order placement.
- **Management Tools:** Add, update, or delete menu items with support for image uploads.

### 📦 Order System
- **Real-time Ordering:** Students can browse and add items to a digital cart.
- **Delivery/Pickup Options:** Supports both self-pickup and classroom delivery.
- **Location Awareness:** For deliveries, users can specify Block, Department, and Classroom.
- **OTP Verification:** Secure pickup/delivery verification via generated OTPs.
- **Status Tracking:** Monitor order progress from "Order Received" to "Delivered".

### 🛠 Administrative Controls
- **Admin Dashboard:** Central hub for managing users, roles, and approvals.
- **Activity Logging:** Tracks administrative actions for audit trails.
- **Notifications:** Send system-wide or targeted notifications to users.

## 🛠 Tech Stack

- **Backend:** [Flask](https://flask.palletsprojects.com/) (Python)
- **Database:** [SQLite](https://www.sqlite.org/)
- **Frontend:** HTML5, Modern CSS3 (Vanilla), JavaScript (ES6+)
- **Storage:** Local filesystem for optimized image serving

## 📂 Project Structure

```text
├── backend/
│   ├── app.py           # Main Flask application and REST APIs
│   └── static/          # Backend-specific static assets
├── frontend/
│   ├── index.html       # Landing and Login page
│   ├── register.html    # User Registration
│   ├── users.html       # Student/User Dashboard
│   ├── staff.html       # Staff/Counter Dashboard
│   ├── admin.html       # Administrator Dashboard
│   ├── admin.js/css     # Admin-specific logic and styling
│   ├── users.js/css     # User-specific logic and styling
│   └── staff.js         # Staff-specific logic
├── college.db           # SQLite database
├── requirements.txt     # Python dependencies
└── static/images/       # Uploaded menu item images
```

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.8+
- pip (Python package manager)

### Steps
1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd college-kiosk
   ```

2. **Set up a Virtual Environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   *Note: Ensure `Flask` and `flask-cors` are installed.*

4. **Run the Application:**
   ```bash
   python backend/app.py
   ```

5. **Access the Application:**
   Open your browser and navigate to `http://127.0.0.1:5000`.

## 🔑 Default Credentials
- **Admin Email:** `kioskadmin@saintgits.org`
- **Admin Password:** `QAZwsx1!` (Configurable in `app.py`)

## 📄 License
This project is developed for college academic purposes.
