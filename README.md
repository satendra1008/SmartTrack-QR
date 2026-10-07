# 📦 SmartTrack QR

### AI-Powered Product Tracking & Inventory Management System

SmartTrack QR is a modern web-based product tracking and inventory
management system that uses QR codes to identify products, track their
movement, and manage inventory efficiently.

---

## 🎯 Problem Statement

Traditional inventory systems can make product tracking, movement
monitoring, and stock management difficult.

SmartTrack QR provides a centralized system where products can be
identified using QR codes and their movement can be tracked in real time.

---

## ✨ Features

### 🔐 Authentication

- User registration
- Secure login
- JWT authentication
- Role-based access control
- Admin
- Manager
- Staff

### 📦 Product Management

- Add products
- Edit products
- Delete products
- Search products
- Product categories
- Product status
- Product images

### 📱 QR Code System

- Generate unique QR codes
- Download QR codes
- Print QR codes
- Bulk QR generation
- Scan QR codes using camera

### 📍 Product Tracking

- Track product movement
- Record every scan
- Timestamp scan activity
- Track current location
- Track product status

### 🏭 Inventory Management

- Stock In
- Stock Out
- Warehouse management
- Low-stock alerts
- Inventory monitoring

### 📊 Analytics Dashboard

- Total products
- Total warehouses
- Total scans
- Inventory statistics
- Product movement analytics
- Interactive charts

### 📄 Reports

- PDF reports
- Excel export
- CSV export
- Inventory reports
- Product movement reports

---

## 🛠️ Tech Stack

### Frontend

- React.js
- Vite
- Tailwind CSS
- React Router
- Chart.js

### Backend

- Node.js
- Express.js

### Database

- MongoDB
- SQLite for offline scan storage

### Authentication

- JWT
- Role-Based Access Control

### QR

- qrcode
- html5-qrcode

### Reports

- jsPDF
- XLSX

---

## 🏗️ System Architecture

```text
              ┌──────────────────┐
              │      User        │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │   React + Vite   │
              │    Frontend      │
              └────────┬─────────┘
                       │ REST API
                       ▼
              ┌──────────────────┐
              │ Node.js/Express  │
              │     Backend      │
              └────────┬─────────┘
                       │
             ┌─────────┴─────────┐
             ▼                   ▼
      ┌─────────────┐     ┌─────────────┐
      │   MongoDB   │     │   SQLite    │
      │ Main Data   │     │ Offline Data│
      └─────────────┘     └─────────────┘
