# 🍽️ Mini Restaurant Ordering Demo

A simple restaurant ordering demo built using **Next.js**, **Tailwind CSS**, and **Next.js API Routes**.  
This project demonstrates a basic full-stack flow with menu display, order placement, and admin order viewing.

---

## ✅ Task Overview

### **🎯 Objective**
Build a restaurant ordering system where:

- Users can view a list of menu items.
- Users can place an order via a form/modal.
- Admin can view all orders on a separate page.

---

## 🛠️ Tech Stack
- **Next.js**
- **Tailwind CSS**
- **Node.js (Next.js API Routes)**

---

## 📌 Features

### **1. Menu Page (`/`)**
- Fetches menu items from **`/api/menu`**
- Displays items in a clean grid with:
  - Name  
  - Price  
  - Category  
  - Image (dummy/placeholder)
- Each item includes an **“Order Now”** button

---

### **2. Order Modal / Form**
Opens when user clicks “Order Now”.

Form includes:
- Customer Name  
- Table Number / Address  
- Selected Item  

On submit:
- Sends a POST request to **`/api/order`**  
- Shows success or loading state (bonus)

---

### **3. Orders Page (`/orders`)**
- Displays **all placed orders**
- Orders are fetched from **`/api/orders`**
- Useful for admin/testing

---

## 🔧 Backend API Routes

### **GET `/api/menu`**
Returns static menu JSON:
```json
[
  { "id": 1, "name": "Margherita Pizza", "price": 299, "category": "Pizza", "image": "/pizza.jpg" },
  { "id": 2, "name": "Pasta Alfredo", "price": 249, "category": "Pasta", "image": "/pasta.jpg" },
  { "id": 3, "name": "Cold Coffee", "price": 149, "category": "Drinks", "image": "/coffee.jpg" }
]

