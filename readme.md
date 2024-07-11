# Udgam Product Project

This project consists of two parts:
- **Udgam Product (Frontend)**: A React application.
- **Product Backend**: A Node.js backend with MySQL database.

## Backend Setup

### Prerequisites
- Node.js installed
- MySQL database setup

### Steps to Run Backend

1. Clone the repository:
   ```bash
   git clone repo
   cd product-backend
   use your database credential in config/db.js file. And keep table name as products .if you want to change so change it in models/products.js as well.
   run: - node index.js

### Steps to Run frotend

```bash
  cd udgam-product
  npm install
  npx create-react-app@latest
  npm install -D tailwindcss postcss autoprefixer
  npx tailwindcss init -p

 Add the paths to all of your template files in your tailwind.config.js file:
```bash
** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./app/**/*.{js,ts,jsx,tsx,mdx}",
    "./pages/**/*.{js,ts,jsx,tsx,mdx}",
    "./components/**/*.{js,ts,jsx,tsx,mdx}",

    // Or if using `src` directory:
    "./src/**/*.{js,ts,jsx,tsx,mdx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
};
```
 Run the following command to install flowbite-react:
```bash npm i flowbite-react```

 Add the Flowbite React content path and plugin to tailwind.config.js:
```bash
const flowbite = require("flowbite-react/tailwind");

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    // ...
    flowbite.content(),
  ],
  plugins: [
    // ...
    flowbite.plugin(),
  ],
}; ```

```npm start```
