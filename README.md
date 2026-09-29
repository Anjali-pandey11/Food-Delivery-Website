# Food Delivery Website (Tomato)

A frontend food delivery website built with React and Vite. Users can browse a food menu by category, add dishes to a cart, view cart totals, and fill in delivery information at checkout.

## Features

- **Home page** with a hero header ("Order your favourite food here") and a "View Menu" button
- **Explore Menu** with 8 categories: Salad, Rolls, Deserts, Sandwich, Cake, Pure Veg, Pasta, Noodles. Click a category to filter the dishes; click it again to show all
- **Top dishes near you**: a list of 32 food items (4 per category), each with an image, name, rating stars, description and price
- **Add to cart** from each food item, with add / remove quantity counters
- **Cart page** showing item image, title, price, quantity, total, and a remove option, plus:
  - Cart totals (Subtotal, Delivery Fee of $2, Total)
  - Promo code input
  - "Proceed to checkout" button
- **Place Order page** with a delivery information form (first name, last name, email, street, city, state, zip code, country, phone) and cart totals with a "Proceed to payment" button
- **Login / Sign Up popup** with name, email and password fields and a terms checkbox
- **Navbar** with links to home, menu, mobile-app and contact us sections, a search icon, a cart icon with an indicator dot when the cart has items, and a sign in button
- **App download section** with Play Store and App Store badges
- **Footer** with company links, contact details and social icons

## Tech Stack

- [React](https://react.dev/) 19
- [React Router DOM](https://reactrouter.com/) 7
- [Vite](https://vite.dev/) 8
- ESLint
- Plain CSS (one stylesheet per component/page)
- React Context API for cart state management

## Project Structure

```
Food-Delivery-Website/
└── frontend/
    ├── public/
    ├── src/
    │   ├── assets/              # Images, icons and assets.js (menu_list, food_list)
    │   ├── components/
    │   │   ├── AppDownload/
    │   │   ├── ExploreMenu/
    │   │   ├── FoodDisplay/
    │   │   ├── FoodItem/
    │   │   ├── Footer/
    │   │   ├── Header/
    │   │   ├── LoginPopup/
    │   │   └── Navbar/
    │   ├── context/
    │   │   └── StoreContext.jsx # Cart state and helper functions
    │   ├── pages/
    │   │   ├── Cart/
    │   │   ├── Home/
    │   │   └── PlaceOrder/
    │   ├── App.jsx
    │   ├── App.css
    │   ├── index.css
    │   └── main.jsx
    ├── index.html
    ├── eslint.config.js
    ├── package.json
    └── vite.config.js
```

## Routes

| Path          | Page       |
| ------------- | ---------- |
| `/`           | Home       |
| `/cart`       | Cart       |
| `/placeOrder` | PlaceOrder |

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) and npm

### Installation

```bash
# Clone the repository
git clone https://github.com/Anjali-pandey11/Food-Delivery-Website.git

# Go to the frontend folder
cd Food-Delivery-Website/frontend

# Install dependencies
npm install
```

### Run the development server

```bash
npm run dev
```

### Available scripts

| Command           | Description                          |
| ----------------- | ------------------------------------ |
| `npm run dev`     | Start the Vite development server    |
| `npm run build`   | Build the app for production         |
| `npm run preview` | Preview the production build locally |
| `npm run lint`    | Run ESLint                           |
