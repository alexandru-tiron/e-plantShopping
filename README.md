# Paradise Nursery - e-PlantShopping

A modern React application for shopping a variety of plants, featuring a fully functional shopping cart with Redux Toolkit for state management.

## Features

-  Browse plants by category (Air Purifying, Aromatic, Insect Repellent, Medicinal, Low Maintenance)
-  Add plants to a global cart (with quantity management)
-  View and update cart contents (increment, decrement, remove items)
-  See total and per-item costs in the cart
-  Responsive, modern UI
-  State management with Redux Toolkit

## Technologies Used

-  React
-  Redux Toolkit
-  React Redux
-  Vite (for fast development)
-  CSS Modules

## Getting Started

### Prerequisites

-  Node.js (v14 or higher recommended)
-  npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd e-plantShopping
   ```
2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

### Running the App

```bash
npm run dev
# or
yarn dev
```

Visit [http://localhost:5173](http://localhost:5173) in your browser.

## Project Structure

```
src/
  App.jsx           # Main app component
  ProductList.jsx   # Product listing and add to cart
  CartItem.jsx      # Cart view and management
  CartSlice.jsx     # Redux slice for cart state
  store.js          # Redux store setup
  ...
```

## Redux Store

-  The Redux store is set up in `store.js` and provided globally via the `Provider` in `main.jsx`.
-  Cart state is managed in `CartSlice.jsx` with reducers for adding, removing, and updating item quantities.
-  All cart actions and state are accessed via React Redux hooks (`useSelector`, `useDispatch`).

## Cart Functionality

-  Add to Cart: Adds a plant to the cart or increases its quantity if already present.
-  Remove: Removes a plant from the cart.
-  Increment/Decrement: Adjusts the quantity of each plant in the cart.
-  Cart badge: Shows the total number of items in the cart in the navbar.
-  Cart state is persistent as long as the app is running.

## Customization

-  You can easily add more plant categories or products by editing the `plantsArray` in `ProductList.jsx`.

## Deployment

-  You can deploy this app to GitHub Pages, Vercel, Netlify, or any static hosting provider.


