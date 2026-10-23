# Paradise Nursery Shopping Application

Welcome to **Paradise Nursery**, an online plant store shopping application developed with **React**, **Redux Toolkit**, and **Vite**. This application provides a seamless e-commerce experience for plant lovers to explore a curated selection of houseplants, learn about their unique benefits, and manage their cart effortlessly.

---

## 🌿 Table of Contents
- [Project Overview](#-project-overview)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Grading Tasks & Implementation Details](#-grading-tasks--implementation-details)
- [Getting Started](#-getting-started)
- [Author & License](#-author--license)

---

## 🌱 Project Overview
**Paradise Nursery - Where Green Meets Serenity** is designed to bring nature closer to everyday living spaces. The web application allows users to:
1. Land on an interactive Welcome / Landing page featuring company details, mission statement, and a "Get Started" call-to-action button.
2. Browse a variety of houseplants organized into multiple distinct categories (Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, and Low Maintenance).
3. View high-quality thumbnails, names, descriptions, and prices for at least six unique plants per category.
4. Add plants to the shopping cart, disabling the "Add to Cart" button once selected to prevent duplicate single-add errors.
5. Track cart totals dynamically in the navigation bar via a responsive cart icon badge.
6. Open the Shopping Cart page to adjust item quantities (+ / -), remove items, view itemized totals and overall cart cost, continue shopping, or proceed to checkout.

---

## ✨ Features
- **Dynamic Landing Page**: Elegant greenhouse background image, welcome banner, and About Us section.
- **Categorized Houseplants**: More than 30 unique houseplants spread across 5 functional categories.
- **Redux State Management**: Centralized global state using Redux Toolkit (`CartSlice.jsx`) with actions:
  - `addItem`: Adds plant to cart or increments quantity.
  - `removeItem`: Deletes an item from the cart.
  - `updateQuantity`: Adjusts item quantity dynamically.
- **Interactive Navigation Bar**: Persistent navigation present on both product listing and cart views with links to Home, Plants, and Cart.
- **Dynamic Cart Counter**: Live badge on the cart icon indicating total item quantity.
- **Full Shopping Cart Functionality**:
  - Item thumbnail, name, unit price, quantity controls, and subtotal.
  - Decrementing to 0 removes the item automatically or via the Delete button.
  - Overall total cart cost calculation.
  - "Continue Shopping" button returning to the product catalog.
  - "Checkout" button displaying a "Coming Soon" notification.

---

## 🛠 Technologies Used
- **React 18** (Functional Components, Hooks: `useState`, `useEffect`)
- **Redux Toolkit (`@reduxjs/toolkit`) & React-Redux (`react-redux`)**
- **Vite** (Next-generation frontend tooling and bundler)
- **HTML5 & Vanilla CSS3** (Responsive design, CSS Flexbox & Grid, media queries)

---

## 📁 Project Structure
```text
React/
├── public/
├── src/
│   ├── assets/
│   ├── AboutUs.css          # Styling for About Us section
│   ├── AboutUs.jsx          # Company background and mission details
│   ├── App.css              # Landing page styles and background image
│   ├── App.jsx              # Main application entry with landing page toggle
│   ├── CartItem.css         # Shopping cart view styles
│   ├── CartItem.jsx         # Cart display, quantity adjustment & checkout
│   ├── CartSlice.jsx        # Redux Toolkit slice managing cart state
│   ├── ProductList.css      # Catalog & navigation bar styling
│   ├── ProductList.jsx      # Plant listing grouped by categories & navbar
│   ├── index.css            # Base stylesheet
│   ├── main.jsx             # React DOM root render with Redux Provider
│   └── store.js             # Redux store configuration
├── index.html               # Main HTML template
├── package.json             # Dependencies and build scripts
├── README.md                # Project documentation and details
└── vite.config.js           # Vite configuration
```

---

## 📝 Grading Tasks & Implementation Details
- **Task 1: README.md** - Contains comprehensive project name, overview, and feature documentation.
- **Task 2: AboutUs.jsx** - Provides informative details on Paradise Nursery's passion, mission, and plant quality assurance.
- **Task 3: App.css** - Implements the full-screen greenhouse background image and responsive landing page layout.
- **Task 4: App.jsx** - Implements the Paradise Nursery landing page, company heading, tagline, and "Get Started" button.
- **Task 5: CartSlice.jsx** - Implements Redux Toolkit state slice for `addItem`, `removeItem`, and `updateQuantity`.
- **Task 6: ProductList.jsx** - Renders plant categories with thumbnails, prices, descriptions, disabled "Added to Cart" state, and dynamic navbar cart count.
- **Task 7: CartItem.jsx** - Implements itemized costs, total cart calculation, quantity modification (+ / -), deletion, continue shopping, and "Coming Soon" checkout alert.

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v16.0.0 or higher recommended)
- npm (v8.0.0 or higher)

### Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`.

5. Build for production:
   ```bash
   npm run build
   ```

---

## 📄 License
This project is open-source and available under the MIT License.