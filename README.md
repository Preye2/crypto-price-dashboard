# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

# Crypto Prices Dashboard

A React application that displays cryptocurrency prices and market data using the CoinGecko API.

## Features

- Display cryptocurrency prices, market cap, and 24h change
- Sort cryptocurrencies by different metrics
- Adjust number of displayed cryptocurrencies
- Responsive design for all screen sizes
- Error handling for API failures
- Loading state while fetching data

## Technology Stack

- React 19
- Vite for build tooling and development server
- CoinGecko API for cryptocurrency data
- CSS for styling (no external UI libraries)

## Project Structure

// Project Structure:

crypto-dashboard/
├── node_modules/
├── public/
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── CryptoDashboard.jsx
│   │   ├── CryptoList.jsx
│   │   ├── CryptoItem.jsx
│   │   ├── LoadingSpinner.jsx
│   │   └── ErrorMessage.jsx
│   ├── App.jsx
│   ├── App.css
│   ├── main.jsx
│   └── index.css
├── .eslintrc.cjs
├── index.html
├── package.json
├── vite.config.js
└── README.md


The application is structured with reusable components:
- CryptoDashboard: Main container component
- CryptoList: Reusable list component for showing cryptocurrency data
- CryptoItem: Component for each individual cryptocurrency
- LoadingSpinner: Component shown during API calls
- ErrorMessage: Component displayed when API calls fail

## Running the Project

1. Install dependencies:
   ```
   npm install
   ```

2. Start the development server:
   ```
   npm run dev
   ```

3. Open http://localhost:3000 in your browser

## API Integration

The application uses the CoinGecko API to fetch real-time cryptocurrency data. The main endpoint used is:
```
https://api.coingecko.com/api/v3/coins/markets
```

[Proof of Implementation](https://github.com/Preye2/crypto-price-dashboard/blob/276e708ecd8b75191f340e2d0d3e6cf75cb6210e/proof-of-implementation.jpg)
