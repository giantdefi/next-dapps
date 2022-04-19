Add Tailwinds Css to the basic NextJS application

## Install Tailwinds css
Run this comment in the console :

```bash
yarn add tailwindcss postcss-cli autoprefixer -D

yarn tailwindcss init -p  
```

It will create tailwind.config.js. Modify this file to enable css to all files inside 'pages' folder :

```bash
module.exports = {
  content: [
    "./pages/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

Modify global.css in /styles folder :

```bash
@tailwind base;
@tailwind components;
@tailwind utilities;

```

That's all...!

## Deploy on Vercel

Check out the deployed of this script [https://next-dapps.vercel.app/](https://next-dapps.vercel.app/) 
