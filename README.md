# BookstoreApp 📚 
**Angular 19 + Stripe E-Commerce Solution**

🔗 [Live Website](https://kitaabi-zeta.vercel.app/)  
🎬 [Demo Video](https://www.youtube.com/watch?v=LVSavDxwY_Q)

---

## 🧾 Project Overview  
A full-featured bookstore application with:

- ✅ Angular 19 frontend  
- ✅ Node.js + Express backend API  
- ✅ Stripe payment integration  
- ✅ Responsive Material UI design  

---

## 🌟 Key Features  

### 📚 Book Management  
- Browse books by category  
- Search with filters  
- Shopping cart system  

### 💳 Secure Payments  
- Stripe Checkout integration  
- PCI-compliant flows  
- Order history tracking  

---

## 🛠️ Tech Stack  

| Layer      | Technology          |
|------------|---------------------|
| Frontend   | Angular 19          |
| Backend    | Node.js / Express   |
| Database   | MongoDB             |
| Payments   | Stripe API          |
| UI         | Angular Material    |

---

# 🏗️ Project Architecture

The application follows a modular and scalable folder structure, with clear separation of concerns and best practices in Angular:

```
bookstore-app/
├── src/
│   └── app/
│       ├── auth/                # Login, registration
│       ├── core/                # Global services, guards, models, pipes, validators
│       ├── dashboard/           # Main dashboard views
│       ├── features/            # Core business features
│       │   ├── books/           
│       │   ├── cart/            
│       │   ├── checkout/        
│       │   ├── order-history/   
│       │   ├── order-details/   
│       │   ├── wishlist/        
│       │   ├── home/            
│       │   ├── success/         
│       │   └── ...              
│       ├── layouts/             # Header, Footer, layout wrappers
│       ├── shared/              # Reusable components (e.g., confirm-dialog)
│       ├── app.component.*      # Root component
│       ├── app.config.ts        # Global configuration
│       └── app.routes.ts        # App routing setup
├── api/                         # Node.js backend (Express)
│   ├── routes/
│   │   ├── books.js             # Product endpoints
│   │   └── payments.js          # Stripe integration
│   └── ...
├── database/                    # Mock data or DB setup for dev
```

## 📐 Design Principles:

- **Feature-Based Modularization:** Business logic is encapsulated under `features/` (e.g., cart, books, checkout).
- **Core Module:** Centralized single-use services, guards, and global utilities.
- **Shared Module:** Houses reusable components and utilities used across features.
- **Separation of Concerns:** Clear distinction between authentication, layout, core logic, and features.
- **Routing & Configuration:** Clean routing in `app.routes.ts` and global configs in `app.config.ts`.

---

## ⚡ Setup Guide  

### 1. Install Dependencies  
```bash
# Frontend
cd bookstore-app
npm install

# Backend 
cd api
npm install
